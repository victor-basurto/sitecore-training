1- _What are the benefits of `dynamic-binding`?_
- New page types can be assembled from existing components
- changes to page structure do not require a developer
- supports content re-use
- supports **Sitecores Personalization** and testing

2- _why should you never cache a component that displays personal information?_
- another visitor to your site can see that information

3- _what is the name of the feature tht makes **WCM** possible in Sitecore?_
- Experience Management (xManagement)

4- _True or False: The view should contain all the business logic_.
- False

5- _In what order are these configuration files processed by default?_
- Alphabetically by file name

6- _Name 2 devices you may want to target with different presentation details?_
- Tablets and Mobiles

7- _Name some features of Sitecore Instance Manager (SIM)_
- Packages, customize, extend, reinstall & remove instances.

8- _What happens when you set a field as shared? and un-versioned?_
- A shared filed contains a **single version** of the data for **all versions in all languages**.
- An un-versioned field contains onver version of the data per language.

9- _What to do to make sure your author can use the testing functionality?_
- add `Launch Create Test Dialog` to workflow
- make sure the Experience Editor works and is configured correctly.
- Ensure components that should be tested are configured to accept data sources.

10- _What does the presence of the **__Final Rendering** field allows an author to do?_
- To define individual presentation details for each version of an item.

11- _You have just created new content but you cannot see it on your live website, why not?_
- you need to publish new or edited content

12- _What type of components might be good **candidates for static binding**?_
- page scaffolding, like headers and footers.

13- _What method do you use to retrieve item's URL?_
- `LinkManager.GetItemUrl()`

14- _What type of settings can be applied to standard values?_
- Default field values
- Default insert options
- Default presentation
- Default Workflow

15- _In which situations would you want to change the Links that are generated for an individual link?_
- if you need to force the language of content that is to be rendered from Sitecore

16- _Name 4 Properties that you might get from `Sitecore.Context`_
- Context User
- language
- database
- item

17- _How would you enable the use of a **Field Editor**?_
- By adding a **Field Editor** Button to a toolbar

18- _What tool will show you all contacts that have been to your site?_
- Experience Profile

19- _When does a **layout delta** get created?_
- when presentation coming from the standard values of an items templates is overridden on that item

20- _Which field types are suitable for editing using the `.Value` property?_
- Simple text fields. For example, **Single-Line Text**

21- _Name some of the sites that you can refer to for more information and module downloads_
- **SDN, Knowledge Base, Marketplace, Sitecore XP 9 documents**

22- _How can you restrict authors to specific types of item for a components data source?_
- add the data template to the components data-source template field.

23- _How does Sitecore define type of **Item (data schema)**?_
- Templates

24- _What field type would you use to store **formatted HTML**?_
- **Rich Text Field**

25- _When building your own search result class, how do you account for fields with spaces?_
- Decorate with `[IndexField("Page Heading")]`

26- _List the benefits of participating in the Sitecore Community_
- Complete sample modules can be found on **Sitecore Marketplace**. You can re-use these sample modules in your own projects.
- You can get free 24/7 help from hundreds of community members around the globe, including **Sitecore employees**, **Sitecore Certified Developers and MVPs**.
- While contributing actively to the Sitecore Community, you can become a **Sitecore MVP**. This gives you lots of **Sitecore-related benefits**.

27- _If a component is not in the Allowed Controls list, can it be added into that placeholder through the Experience Editor?_
- No

28- _Name three places where component HTML caching options can be defined_
- Definition Item
- Standard Values
- per instance of the component

29- _Why is it a good idea to avoid using Rich Text Fields as much as possible?_
- one of the benefits of using Sitecore is the separation of content and presentation. The Rich text field is the only exception to this, as it stores HTML content directly. If abused and not configured properly, it may give users the ability to break the design of the site.

30- _You are retrieving a large number of items using `Axes.GetDescendants` What is a better alternative?_
- Use `Sitecore.ContentSearch` API

31- _What do facets allow you to do?_
- Progressively apply filters (based on fields) to narrow down your result set

32- _Why does Sitecore not allow the use of certain characters in an items name?_
- Item names are used to form the URLs. Some characters have a special meaning in a URL.

33- _Before contacting support you should..._
- Refer to help desk best practices

34- _Why is it important to think of you data template creation an inheritance structure from the beginning?_
- Refactoring template inheritance may cause **data loss**

35- _Name three permissions that are applied to access rights_
- Allow, Deny, and Not Specified

36- _What is the difference between a **View Rendering** and **Controller Rendering**?_
- **Controller Rendering** follows the MVC pattern more closely.

37- _What is the recommended practice for setting **Insert Options**?_
- **Insert Options** are set on the **Template Standard Values** item

38- _Why is it a good idea to configure **Insert Options** on standard values?_
- All items using that data template will have the same **Insert Options**

39- _What is an item composed of?_
- Field sections and fields

40- _What happens if you try to reuse a component containing a `non-dynamic` placeholder?_
- Anything added to that placeholder is duplicated

41- _What affects whether or not a piece of code will run?_
- That user's permission

42- _What is the biggest challenge when you post forms with Sitecore MVC?_
- Having multiple controllers invoked in the same page request. Only one of the should handle the post.

43- _What do parameters allow you to do?_
- Allow properties to be set per instance of a component

44- _How do you configure an items presentation details in Sitecore Rocks?_
- `Right-click -> Tasks -> Design Layout` or `CTRL + U`

45- _What type of objects does the `GetChildren()` method return?_
- `Sitecore.Collections.ChildList`

46- _How would you render a **Multi-list** field?_
- By retrieving its value in code and using it to create some output.

47- _Unless you are doing a very simple query on a very limited area of your Sitecore tree, what should you use instead?_
- Sitecore Search

48- _What are some of the features of Sitecore Rocks?_
- Integration with Visual Studio
- Creating and editing items
- management tools
- viewing website file system

49- _Which **Experience Editor Mode** would you use to add a new component?_
- Designing Mode

50- _Why should you tune your index configuration and not index everything by default?_
- The index can grow too large with time
