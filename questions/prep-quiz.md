## Prep QUIZ
---

What are the types of publishing?

: Delayed, parallel an dedicated

What is the name of the template all templates should inherit from?
: Standard Template

When would you set languageEmbedding option to never?
: Site is not multilingual

Where should i set insert options as best practice?
: Standard Values

What does an unversioned field contain?
: Data for all version in all languages

Which of the following are reasons for using field types in Sitecore?
: To define the raw value stored in the database, to determine which editor control will be used in the authoring tools, to determine the API field class used in code.

What are the 3 folders in the physical path of the content folder that hosts the Sitecore application?
: Website, data, and database

Which method is not supported by Sitecores implementation of `Iqueryable<T>`?
: `GroupBy`

What does it do when you make an item bucketable?
: the item is hidden

What is Sitecores easy-to-use authoring tool and what functionality does it provide?
: The Experience Editor provides editing and designing functionality.

What is the best way to source control Sitecore items?
: Serializing them

What item setting needs to be specified for authors to be able to add content?
: Insert Options

What is the preferred way to modify the `web.config`?
: Use .config file in `App_Config/Include`

Which interface would an author use to see and edit items in a tree structure?
: Experience Editor

Select the name of the Sitecore component-based architecture guidelines from the list.
: Helix

When you patch in changes to the `Sitecore.config` file, how can you control the order in which your changes are applied?
: In `App_Config/Include`, use a naming convention and sub-folders for config files

Where is the license located?
: Sitecore application root `folder/Data/license.xml`

What do you need to create to enable Dynamic Binding?
: Placeholder

When would you use the DisableWebEdit parameter when rendering a field?
: When rendering a field inside the` <title>` tag in the `<head>` of HTML

What happens if an item version is not in a final workflow state?
: No automatic versioning and version is not publishable.

Publishing synchronizes what between master and web databases?
: Adding new items, updating edited items, removing deleted or unpublishable items.

What happens if a role denies an access right and another one allows it?
: Deny

Where can I check the effective permission of an account?
: Access viewer

What is a Sitecore item?
: The construct Sitecore uses to store data

What part of presentation details applies to all versions of an item?
: Shared Layout

What field type can I use with Rendering Parameters?
: All field types

What should you define in a template?
: Fields, Field Sections, Icons and Base Templates

How do I display the content of a field in code?
: `@Html.Sitecore().Field(<field name>)`

How can I use placeholders inside of placeholders?
: This cannot be done directly.

What does the item Resolver do?
: Maps a URL to an item in the content tree.

Config changes get added alphabetically by default. How can I change it?
: `<loadOrder>`

Select the name of the Sitecore component-based architecture guidelines from the list.
: `/App_Config/Include/c/a.config`

How would you retrieve the URL of an item?
: Use `LinkManager.GetItemUrl()`

Which field type do I use to store formatted html
: Rich text field

How does Sitecore support one of the CMS pillars, Presentation?
: Layouts and components

What parts of the page are typically added using Static Binding?
: Scaffolding, like headers and footers

Why would you use dynamic placeholders
: To reuse a component containing placeholders.

How can I open a bucketable item?
: Use the Sitecore search functionality to locate and open the item.

How can you handle more than one input form on a controller rendering in Sitecore?
: Create an extension method invoking the `FormHandler()` and Use `Ajax.BeginForm()` and specify the controller and action.

Where does Master database publish items to?
: Master database

What are the SIM Import/Export features?
: Export an entire set of Sitecore database with content and import to a new environment.


What happens if the same field name is used in two separate inherited data templates?
: The field will be duplicated.

Where can Presentation Details be set?
: Experience Editor (Design Mode), Content Editor, Template Manager, Sitecore Rocks

What happens when an item inside a bucket is not bucketable?
: Item is not hidden.

What is the CMS parts of Sitecore?
: xManagement

What can I use to translate fields and help texts in the Sitecore client?
: Sitecore Dictionary entries

What tools can I use to install Sitecore?
: Manual or zip file, Scripts, Sitecore Rocks, SIM, EXE

When I made Template bucketable, the existing items are still not hidden. What should I do?
: Sync the existing items.

Which search providers does Sitecore ship with by default?
: Solr and Azure Search

What do you need to do to allow users to add and remove components from a placeholder using the Experience Editor?
: Create a Placeholder setting item for that placeholder.