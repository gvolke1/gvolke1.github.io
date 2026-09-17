---
layout: "archive"
title: "IMPACT Hazard Data and Population Exposure"
permalink: "/portfolio/professional_experience_examples/impact-incident-management-prioritization-alerting-and-coordination-tool/"
author_profile: true
excerpt: "Built recurring hazard-data workflows and corrected a Census-to-H3 assignment problem affecting population exposure estimates."
project_employer: "New Light Technologies"
skills: ["Data Engineering and API Integration", "Databases and Data Quality", "GIS and Spatial Analysis", "Automation and Workflow Improvement", "Emergency Management and Public Safety Analytics"]
---

**Organization:** New Light Technologies  
**My role:** GIS analyst and data engineering

I helped develop the geospatial data infrastructure for IMPACT, New Light Technologies' emergency-management decision-support platform. My work connected hazard information with population data so emergency managers could examine who might be exposed to a developing natural hazard. It combined recurring hazard data ingestion with a detailed process of geoprocessing to assess areas, populations, and infrastructure that would be affected by natural hazards.

I identified and categorized hazard resources, including flood zones, wildfire perimeters, and weather forecast data. These sources differed in their geographic coverage and update schedules. I developed Python extract-transform-load workflows to bring them into the platform's analysis process, with hourly and daily ingestion routines matched to the relevant feeds. The purpose was to make updated information available through a repeatable process that supported monitoring and planning.

A significant troubleshooting issue emerged when I examined how Census population data were being assigned to the platform's H3 hexagonal grid. Census tracts could extend across multiple cells, so the geographic relationship required more attention than the original polygon-join approach provided. The shape of the reporting units and the shape of the analytical grid did not line up neatly. That mismatch affected the exposure counts used by the platform.

I replaced the original join approach with a revised method for assigning population data to the hexagonal cells. The correction improved the population exposure estimates for eight HHS-defined at-risk groups. This was a problem in the analytical foundation of the product, so resolving it mattered to the information the map communicated as well as to the data pipeline itself.

I also developed and troubleshot automated workflows for observed and forecast flood and wildfire data. This included working with National Interagency Fire Center resources, National Water Model datasets, and MODIS and VIIRS fire observations. I checked returned GeoJSON, geographic coverage, and record limits, and resolved retrieval problems associated with larger datasets.

To support the broader integration process of census data and mapping that to our webmap, I built tools to retrieve state and county boundaries automatically, derived state identifiers from county FIPS codes, and helped define a consistent structure for H3 output files.

My contribution helped connect live and forecast hazard information to population characteristics in a way that emergency-management users could explore through the platform.