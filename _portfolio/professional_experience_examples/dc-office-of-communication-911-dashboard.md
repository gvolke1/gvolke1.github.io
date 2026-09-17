---
layout: "archive"
title: "DC Office of Unified Communications 911 Dashboard"
permalink: "/portfolio/professional_experience_examples/dc-office-of-communication-911-dashboard/"
author_profile: true
excerpt: "Integrated dispatch and vehicle telemetry feeds into PostGIS, adding quality checks, SQL views, and reporting for operational monitoring."
project_employer: "New Light Technologies"
skills: ["Data Engineering and API Integration", "Databases and Data Quality", "Web Development", "Application Prototyping, Dashboards and Business Intelligence", "Automation and Workflow Improvement", "Emergency Management and Public Safety Analytics"]
---

**Organization:** New Light Technologies  
**My role:** Application development, API integration, SQL,  and project coordination

I supported development of a dashboard for the DC Office of Unified Communications, bringing together information about communications equipment used in emergency operations. My work focused on the application services needed to prepare, store, and deliver data to the dashboard.

I developed a JavaScript and Node.js API that loaded JSON data into memory, saved cached records to a local file, and reloaded those records when the application restarted. I also created synthetic data to support development and testing. This gave the team a consistent set of records to work with while building the dashboard’s interface and data connections.

For database storage, I developed a separate PostgreSQL module and an API endpoint that saved cached records to the database. The table stored JSON data alongside its source and timestamp. I tested the endpoints locally to verify that the application could retrieve cached data and save it to PostgreSQL.

Another part of my work involved preparing information for map display. I wrote code to convert JSON into GeoJSON, worked with router data from the AMM API, and matched data attributes to the frontend’s requirements. I coordinated this work through GitHub and collaborated with the frontend developer to make the data service straightforward to connect to the interface.
