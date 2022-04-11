# Sitecore Certificate Exam 9.0
## Helix
---
What are the Principles of Package Design for Package Cohesion?
: - What goes into a package and what stays out.
  - Questions in relation to Package Cohesion
  - What defines a module?
  - How do you make modules manageable?

What are the Principles of Package Design for Package Coupling?
: - How do the modules connect?
  - How do you control the dependencies of your solution?
  - Questions in relation of Package Coupling

The Re-Use Release Equivalence Principle?
: - All classes in reusable module should be reusable by the same audience
  - You should consider the content of a module from the point of view of potential consumers.

The Common Reuse Principle?
: - Classes that are tightly bound to each other with class relationships should be in the same module.
  - This principle tells which classes should not be put together in the same module; classes that are not tightly bound to each other should not be in the same component.

The Common Closure Principle?
: - A change that affects a module affects all the classes in that module and no other module
  - This principle is the Single-Responsibility Principle stated for modules; i.e., a module should only have one reason to change.

The Acyclic Dependencies Principle
: - Allow no cycles in the module dependency graph.
  - There should be no circular dependencies between modules.
  - You should continuously ensure no circular dependencies appear as the module dependency graph grows.

The Stable Abstractions Principle
: - A module should be as abstract as it is stable.
  - A stable module should be abstract so its stability does not prevent it from being extended
  - An unstable module should be concrete since its instability allows the concrete code inside to be easily changed.

Where do we see the Principles of Package design show up in Sitecore Helix?
: A Sitecore solution based on the Helix principles will typically have its modules laid out in three layers: _**Foundation**_, _**Feature**_, and _**Project**_. Dependencies between modules in these layers flow in only one direction.

#### Helix Terminology
Dependency
: - A dependency is a relationship between two modules.

Implementation
: - An _"Implementation/Customer Implementation"_ is the total number of modules, features, and functionalities deployed to solve customer's business problem.

Module
: - A Module is a conceptual grouping of assets that relates to particular business requirement. A way to group all assets, business logic and configuration, into a single unit.

Solution
: - Refers to _"Visual Studio Solution"_. also referred to as _"Implementation"_.

Stability
: - Refers to _"Principles of Package Design"_. You determine the stability of a module by the number of its incoming and outgoing dependencies.
_The more external dependencies a module has, the more stable it must be **(Stable-Dependencies Principle)**_

| Term | Description |
|---|---|
| Dependency | Describes how a feature and functionality in the solution relate to each other |
| Implementation | Total number of modules, features, and functionalities developed and deployed |
| Module | Conceptual grouping of assets that relates to a particular  business requirement |
| Solution | Visual Studio Solution or an Implementation |

The statement that best differentiates Sitecore Helix from Helix Examples
: - Sitecore Helix specifies recommended conventions for Sitecore development, while Helix Basic Company <br>is an example of an implementation following Helix practices.

For Solution architects, which of the following are the problems caused by a highly- coupled implementation?
: - Making changes is very expensive.
  - Reusability becomes infeasible.
  - Managing dependencies becomes impossible.

True or False: Sitecore Helix is the same as Atomic Design.
: - False

Which of the following are considered the basic building blocks in Helix?
: - Modules

For Sitecore Developers, what is the primary focus of Sitecore Helix?
: - Controlling dependencies

Which of the following is the prime focus of the Principles of Package Coupling in Sitecore Helix?
: - Stability

True or False: The primary focus of a module in Sitecore Helix is implementing business objectives and <br>grouping together multiple technology building blocks that refer to each objective.
: - False

Which of the following is the most stable layer in Sitecore Helix architecture?
: - Foundation Layer

Select the statements that best explain the value of layer conventions in Sitecore Helix.
: - Provide a common solution architecture for Sitecore implementations
  - Encourage stable dependencies
  - Help visualize the dependencies in a solution

Which of the following principles helps us set boundaries between features?
: - Principles of Package Cohesion

Select all the statements that are true for identifying modules.
: - The objects in a module should be closed together against the same kinds of changes.
  - Identifying modules is all about identifying responsibilities.

folder that should not be placed at the root level of the solution
: - Templates

Which of the following is correct regarding the Visual Studio (VS) implementation of a Sitecore project on <br>Helix?
: - All Visual Studio projects belonging to a logical module should be managed together in one VS solution.
  - One VS solution can represent an entire Sitecore implementation.
  - A Sitecore implementation can span multiple VS solutions.

A project and assembly should be named in a namespace-like fashion with the:
: - Module name

Which of the following is the correct representation of the content tree structure to store templates?
: - `/Sitecore/templates `
  - `/Sitecore/templates/Feature/module/`

Which template type can you assign a page layout to?
: - Page Type template

Which of the following item types is not typically a developer-owned definition Item?
: - Page Item

Select the option that shows the correct path of the serialization folder in the file system.
: - `/src/Foundation/Module/serialization`

Which of the following is typically controlled by layouts and renderings to contain project-specific markups?
: - Overall page design

Which of the following modules do controller or view renderings typically belong to since they are connected <br>to business features in the solution?
: - Component Module

According to Helix semantics, you can typically manage which of the following as a part of the content in Sitecore?
: - Settings

Select all the statements that are applicable for naming view files and rendering items in Sitecore to ensure discoverability and simplicity.
: - Align the rendering item name with the cshtml file name.
  - Naming of view files and the rendering items should be aligned as much as possible.
  - Set your display names to support languages.
  - Always favor editors over Developers, so avoid CamelCase and never use DevAbbrevInNames.

When working with Sitecore Experience Commerce, how should you structure Visual Studio projects for features that contain shared functionality for your website, unit testing, and the Commerce Engine?
: - The website, unit testing, and commerce Visual Studio projects should be placed in one Feature module based on their common and coherent focus.

