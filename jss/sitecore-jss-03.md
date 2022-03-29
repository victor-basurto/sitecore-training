## Determine JSS Content Presentation
### Define Component Rendering
> JSS injects the content data from the mock or Sitecore Layout Service to a page. A Component in the framework template is rendering of the JSS component that use the router library to sync the framework library and allows navigation between pages.

**Render Components**
 Common Features
1- Compare Scaffolding Types
- JSS Scaffolding differs from traditional Sitecore Scaffolding
	- in Sitecore-first app, the task of adding new component involves a repetitive set of steps (e.g. create a rendering item, datasource template item, datasource location folders and then linking them together)
	- JSS Scaffolding creates the framework component (e.g. VUE)

2- Identify Scaffolding Scripts
- is located in _**scripts/scaffold-component.js**_ and is fully customizable. (you can customize manifest on same file)
- also change component factory generation script _**scripts/generate-component-factory.js**_
- JSS layout is used just to indicate that you are using JSS and points to an empty Razor view. Whereas in traditional Sitecore, layout is pointing to CSHTML

3- Components Definitions
- you create the component definitions and their files in JSS to export to Sitecore.

4- Register Component
- create component manifest definition file e.g. **OurNewComponent.sitecore.js**
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
| Description | File Location |
|---|---|
| fully customizable, <br>Customizable Manifest  | `/scripts/scaffold-component.js` |
| Modify in case you want to match <br>Nested Components | `/scripts/generate-component-factory.js` |
|  Component Manifest | `/sitecore/definitions/components/OurNewComponent.sitecore.js` |
| To access `Route-Level` Fields | `/src/components/OurNewComponent/index.js` |

---
### **Add field to component manifest**
> _Adding fields to component manifest allow us to create component instances with different fields._

The **Layout Service Placeholders** field defines the placeholders that will be used within the rendering in your Javascript component.
It emits **field** data in two formats: **Value** and **Editable**
- **Value**: 
The **value** property of a field object contains the "raw" un-rendered value of a filed stored in Sitecore.
- **Editable**:
The **editable** property of a field object contains the result of the `renderField` pipeline for the given field.
```javascript
export default function(manifest) {
  manifest.addComponent({
    name: 'OurNewComponent', // -> Component name
    icon: SitecoreIcon.DocumentTag,
    fields: [{ 
		name: 'heading', // field name
		type: CommonFieldTypes.SingleLineText // heading field as SingleLineText
	}, {
		name: 'description', // field name
		type: CommonFieldTypes.RichText // description field as RichText
	}], // add more fileds
  });
}
```
### **Define a Text String**
Located under `~/data/routes/en.yml`
After added new Component, add definitions into `en.yml` file. 
<sub>Note: _Make sure it matches Component Manifest settings_</sub>
```yaml
- componentName: OurNewComponent //-> should match manifest component name
  fields:
	- heading: My Custom Heading
	- description: My Custom Description
```

