## Determine JSS Content Presentation
### Define Component Rendering
> JSS injects the content data from the mock or Sitecore Layout Service to a page. A Component in the framework template is rendering of the JSS component that use the router library to sync the framework library and allows navigation between pages.

**Render Components**
 Common Features
1- Compare Scaffolding Types
- JSS Scaffolding differs from traditional Sitecore Scaffolding
	- in Sitecore-first app, the task of adding new component involves a repetitive set of steps (e.g. create a rendering item, dataosource template item, datasource location folders and then linking them together)
	- JSS Scaffolding creates the framework component (e.g. VUE)

2- Identify Scaffolding Scripts
- is located in **scripts/scaffold-component.js** and is fully customizable. (you can customize manifest on same file)
- also change component factory generation script **scripts/generate-component-factory.js**
- JSS layout is used just to indicate that you are using JSS and points to an empty Razor view. Whereas in traditional Sitecore, layout is pointing to CSHTML

3- Components Definitions
- you create the component definitions and their files in JSS to export to Sitecore.

4- Register Component
- create component manifest defintion file e.g. **OurNewComponent.sitecore.js**
- allow JSS to detect the component.
- enable adding component instances to routes.

**Create New Component and add it to Navigation**
- `$ jss scaffold OurNewComponent`
- Update `/src/components/OurNewComponent.vue` to add your component logic e.g. RichText, Text, etc.
- Update fields on `/sitecore/definitions/components/OurNewComponent.sitecore.js` to match `/src/components/OurNewComponent.vue`
- Create Folder with Components Name [^1] e.g `/test` and `YAML` file in it > `en.yml`
- Add components Route and definitions `YAML` File: `/data/routes/en.yml`
- Update component `/Navigation.vue` to add your component to the navigation

[^1]: Name of the folder should be the same as the component name.

New components are generated in:
| File Location | Description |
|:---:|---|
| `/scripts/scaffold-component.js` | fully customizable, <br>Customizable Manifest  |
| `/scripts/generate-component-factory.js` | Modified in case you want to match <br>Nested Components |
| `/sitecore/definitions/components/OurNewComponent.sitecore.js` | Component Manifest |
| `/src/components/OurNewComponent/index.js` | To access `Route-Level` Fields |

---
**Add field to component manifest**
