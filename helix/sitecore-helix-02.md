# Sitecore Helix 02
### Q&A
---
**The statement that best differentiates Sitecore Helix from Helix Examples**
- Sitecore Helix specifies recommended conventions for Sitecore development, while Helix Basic Company <br>is an example of an implementation following Helix practices.

**For Solution architects, which of the following are the problems caused by a highly- coupled implementation?**
- Making changes is very expensive.
- Reusability becomes infeasible.
- Managing dependencies becomes impossible.

**True or False: Sitecore Helix is the same as Atomic Design.**
- False

**Which of the following are considered the basic building blocks in Helix?**
- Modules

**For Sitecore Developers, what is the primary focus of Sitecore Helix?**
- Controlling dependencies

**Which of the following is the prime focus of the Principles of Package Coupling in Sitecore Helix?**
- Stability

**True or False: The primary focus of a module in Sitecore Helix is implementing business objectives and <br>grouping together multiple technology building blocks that refer to each objective.**
- False

**Which of the following is the most stable layer in Sitecore Helix architecture?**
- Foundation Layer

**Select the statements that best explain the value of layer conventions in Sitecore Helix.**
- Provide a common solution architecture for Sitecore implementations
- Encourage stable dependencies
- Help visualize the dependencies in a solution

**Which of the following principles helps us set boundaries between features?**
- Principles of Package Cohesion

**Select all the statements that are true for identifying modules.**
- The objects in a module should be closed together against the same kinds of changes.
- Identifying modules is all about identifying responsibilities.

**folder that should not be placed at the root level of the solution**
- Templates

**Which of the following is correct regarding the Visual Studio (VS) implementation of a Sitecore project on <br>Helix?**
- All Visual Studio projects belonging to a logical module should be managed together in one VS solution.
- One VS solution can represent an entire Sitecore implementation.
- A Sitecore implementation can span multiple VS solutions.

**A project and assembly should be named in a namespace-like fashion with the:**
- Module name

**Which of the following is the correct representation of the content tree structure to store templates?**
- `/Sitecore/templates `
- `/Sitecore/templates/Feature/module/`

**Which template type can you assign a page layout to?**
- Page Type template

**Which of the following item types is not typically a developer-owned definition Item?**
- Page Item

**Select the option that shows the correct path of the serialization folder in the file system.**
- `/src/Foundation/Module/serialization`

**Which of the following is typically controlled by layouts and renderings to contain project-specific markups?**
- Overall page design

**Which of the following modules do controller or view renderings typically belong to since they are connected <br>to business features in the solution?**
- Component Module

**According to Helix semantics, you can typically manage which of the following as a part of the content in Sitecore?**
- Settings

**Select all the statements that are applicable for naming view files and rendering items in Sitecore to ensure discoverability and simplicity.**
- Align the rendering item name with the cshtml file name.
- Naming of view files and the rendering items should be aligned as much as possible.
- Set your display names to support languages.
- Always favor editors over Developers, so avoid CamelCase and never use DevAbbrevInNames.

**When working with Sitecore Experience Commerce, how should you structure Visual Studio projects for features that contain shared functionality for your website, unit testing, and the Commerce Engine?**
- The website, unit testing, and commerce Visual Studio projects should be placed in one Feature module based on their common and coherent focus.