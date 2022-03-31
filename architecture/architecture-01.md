# Sitecore Architecture
### Review
---
Sitecore's three major products are:
: - Sitecore Experience Editor (XE)
  - Sitecore Experience Manager (XM)
  - Sitecore Experience Commerce (XP)

Roles Group by Product
: - They are licensed and installed and in which they are primarily used.

Roles Group by Type
: - Where roles are grouped by their usage or technology.

Role Group by Combination
: - For Scalability and Simplicity reasons, some logical roles can be combined to form a single running entities in a topology

Content Delivery (CD)
: - Handles requests from visitors across channels, determines which content to serve, and renders output in the relevant format for the channel.

Content Management (CM)
: - Enables Content Authors to create, manage, and publish content.

Sitecore's Collection and analysis of experience data
: - Experience Database (xDB)
    - Collection of services and storage roles that store and process experience data
  - xContent
    - Set of services that sits between xDB and any trusted client, device or interface that wants to collect and search experience data over HTTPS.

What is a Topology?
: - Web Deploy Packages (WDPs), which will be zip files that contain everything you need to set up a role or role combination (e.g., application or worker root)
  - Configuration Files (or Azure Resource Manager templates in Azure) for each role or resource that define parameters used during installation.

Data Exchange Framework
: - enables synchronize data to and from sitecore or any other db in the system. (Highly customizable, typically defined by Developers and Administrators)

Private Session State Store
: - for active visitors, includes metadata and active visits for personalization. (Hosted in SQL Server, Redis, Azure SQL, or Azure Redis)

Shared Session State Store
: - storage of information about the current contact state and related data, including all data unique to a contact that can be shared across multiple sessions.

Device Detection
: - SaaS Cloud service that provides continuously updated information and hardware and is based on User Agent string. It has no requirements regarding solution infrastructure.

IP Geolocation
: - web service that looks up the approximate geographic location of an OP address. The services does not handle or store personal data.

Content Publishing
: - publishes content from the Master Database to Web database and is an optional replacement for he Sitecore publishing method that are part of the  Content Management role.
  - Content Publishing as a web application, it can be scaled.