# Sitecore Omni
- is a headless CMS architecture that includes the easy editing ability found in a traditional CMS but uniquely offers personalization on any device or application.

### Sitecore Omni Products
<table>
	<thead>
		<tr>
			<th colspan="5">Omni Products</th>
		</tr>
		<tr>
			<th>GraphQL</th>
			<th>Sitecore Services</th>
			<th>Sitecore Xperience Accelerator</th>
			<th>Sitecore Universal Tracker</th>
			<th>Sitecore JSS</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Query Language,<br> Returns query</td>
			<td>SXA Offers services to access <br>standard editing content</td>
			<td>Delivers personalized <br>decoupled content as json</td>
			<td>Scalable tracking service API</td>
			<td>Seamless omnichanel</td>
		</tr>
	</tbody>
</table>


Code-First Workflow:
- Develope preferred OS separated from Sitecore

Ease of Use:
- JSS SDK provides easy web deployment in self contained bundle

Application Integration:
- JSS Generates the necessary artifacts for Sitecore

Application Scalability:
- You can use CDN's Proxies and Nodejs services to scale your application.

Cross Platform Support:
- SDK support to deploy your app seamlessly on any platform that runs js server-side

Headless Server Side Rendering:
- Supports hosting nodejs applications for headless rendering

### Sitecore JSS Capabilities
<table>
	<thead>
		<tr>
			<th colspan="4">Sitecore JSS Features</th>
		</tr>
		<tr>
			<th>JSS Library</th>
			<th>Sitecore Layout Service</th>
			<th>Javascript View Engine</th>
			<th>Application Import</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>NPM Packages</td>
			<td>Composition Pages for each component <br>Emulates data</td>
			<td>Allows Server-Side Rendering</td>
			<td>Code-First Approach</td>
		</tr>
	</tbody>
</table>

### Code First Approach
**Designing with Code-First Workflow**
Code-First Approach When:
- Prototyping
- No instance of Sitecore
- Non-win OS
- JS are Primarily Developers
- Simple app from Content Perspective
- External Developers

Code-First Benefits:
- Deploy cross-platform apps
- Decoupled from Sitecore
- Work with JSS SDK without Sitecore Backend

**Implementing UX Design Strategies**
- Allows you to work with UX Designers to ensure required collaboration between developers and designers.

**Considering UX Designer Role**
- UX Designers provides JS Developers UX designers might provide JavaScript developers with an integrated or separate code approach for less complex sites or simple redesigns.

**Designing with No Limitations**
- JSS allows no limitations to UX Designers
---
# Identify JSS Requirements
**Explore JSS CLI**
- JSS CLI is a nodejs command-line tool with development scripts, it allows you to:
	- Create, Maintain and Run JS Applications
	- Scaffold Components
	- Deploy apps to Sitecore

**CLI Scripts**
| Command | Description |
|:---:|---|
| `npm` | Node Package Manager |
| `install` | Install Command |
| `-g` | Flag enables the jss command to run from any directory |
| `@sitecore-jss/sitecore-jss-cli ` | Package name of the JSS CLI |

e.g. install JSS-CLI using Yarn
```sh
$ npm install -g @sitecore-jss/sitecore-jss-cli
```

to verify successful installation
```sh
$ jss --help
```
---
## Create JSS Application
`app-name` -> JSS Application Name
`app-template-name` -> Angular, Vue, React, etc.
```sh
$ jss create <app-name> <app-template-name>
```
E.g. Create a JSS `my-first-app` in `vue`
```sh
$ jss create my-first-app vue

$ cd my-first-app

$ jss start
```
---
Which of the following statements best describes why you install the JSS-CLI ?
- To create, maintain and run JS applications
- To Scaffold Components
- To Deploy apps to Sitecore




