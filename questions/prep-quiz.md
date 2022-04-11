## Prep QUIZ
##
**Q:** What are the types of publishing?

**A:** Delayed, parallel an dedicated
##
**Q:** What is the name of the template all templates should inherit from?

**A:** Standard Template
##
**Q:** When would you set languageEmbedding option to never?

**A:** Site is not multilingual
##
**Q:** Where should i set insert options as best practice?

**A:** Standard Values
##
**Q:** What does an unversioned field contain?

**A:** Data for all version in all languages
##
**Q:** Which of the following are reasons for using field types in Sitecore?

**A:** To define the raw value stored in the database, to determine which editor control will be used in the authoring tools, to determine the API field class used in code.
##
**Q:** What are the 3 folders in the physical path of the content folder that hosts the Sitecore application?

**A:** Website, data, and database
##
**Q:** Which method is not supported by Sitecores implementation of `Iqueryable<T>`?

**A:** `GroupBy`
##
**Q:** What does it do when you make an item bucketable?

**A:** the item is hidden
##
**Q:** What is Sitecores easy-to-use authoring tool and what functionality does it provide?

**A:** The Experience Editor provides editing and designing functionality.
##
**Q:** What is the best way to source control Sitecore items?

**A:** Serializing them
##
**Q:** What item setting needs to be specified for authors to be able to add content?

**A:** Insert Options
##
**Q:** What is the preferred way to modify the `web.config`?

**A:** Use .config file in `App_Config/Include`
##
**Q:** Which interface would an author use to see and edit items in a tree structure?

**A:** Experience Editor
##
**Q:** Select the name of the Sitecore component-based architecture guidelines from the list.

**A:** Helix
##
**Q:** When you patch in changes to the `Sitecore.config` file, how can you control the order in which your changes are applied?

**A:** In `App_Config/Include`, use a naming convention and sub-folders for config files
##
**Q:** Where is the license located?

**A:** Sitecore application root `folder/Data/license.xml`
##
**Q:** What do you need to create to enable Dynamic Binding?

**A:** Placeholder
##
**Q:** When would you use the DisableWebEdit parameter when rendering a field?

**A:** When rendering a field inside the` <title>` tag in the `<head>` of HTML
##
**Q:** What happens if an item version is not in a final workflow state?

**A:** No automatic versioning and version is not publishable.
##
**Q:** Publishing synchronizes what between master and web databases?

**A:** Adding new items, updating edited items, removing deleted or unpublishable items.
##
**Q:** What happens if a role denies an access right and another one allows it?

**A:** Deny
##
**Q:** Where can I check the effective permission of an account?

**A:** Access viewer
##
**Q:** What is a Sitecore item?

**A:** The construct Sitecore uses to store data
##
**Q:** What part of presentation details applies to all versions of an item?

**A:** Shared Layout
##
**Q:** What field type can I use with Rendering Parameters?

**A:** All field types
##
**Q:** What should you define in a template?

**A:** Fields, Field Sections, Icons and Base Templates
##
**Q:** How do I display the content of a field in code?

**A:** `@Html.Sitecore().Field(<field name>)`
##
**Q:** How can I use placeholders inside of placeholders?

**A:** This cannot be done directly.
##
**Q:** What does the item Resolver do?

**A:** Maps a URL to an item in the content tree.
##
**Q:** Config changes get added alphabetically by default. How can I change it?

**A:** `<loadOrder>`
##
**Q:** Select the name of the Sitecore component-based architecture guidelines from the list.

**A:** `/App_Config/Include/c/a.config`
##
**Q:** How would you retrieve the URL of an item?

**A:** Use `LinkManager.GetItemUrl()`
##
**Q:** Which field type do I use to store formatted html

**A:** Rich text field
##
**Q:** How does Sitecore support one of the CMS pillars, Presentation?

**A:** Layouts and components
##
**Q:** What parts of the page are typically added using Static Binding?

**A:** Scaffolding, like headers and footers
##
**Q:** Why would you use dynamic placeholders

**A:** To reuse a component containing placeholders.
##
**Q:** How can I open a bucketable item?

**A:** Use the Sitecore search functionality to locate and open the item.
##
**Q:** How can you handle more than one input form on a controller rendering in Sitecore?

**A:** Create an extension method invoking the `FormHandler()` and Use `Ajax.BeginForm()` and specify the controller and action.
##
**Q:** Where does Master database publish items to?

**A:** Master database
##
**Q:** What are the SIM Import/Export features?

**A:** Export an entire set of Sitecore database with content and import to a new environment.

##
**Q:** What happens if the same field name is used in two separate inherited data templates?

**A:** The field will be duplicated.
##
**Q:** Where can Presentation Details be set?

**A:** Experience Editor (Design Mode), Content Editor, Template Manager, Sitecore Rocks
##
**Q:** What happens when an item inside a bucket is not bucketable?

**A:** Item is not hidden.
##
**Q:** What is the CMS parts of Sitecore?

**A:** xManagement
##
**Q:** What can I use to translate fields and help texts in the Sitecore client?

**A:** Sitecore Dictionary entries
##
**Q:** What tools can I use to install Sitecore?

**A:** Manual or zip file, Scripts, Sitecore Rocks, SIM, EXE
##
**Q:** When I made Template bucketable, the existing items are still not hidden. What should I do?

**A:** Sync the existing items.
##
**Q:** Which search providers does Sitecore ship with by default?

**A:** Solr and Azure Search
##
**Q:** What do you need to do to allow users to add and remove components from a placeholder using the Experience Editor?

**A:** Create a Placeholder setting item for that placeholder.