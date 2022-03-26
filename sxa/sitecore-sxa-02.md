# SXA Content Editor, XE, HORIZON
### Content Editor
Designed for more experienced Content Authors.
Content Editor Tool's Interface consist in three main areas:
- **The Ribbon**--the area where all the functionality is available
- **The Content Tree**--the area where all the items are organized.
- **The Content Area**--the area where you can edit your items.

### XE - Experience Editor
**"`WYSIWYG`"** environment designed for Content Authors.
Unlike <u>_Content Editor_</u>, you can see the changes in real-time when working with the Experience Editor.

### HORIZON
Combination of <u>_Content Editor_</u> and <u>_Experience Editor_</u>, **Horizon** has <u>three</u> powerful features that will be particularly useful to _Content Authors_ and other business users
- **The Page Editor**--allows you to create and edit webpages.
- **Simulator More**--allows you to preview webpages as they will appear on different dates and devices.
- **Insights View**--allows you to see analytics for you webpages.

**Which Sitecore editing tool provides you with the following options: The page Editor, Simulator Mode, Insights View?**
- Horizon

**Sitecore Experience Accelerator speeds up the web development process by combining structure and design on a website**
- False


**How would you describe the hierarchical organizational structure of Sitecore's content tree?**
- Parent items can have many child items, but child items can only have one parent item. 

**If you wanted to navigate to a specific page for a site in the content tree, which item would you use?**
- Home

**You're working on a new SXA project, and a colleague who's just joined your team asks you how SXA can help save time for Content Authors and other business users. Which response (or responses) would you give in reply?**
- Sittecore Experience Accelerator includes drag-and-drop toolkit that allows you to move default rendering directly onto the page where you need them.
- Sitecore Experience Accelerator allows you to access rendering parameters without having to navigate through a series of drop-down menus.
- Sitecore Experience Accelerator lets you publish content directly from the editing area without having to go into the publishing directory.

**When reviewing content for a web project, you decide you would like to add an image to an SXA page. What would be your first step?**
- Start by dragging and dropping the image component onto the page from the `SXA` Toolbox.

**If you are navigating through the content tree for you company's site, what are some of the different items you'll want to be familiar with when building content?**
- `Home`
- `Media`
- `Data`

**True or False: The `Media` folder in a site's structure is a shortcut that allows you to preview a scoped view of the media library that is specific to that specific site.**
- True

## Datasource Configuration Options for Snippets
#### Datasource Configuration Options
- Do not copy, use global data source.
    - Default option
    - This setting indicates that the snippet will use a globally assigned data source.
- Copy global data source to local context upon selection.
    - This option allows you to localize the snippet configuration to the page.
- Ask user whether the copy of the data source to local context is desired.
    - With this option, Digital Marketers or any other Content Author can choose how to reuse the snippet.

### Guide to Testing in Sitecore

| Component | Effect | Variants | Content Editor | Experience Editor |
| --- | --- | --- | :---: | :---: |
| Basic Content Test  | Compares Page, Old and New versions | | ✓ | ✓ |
| Component Test  | Component Variants lets you create complex tests | - Test more than two variants of a single component against each other <br> - Test multiple components simultaneously | ✓ | ✓ |
| Page Test  | his form of testing is useful for landing pages | Create only on Experience Optimization | x | x |

### Guide to Personalization with SXA
Personalize at the rendering variant level.
- Using the rules engine you can personalize rendering variants so that the renderings on your site show content specific to a particular group

Personalize Composites
- A composite rendering consists of several other renderings. When a composite rendering is rendered on a page, it queries each item from its data source and pull data and layout.

Centrally manage page and partial design personalization
- The reusability of content and design elements with working with SXA and the ability to use rules when setting page design options provides additional option for personalization.

**Choose the correct answer to fill in the blank: Sitecore automatically uses the data provided by content testing to create ______________________, giving your team options to target the content that is shown on your site to specific visitors.**
- Testing Conditions.

**How does using SXA to personalize your content help speed up the production of your organization's website?**
- SXA allows you to do more with less by providing a central location to manage the personalization of page and partial designs.

**You are working with your team on a Lifestyle website promoting healthy habits. A critical part of your site is a curated set of blog posts written by health and fitness professionals. You want to ensure that all blog posts are styled the same way across your site, but you are unsure which content will be the most effective with visitors. You specifically want to know which of the two variations of the blog post partial design will lead customers to visit a particular product page. What can you do to track and measure how visitors engage with the blog post partial design?**
- Use SXA to run a content test on the blog post partial design across the pages of your website.

**True or false: When personalizing composites, the data source of the composite must point to a data source that is distinct from that of the default rule in the personalization settings.**
- False

**Which of the following best describes how Sitecore manages content testing for your website?**
- Sitecore allows only one active content test per page, and you can only test one partial design included in your page design at a time. 

**You are working on a partial design that will show personalized Recommended Content based on whether a visitor is an authenticated user. How can SXA support you in ensuring that this personalized content is built out across all occurrences of the partial design on your website?**
- With SXA, you can centrally manage the personalization of partial designs, meaning you will only have to set the rules and actions once for it to be leveraged on that partial design across your site.
