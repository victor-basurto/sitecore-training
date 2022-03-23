# Multitenancy with `SXA`
- Tenant [^1]
    - Independent group of sites. [^2]
    - Often represents a brand and can include any number of related websites.
    - Typically a tenant is the equivalent of a business unit.

- Module [^3]
    - Isolation of Features and Functionality

## Overview of modules in the Create a tenant wizard
| Module Name | Functionality |
| :---: | --- |
| Composites | Renderings such as `Accordions`, `Carousel`, `Snippets`, `Flip` and `Tabs` to create complex elements on the page. |
| Error Handling | Allows you to specify pages that will be shown to the user when a page is not found or a server experiences a problem. |
| `JSON` | Enables `SXA` pages to be consumed by mobile apps and devices by exposing them in a more machine-friendly `JSON` format. |
| Navigation | Contains components that allow your visitors to navigate the site using concepts such as navigation, `breadcrumb`, and `links/buttons`. |
| Redirects | Allows you to define redirect rules to create vanity `URLs` and keep `URLs` that drive traffic to your website, ensuring that your website has the best possible `SEO` rating. |
| Search | Enables you to use Sitecore content search with rich filtering and presentation, including `geospatial search`, `paging`, `infinite loader`, and any `sorting` that you may need. |
| Security | Allows Admins to secure the website in a `multi-role` scenario where you have users of various proficiency and responsibility. |
| Page Content | Enables _Content Editors_ to easily access fields on the page, along with `Rich Text`, `Plain`, and `HTML`. |
| Page Structure | It consists of renderings such as `containers`, `dividers`, `splitters`, `toggles`, and more, all of which support page structuring. |
| Creative Exchange | Allows your front-end developers to import and export their theme styling easily. |
| Local Data Sources | Provides locations for storing the content placed onto a page in a local folder, just underneath the page. |
| SiteMetadata | Provides metadata important for `SEO`, Sitemap, and social media, thus giving you the flexibility to have custom metadata. |
| Maps | Embeds maps from Google or Bing with locations, routes, and areas that you can mark. The component can also display **POI** results when associated with a search results source. |
| Sticky Notes | Allows your editors to collaborate more effectively through notes that you can attach to the components in Experience Editor. |
| Taxonomy | Provides tagging capabilities to your web content, enabling rich `SEO` and search scenarios. |
| Forms | Enables the functionality of dragging and dropping Sitecore Forms on your `SXA` pages. |

---

**You are a multinational company, and you need sites separated by language for a particular brand. What would you use to structure your web solution?**
- Site
- Tenant

**True or false: A site is a collection of content and output with a common overall business objective sharing a common set of assets.**
- True



[^1]: a single brand can host numerous websites based on geographic region - Solution: Include Multiple Tenants
[^2]: a single brand can support localized markets via one-to-one translated versions,  i.e., one tenant can have multiple sites grouped into their respective site folders for supporting local markets using native Sitecore language support.
[^3]: Use the Helix module and layer conventions to structure your tenants and sites

