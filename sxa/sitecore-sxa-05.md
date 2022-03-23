# Search SXA
### Benefits of Search in `SXA`
---
1. You can use standard components to create your search interfaces.
2. You don't required any custom code; all you need is configuration to get started.
3. You can quickly configure `geospatial-search`, `scoping`, `paging`, `sorting`, `lazy loading`, and more.
4. You can use the search service to power custom components.

### Facets
---
Use to refine search results by categorizing the items returned by the search. For example, if you build a search page <br>for a blog, all blogs will contain fields such as author, date, and language. Based on these fields, you can create facets <br>to allow visitors to use them as filters.

| Facets | Component |
| --- | --- |
| `Date` | **Filter (**_Date_**)** |
| `Distance` | **Filter (**_Radius_**)**, Location Finder |
| `Float` | **Filter (**_Managed Range_**)**, **Filter (**_Range Slider_**)**, **Filter (**_Slider_**)**  |
| `Integer` | **Filter (**_Managed Range_**)**, **Filter (**_Range Slider_**)**, **Filter (**_Slider_**)**  |
| `List` | **Filter (**_Checklist_**)**, **Filter (**_Dropdown_**)** |

You can add facets to your site within the Content Editor by navigating to: 
```sh
Sitecore/content/Tenant/Site/Settings/Facets/
```

### Scopes
---
Search scopes are used to limit the search results based on conditions. For example, to create a search scope for <br>locating a store on the Lifestyle website, you have to narrow the search scope down to only items located in that<br> specific part of the content tree.

The search scopes are stored in the Settings folder of the respective site, i.e., 
```sh
/sitecore/content/Tenant/Site/Settings/Scopes/
```

### Tokens
---
Tokens are used in search queries to apply additional search filters. SXA comes with predefined tokens that you can <br>quickly use to apply _multiple_ search filters

### Pagination
---
Pagination is the process of splitting the contents of a website, or a section of contents from a website, into discrete <br>pages. In SXA, the Pagination rendering allows you to add pagination to a Page List, Event List, and File List renderings, <br>reflecting the number of pages and enabling you to navigate to a page directly or use additional buttons (First, <br>Previous, Next, Last).

### Search Box Rendering
---
Used on webpages to allow visitors to search your website. By default, the Search Box rendering adds the search text <br>box to the page. As an Administrator, you can create and customize search boxes for campaign pages by adjusting <br>the Search Box rendering properties without the support of a developer.

### Search Results Rendering
---
Enables website visitors to view their search results by adding it to the respective page. Using this rendering, you can support short web campaigns by creating a simple search solution so results appear on the same page.

### Page Selector Rendering
---
Using the Page Selector rendering, you can choose how to display the search results page. The default page size <br>configured in the Search Results rendering determines the number of pages displayed. When using the Page Size <br>rendering, remember to configure the page size in the Control Properties dialog box of the Page Size rendering.

### Q&A
---
**Used to apply multiple filters to configure the scope in search queries?**
- Tokens

**True or false: You will need to create custom components to create search interfaces when building your <br>website with SXA.**
- False

**Which of the following renderings would you use to help visitors view the search results within your website?**
- Search Results Rendering

**True or false: The default page size configured in the Search Results rendering determines the number of <br>pages displayed.**
- True

**Administrators use which of the following in search queries to apply predefined filters in a search solution <br>on a particular webpage?**
- Tokens

**True or false: The default page size configured in the Search Results rendering determines the number of <br>pages displayed when a visitor performs a search function.**
- True

**Which of the following are used by visitors to reduce the number of results to only those that will satisfy the <br>user search criteria?**
- Facets

**The Search Results signature can be used to limit results by filtering them based on a unique _________ for <br>specific search results.**
- Signature