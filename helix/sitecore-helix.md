<style>
.principles-table thead { background-color: rgb(28, 166, 163); }
</style>
### Sitecore Notes
-----
**Sitecore Helix** is based on *modular architecture* or *package design*.
*by [Robert C. Martin](http://staff.cs.utu.fi/~jounsmed/doos_06/material/DesignPrinciplesAndPatterns.pdf)*

#### Sympthoms of Rotting Design
- **Rigidity - Inflexibility**
	- Software becomes difficult to change
* **Fragility**
	- Sofware tends to break in many places every time it is updated
* **Inmobility**
	- Software modules are too dependent on other modules and its rewritten instead of being reused
* **Viscosity**
	- Software become to hacky and looses its design or environment
* **Changing Requirements**
	- Changing the requirements tends to be more prone to change the initial design bit by bit as changes continues, the malignancy sets in.
* **Dependency Management**
	- lack of dependency management causes the software to degrade and becomes Rigid, Fragile, Inmovable and Viscous
----

## Principles of Object Oriented Design
### The Open Closed Principle (OCP)
_A module should be open for extension but closed for modification_
The ability of changing what the module does without changing the source code. **Abstraction is the key to the OCP**

### Dynamic Polymorphism
The separation of dependency and interfaces.

### Static Polymorphism
The use of Templates or Generics.

### Liskov Substitution Principle (LSP)
_A module should be substitutable for its subclasses_
Derived classes should be substitutable for their base classes

### Dependency Inversion Principle (DIP)
_High level modules should not depend on low level modules_
Dependency Inversion is the strategy of depending upon **interfaces** or **abstract functions and classes**, rather than upon concrete functions and classes

### Depending upon Abstractions
_Every dependency in the design should target an **interface**, or an **abstract class**. No dependency should target a concrete class._

### The Interface Segregation Principle (ISP)
_Separate the interface from the implementation._
If you have a class that has several clients, rather than loading the class with all the methods that the clients need, create specific interfaces for each client and multiply inherit them into the class

### The Relase/Resuse Equivalence Principle (REP)
_The granule of reuse is the granule of release_
A reusable element, be it a component, a class, or a cluster of classes, cannot be reused unless it is managed by a release system of some kind

### Common Closed Principle (CCP)
_Classes that change together, belong together_
The ability to group classes that change together to minimized the From-To Relase impact.

### Common Reshuse Principle (CRP)
_Classes that aren't reused together should not be grouped together_

### Stable Abstractions Principle (SAP)
_Abstractions should be stable_
_Stable Packages should be Abstract Packages_
Code Should depend in the direction of stability.

----
<div class="principles-table">

| Principles of Package Design for Package Cohesion 	| Principles of Package Design for Package Coupling |
| -----------------------------------------------	 	| ------------------------------------------------ |
| What goes into a package and what stays out.			| how Packages (in Helix) should interact with each other |
| Questions in relation to Package Cohesion 			| Questions in relation of Package Coupling 		|
| - What defines a module? <br>- how do you make modules manageable? | - How do the modules connect? <br>- How do you control the depencies of your solution? |
</div>


### Guide: Principles of Package Design for Package Cohesion
**The Reuse-Release Equivalence Principle**
- All classes in reusable module should be reusable by the same audience
- You should consider the content of a module from the point of view of potential consumers.

**The Common Reuse Principle**
- Classes that are tightly bound to each other with class relationships should be in the same module.
- This principle tells which classes should not be put together in the same module; classes that are not tightly bound to each other should not be in the same component.

**The Common Closure Principle**
- A change that affects a module affects all the classes in that module and no other module
- This principle is the Single-Responsibility Principle stated for modules; i.e., a module should only have one reason to change.

### Guide: Principles of Package Design for Package Coupling
**The Acyclic Dependencies Principle**
- Allow no cycles in the module dependency graph.
- There should be no circular dependencies between modules.
- You should continuously ensure no circular dependencies appear as the module dependency graph grows.

**The Stable Dependencies Principle**
- Code should depend in the direction of stability.
- Modules are created that are sensitive to certain kinds of change.
- Any module that is volatile should not be depended on by a module that is difficult to change.

**The Stable Abstractions Principle**
- A module should be as abstract as it is stable.
- A stable module should be abstract so its stability does not prevent it from being extended
- An unstable module should be concrete since its instability allows the concrete code inside to be easily changed.

## Summary
Sitecore Helix based on Principles of Package Design by Robert C. Martin. Following guidelines laid out in Helix to protect the long-term value of your product solution and quicker deployment timelines.
|||
|---|---|
| Principles of Package Design for Package Cohesion | Address what goes into a package and what stays out |
| Principles of Package Design for Package Coupling | Address how packages (i.e., modules in Helix) should interact with one another. |
| Common-Closure Principle | The Classes in a module should be closed together against the same kinds of changes. |
| Acyclic Dependencies Principle | No circular dependencies between modules. |


**Where do we see the Principles of Package design show up in Sitecore Helix?**
A Sitecore solution based on the Helix principles will typically have its modules laid out in three layers: Foundation, Feature, and Project. Dependencies between modules in these layers flow in only one direction.

---
## Helix Terminology

**Depency**
- A dependency is a relationship between two modules.

**Implementation**
- An _"Implementation/Customper Implementation"_ is the total number of modules, features, and functionalities deployed to solve customer's business problem.

**Module**
- A Module is a conceptual grouping of assets that relates to particular business requirement. A way to group all assets, vusiness logic and configuration, into a single unit.

**Solution**
- Refers to _"Visual Studio Solution"_. also referred to as _"Implementation"_.

**Stability**
- Refers to _"Principles of Package Design"_. You determine the stability of a module by the number of its incoming and outgoing dependencies.
_The more external dependencies a module has, the more stable it must be **(Stable-Dependencies Principle)**_


|||
|---|---|
| Dependency | Describes how a feature and functionality in the solution relate to each other |
| Implementation | Total number of modules, features, and functionalities developed and deployed |
| Module | Conceptual grouping of assets that relates to a particular  business requirement |
| Solution | Visual Studio Solution or an Implementation |
---