## JSS
---
Why do you install the JSS-CLI?
: - To create, maintain and run JS applications
  - To Scaffold Components
  - To Deploy apps to Sitecore

How route items and the database are defined after JSS setup 1completes?
: JSS setup creates a `./config` file that generates the site definition.

When to Mock data?
: Mock Data by copying files, image fields, and other items into the file system

When to Re-Use Content?
: Reuse content when you need to use the same content in multiple locations such as `Headers` and `Footers` can be reused across multiple pages.

When to `Work Disconnected`?
: Work disconnected from **Sitecore** to create components and mock route data.
  - When the app runs, it does not have the data from **Sitecore** using `HTTP` data calls.
  - You're using a local `datasource` for your content, route (layout), and component registrations.

How Route Provides Mock Data?
: The data is acquired from the local `datasource` and runs on a local development server.

Using Styleguide Data Types...
: Helps mock data.

Route-Level Fields Data...
: Mocks route-level fields by simply adding `fields` property to your route data.

## SXA
---
What is SXA?
: Sitecore Experience Accelerator provides reusable, templated UX layouts and components.

## TDS
---
What is TDS?
: Team Development for Sitecore

When building a solution, hwy might you utilize Team Development for Sitecore (TDS)?
: To serialize your Sitecore items

When inputting your TDS License key during TDS installation, the Company Name and License are Case sensitive?
: True

Why you should configure TDS Global config file?
: To ensure settings you want configured across all projects are applied to all projects.

As a Developer, why is it important to implement unit testing?
: Unit testing allows you to refactor with confidence, and checks your code behaves as you intended.

Why should you utilize Attach to Process in Visual Studio when working with Sitecore?
: To ensure you are attaching to your Sitecore site.

When using TDS for Serialization, it is recommended that you pull all Sitecore items into your project.
: False

---
## General
What is the name of Component Architecture guideline of Sitecore?
: Helix

What is Horizontal scaling and Vertical Scaling?
: - Vertical Scaling
    - Add Resources to a single node in a system.
  - Horizontal Scaling
    - Adds more nodes to a system
  
Which databases is required for CD Server?
: Web and Core

What can be the reason `$token` is visible in one of the items as "`$token`" and not replace it with its value?
: `$token` will replace by value for new items, not the old ones.

Which `DLL` is required to get `RenderingContext`?
: `Sitecore.MVC.Dll`

What is the difference between `Shared` and `Final Layouts`?
: - `Shared Layout`
    - Controls which is added in the shared layout. is shared in all language and numbered versions
  - `Final Layouts`
    - Changes which is made in final layout are specific to the language and version.

Which tag use in `Layers.config` file to define the sequence of execution of config files?
: `<loadOrder>`

How to force the content editor to create similar kind items under article?
: Insert Option

Which roles access right will take precedence?
: `Deny`

What is a difference between Smart, Republish and Incremental Publish?
: - Incremental Publish
    - Publishes only items that are in the publishing queue.
  - Smart Publish
    - Publishes all items that have changed since the last publication.
  - Republish
    - Publishes everything.

What this code do `Sitecore.Globalization.Translate.Text("Title")`?
: Gets phrase of dictionary key "Title"

What is the difference `GetChildren()` vs `GetDescendants()`?
: - `GetChildren()`
    - Returns all direct children of an item
  - `GetDescendants()`
    - Returns all the items under an item

What is a difference between `Treelist` and `TreelistEx`?
: - `Treelist`
    - always loads
  - `TreelistEx`
    - loads on demand

Why we set icons in Sitecore?
: To uniquely and easily identify the item

**_What are the different tokens supported by Sitecore?_**: 
| Token | Description |
| :---: | --- |
| `$name` | the name for the new item entered by the user |
| `$id` | the ID of the new item |
| `$parentid` | the ID of the parent of the new item |
| `$parentname` | the name of the parent of the new item |
| `$date` | the system date in `yyyymmdd` format |
| `$time` | the system time in `HHmmss` format |
| `$now` | the system date and time in `yyyyMMddTHHmmss` format |

What are the different types of Databases available in Sitecore?
: Master, Core, Web

Which editor is mainly designed for no technical Content Editor
: Sitecore Experience Editor

How to get data from xDB?
: `xConnect`

What is the us of Standard Template?
: To store data that is hidden and use ofr an internal purpose

What is hte use of the Core Database?
: Environment settings and Membership details

Why Sitecore have Master and Web Database?
: Changes in Master database in sandbox mode didn't affect LIVE website mode

You have used `GroupBy` clause to get a result from the index, but you didn't get anything, why?
: `GroupBy` clause is not supported by Sitecore search API

**_Match the pair_**
: - Sitecore products and modules download after 8.0 **->**  Sitecore developer Portal
  - Sitecore videos **->**  Sitecore Youtube Channel
  - Sitecore Products and modules download before 8.0 **->**  Sitecore Developer Network
  - Raise tickets for issues **->**  support.sitecore.net

Which field is editable inline in Experience Editor
: Datetime

How you find items in buckets?
: Content Search API

How to edit `Treelist` in Experience Editor?
: Use edit frame and add buttons in toolbar

How to do specify static component in cshtml file?
: `@HTML.Sitecore().Renderings("Path or ID")`

What is the use of Sitecore Packages?
: to create `Zip` files that contain items and code files and to install it on some another Sitecore Instance

You have `Title` field in Event template and `Title` field in Article Template. What you will do to follow the recommended approach?
: Create a base template and inherit on both.

How does Sitecore knows you are a returning customer?
: by calling `Identify()` method
