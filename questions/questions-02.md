1- _What mode in experience Editor Shows profile, cache settings and HTML output for Individual Components?_
- `Debug Mode`

2- _What are the options to source control your items?_
- You can serialize your items for source control with `Sitecore Rocks` or use a product like `TDS` to do it.

3- _What are workflows used for?_
- Content Approval
- Versioning
- Tracking

4- _How does Sitecore store visitor Data?_
- Data is collected in a `MongoDB` collection database
- That information is aggregated and stored in a SQL Server database optimized for reporting

5- _What can be tested with Sitecore Testing?_
- Content
- Components
- or Entire Page

6- _Where can you download the latest version of Sitecore?_
- `dev.sitecore.net`

7- _Why do we set icons on our templates?_
- To make easier to find for Authors

8- _How can you change the configuration files load order?_
- Using `<loadOrder>`

9- _What setting determines whether or not an item can be viewed in the browser?_
- Presentation Details

10- _What do you need to create to enable **Dynamic Binding**?_
- a Placeholder

11- _What property **automatically propmts a user to choose a data-source** when adding a component in the **Experience Editor**?_
- Data-source Location

12- _What would you not use `Axes.GetAncestors()` when retrieving items?_
- Poor performance when retrieving a large number of items

13- _**Poor Performance** when retrieving a large number of items_
- if the changes only exist on the **Web Database** they will be lost during the next publish operation.

14- _What happens when an items inside a bucket is not **bucketable**?_
- The item is not hidden, it appears as a normal child item.

15- _How can you make it easier to communicate issues with **Sitecore Support**?_
- Use the **Support Package Generator**

16- _Name three **Sitecore Interfaces**?_
- Desktop
- Content Editor
- Experience Editor

17- _Which **Experience Editor** would you use to add an image or edit text?_
- Editing mode

18- _The Content Editor in Experience Editor - Designing Mode **can't select header**. Why is this?_
- It is included statically. There is no placeholder

19- _What are the two types of default field values?_
- Dynamic (uses tokens) and Static

20- _What are presentation details?_
- Configuration that determines what an item looks like when requested by the browser

21- _How many Layouts can you assign to a single item?_
- one per Device

22- _What is the **Sitecore Control** that allows you to **dynamically bind** components to a page?_
- `sc:Placeholder`

23- _How can Sitecore help you resize images dynamically?_
- Set `MaxWidth` *and/or* `MaxHeight` on the `sc:Image` tag

24- _When you are looking at a page in Experience Editor mode, what is the **context database**?_
- **Master**

25- _Why should you not use `GetDynamicUrl()` for your site's frontend?_
- Unreadable 'developer' URL, uses IDS

26- _What permissions does **extranet\anonymous lack** by default?_
- Permission to create or edit items

27- _Why should you use `FieldRenderer.Render()`?_
- Transforms field content into valid `HTML`
- Automatically makes fields editable in **Experience Editor**
- Allows you to pass in parameters that match the one available in **Sitecore controls** - For Example: `image max width`
- Translates dynamic links in **Rich Text Editor** fields into **_SEO-friendly_** Url's

28- _How are **parameters encoded** when sent to your component?_
- as a URL query string, that is: `key1=value1&key2=value2`

29- _How does the **XML of a layout delta** differ from the **XML specified on a templates standard values**?_
- Layout Deltas only contain differences between an items standard values presentation and any changes made by the author on the item.
- The standard value XML contains all presentation details.

30- _When will Sitecore use the language attribute of the site definition in the `web.config`?_
- if there is no explicit language specified in the URL nor a language cookie

31- _Which item versions can have **individual presentations** defined on them?_
- Numbered and language versions of an item.

32- _How does Sitecore support each of the CMS pillars? (data-definition, content, presentation)_
- Data definition: _**data templates**_
- Content: _**items**_
- Presentation: _**layouts and components**_

33- _Why should you avoid defining the same field multiple times in more than one template?_
- It makes it much harder to manage later on

34- _Why would you need to run a **full-republish**?_
- Theoretically, you should not need to do this as a user

35- _What do you need to do to allow users to **add and remove components** from a placeholder using the **Experience Editor**_
- Create a **Placeholder Settings** item for that placeholder

36- _What do you need in addition to the Experience Management to take full advantage of the Sitecore Experience Platform?_
- You need the **Experience Database** to take full advantage of the available features. It supports **_Analytics_** and **_Marketing_** features.

37- _When you set up multiple site structures in the content tree, what is the recommended practice for handling content that will be shared between sites?_
- Keep it outside of any site structure.

38- _To provide a rich user experience, what are some recommended practices you should use when you create templates?_
- Provide default values, use user friendly names and icons, limit the use of **Rich Text Editors**

39- _Which type of component would you create if you wanted to **closely follow MVC patterns** or invoke complex logic?_
- Controller Rendering

40- _What data template must be used as a **base template for your Parameters**?_
- The **Standard Rendering Parameters Template**

41- _You have a component that you want **cached on every Event Details Page**. Where would you define its cache settings?_
- On the component on the **Event Details Template Standard Values item**

42- _Why is it important to have **friendly folder structures** within your content tree?_
- Because they dictate the segments that are within your URL

43- _What Class would you us to retrieve the content of a **Tree list field**?_
- `Sitecore.Data.Fields.MultilistField`

44- _How would you **show a toolbar** in a random part of the page?_
- Using an `Edit Frame`

45- _What methods do you invoke when you begin and finish editing an item through the **API**?_
- `.Editing.BeginEdit()`
- `.Editing.EndEdit()`

46- _What does the **Datasource Location** field automatically do in the Experience Editor?_
- Opens the Select the Associated Content dialog when authors add a new component

47- _Once Custom Experience buttons are assigned, where do they show up?_
- On a component/field and displayed in the **Experience Editor**

48- _How do you **create a bucket**?_
- Select the item you want to turn into a bucket and click the `Bucket` command on the `Configure` tab

49- _What method should you use to return rich results object?_
- `GetResults()`

50- _What are the three layers that the item cache mechanism have?_
- Item
- Data
- Prefetch

