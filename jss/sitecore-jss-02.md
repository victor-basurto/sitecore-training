## Maintain APP Directories
> NOTE: In order to connect the JSS app to Sitecore, the manifest is imported into Sitecore, which creates the necessary structures to support the app.

**Role of the Manifest API**
- Defines the structure of your JSS site
- Runs the Site Mocked Data
- Imports the site into Sitecore

In **disconnected mode**, the Manifest API creates a manifest of the JSS app's content.
- Includes content data and data schema with both components and routes from a set of files.
- Enables JSS to execute local mock content without Sitecore instance.
- Assigns JSS app as master copy

**App's Main Directory Elements**
_Three Types `Arbitrary Content`, `Routes` and `Components`_
- Arbitrary Content:
	- They're not used as **pages** or **datasources**
	- Referred as **"_lookups_"** or **"_list items_"**
	- **Can't** be viewed in browser because there are no layout data.

- Routes:
	- They're used as **pages**
		- **can** be viewed in browsers using **unique URLs**
		- contain **route-level fields** to lay out the **route’s components**.
	- Site implementations may need multiple route types to capture route-level fields also known as  **"_templates_"**

- Components:
	- **_Rendering Datasources_**
	- **_Component-Level Fields_** - Can't viewed in browser because there are no layout data.

---
### Purpose of Routes
**Traditional JS APP vs Sitecore JSS APP**
| Traditional JS APP | Sitecore JSS APP |
|---|---|
| Each Route Hosts Known Components | Disconnected data defines route's component and data |
| Components are Static [^1] | `JSS` extends Sitecore's dynamic component-based layout model  |
|  | Raw data from `YAML` or `JSON` |

[^1]: Static Component does not have datasource and displays non-customizable data.

JSS Two features to define Routes
: JSS Library
The Layout Service - Presentation Layer that provides composition for data needed in component

**Mock Layout Service**
- Consistent API to create complex Single Page JSS Applications
- Integration with Sitecore
- Disconnected JSS app is essentially built to consume and render a data-driven layout available via Mock Layout Service
- Component data is a set of fields from the datasource item.
- Mock returns JSON

> When connecting to JSS app to Sitecore:
> - Currently no built-in tool into JSS SDK to retrieve and store Sitecore-connected Layout Service data as Files.
> - Save Layout Service data queried from Sitecore in a JSON file.
> - Once you have that data disconnected you might consider building your own service layer to fetch "raw" Layout Service data from the JSON file(s) you saved.

### Routes and Templates
- Templates: you put a template with static component data in **data/component-content** folder of the sample library to share static component data.
To add components into multiple routes while reusing same data, put that component data into **component-content**

| Routes | Templates |
|---|---|
| are items in a page that map, or correspond, to a route | do not have presentation as they are arbitrary content.|
| Every file under `Routes` becomes a page |   |
| are made from templates |  |

Templates live inside **component-content** folder.

---
### Fields on Routes vs Components
Each JSS app has one default route template, `routes.sitecore.js`

> - Add fields to components when they are generic fields -> this allows multiple  component datasource.
> - Add fields to routes if you'll be doing a lot of filtering and searching.
> - JSS import process will always generate a route template for each app.
---

#### Steps to create a Route
Adding a `addRouteType`
1- VSCode navigate to **/sitecore/definitions/routes.sitecore.js** folder and then create a **routes** folder.
- copy and paste the **routes.sitecore.js** file in **/sitecore/definitions/routes**
- rename to **[Pagename]Route.sitecore.js** [^2]

2- use the API `addRouteType` function to:
- call for new routes
- its how you add a route type with a name and fields
- it can add inherited data.

```javascript
import { CommonFieldTypes, Manifest } from '@sitecore-jss/sitecore-jss-manifest';

export default function (manifest) {
  manifest.addRouteType({
    name: 'my-route-type',
    displayName: 'My Route Type',
    fields: [{
      name: 'description', // -> Make sure it matches Definition File
      type: CommonFieldTypes, RichText,
      displayName: 'Description',
      required: false,
    }],
  });
}
```

Adding Template Property
- **[Pagename]Route.sitecore.js** to add a template property
- add the files that matches the route name, to tell JSS is a custom route.

```json
{
	"name": "route",
	"template": "MyRoute",
	"displayName": "Route",
	"placeholders": {
		// ...
}
```

Create New Route Folder under `/data/routes/` make sure it matches the _manifest file_ route[^3]. e.g. `/data/routes/my-route-type/`

Create a new `YML` file under `/data/routes/my-route-type/` and name it: `en.yml




> After first import to Sitecore, any existing route type data templates will remain unchanged until you:
- Manually delete them.
- Manually change them.
- Utilize Full Wipe Mode during development.

---
### Inspect JSS App Templates
**Identify Template Contents**
- all the boilerplate code in the config file to run the app using (angular, vue or react)
- a sample website to get you started with JSS

How route items and the database are defined after JSS setup completes?
- JSS setup creates a config file that generates the site definition.

[^2]: Manifest definition file ned to have the **\*path.basename** as **\*.sitecore.js** for the following reasons: Sitecore file-naming convention. When manifest generation runs, it will only look to generate files that end with **sitecore.js**

[^3]: Sitecore will translate the route name to a folder name. 
e.g `my-route-type` will be translated to `https://www.my-sitecore-app.com/my-route-type/`

