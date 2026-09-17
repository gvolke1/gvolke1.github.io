---
title: "City of Peoria Fire-Medical Dept. Optimization Project"
collection: portfolio
permalink: "/portfolio/professional_experience_examples/city-of-peoria-fire-medical-dept-optimization-project/"
layout: archive
author_profile: true
skills:
  - "Web Development"
  - "Front End Development"
  - "Cartography and Data Visualization"
  - "GIS and Spatial Analysis"
  - "Data Engineering and API Integration"
  - "Development Workflow and Collaboration"
  - "Application Prototyping, Dashboards and Business Intelligence"
  - "Project Coordination and Stakeholder Communication"
  - "Emergency Management and Public Safety Analytics"
header:
  teaser: "peoria_landing_page.png"
---
 <!--when I have time, I want to review all the files I have on my role in Peoria thoroughly, and include more image breaks for better visuals here. Looking at things like "NLT Accomplishments", and "Peoria Fire Optimizer system overview, City of Peoria Firew Department optimization project, Peoria Project README, Peoria Plots & GIS Layer Information, etc.-->

 <!--## Tools and Skills to consider later

- Web GIS
- React, MapLibre, and deck.gl
- H3 spatial indexing and hexagon-based aggregation
- ArcGIS REST services and GIS data integration
- CAD incident data and geocoding
- Fire and EMS demand, hotspot, and temporal analysis
- GIS application testing
- Cartographic design
- Color theory and thematic map symbology
- Spatial data
- Technical documentation
- Quality assurance
- Project coordination
-->
![Peoria IMPACT FEMS Optimization Platform]({{ '/images/peoria_landing_page.png' | relative_url }})

## Project Overview
The City of Peoria Fire-Medical Department Optimization Project is a data-driven decision-support platform for fire and EMS planning. The platform brings together Computer-Aided Dispatch (CAD) incident records, fire station and unit locations, road and infrastructure data, demographic context, and interactive geospatial analysis in one web-based dashboard.

The project helps users examine where and when demand occurs, understand response-time and coverage patterns, and explore how changes to station resources or deployment could affect service. Its map layers include unique-call density, dispatch-unit volume, fire and medical demand, hotspot locations, temporal patterns, travel-time analysis, and contextual infrastructure such as hospitals and train crossings. A simulation workflow and supporting charts provide a way to compare operational scenarios with a baseline configuration.

The resulting platform is intended to help department staff and city decision-makers evaluate station placement, resource allocation, staffing, and future demand using a consistent set of maps, measures, and documented interpretations.

## My Role
I was the project's geospatial lead, helping turn CAD, GIS, and demographic data into an understandable planning interface. I confirmed fire station locations, completed an initial geocoding pass for incidents, developed a heatmap of geocoded incidents with station locations, and selected demographic variables relevant to fire and EMS planning for Maricopa and Yavapai counties.

I also helped define the map content and visual language used throughout the dashboard. This included mapping demand across Peoria and areas outside the city limits, creating unique-call and dispatch-unit-volume views at H3 resolution 8, identifying top locations for all calls as well as fire and medical calls, and producing fire and medical hotspot layers. I created temporal views for selected days, including Thursday and Friday examples, and prepared maps that demonstrate the dashboard's functionality.

In addition, I added contextual layers from Peoria ArcGIS REST services, including hospitals and other infrastructure, and helped confirm that each layer's symbology communicated its meaning clearly. I selected and documented a blue sequential color ramp for the EMS-oriented density layers, using color-theory principles to create a calm, ordered visual scale while preserving distinctions between demand, reference, and hotspot layers.

I used GitHub to organize and share my project materials, documentation, and development work for review and deployment by the rest of the team.

## Web Development
I contributed to the design and content of an interactive web GIS dashboard that combines mapping, filters, layer controls, selection tools, charts, and simulation results. The interface supports exploration of demand by location, call category, and time period, while keeping analytical layers and reference layers organized for repeated operational use.

The platform uses web mapping technologies including React, MapLibre, deck.gl, and open geospatial data services. The broader system is supported by cloud services for authentication, storage, model execution, status updates, and deployment automation.

## Cartography and Data Visualization
I designed the visual system for the dashboard's analytical layers, including color ramps, layer symbology, hotspot markers, and map presentation choices. The blue sequential ramp communicates increasing call density without implying alarm, while separate symbols and supporting labels distinguish fire, ALS, BLS, and other hotspot categories.

![Blue sequential color ramp used for Peoria unique-call density]({{ '/images/peoria_unique_calls_color_ramp.png' | relative_url }})

I produced and reviewed maps for all-call demand, dispatch-unit volume, unique calls, fire calls, medical calls, top locations, fire and medical hotspots, temporal demand, and dashboard demonstrations. The goal was to make the maps readable at a glance while giving users enough context to interpret what each layer represents.

## GIS and Spatial Analysis
I used H3 hexagons as a standardized area of measurement for aggregating and comparing demand across Peoria. Incident points were geocoded, assigned to hex cells, and summarized to create density layers. I also supported hotspot analysis by ranking repeated incident locations for all calls and for specific fire and medical call categories.

The analysis incorporated fire station locations, incident geocoding, demographic variables, road and infrastructure layers, and response-related measures. Additional contextual layers from Peoria's ArcGIS REST services, such as hospitals and train crossings, help users interpret demand alongside community assets and potential operational constraints.

## Testing and Documentation
I wrote user-facing documentation explaining how to use the platform, what the controls and layers do, and how to interpret the analytical outputs. This included guidance for filters, selections, map tools, density classes, travel-time layers, simulation controls, and scenario charts.

I also reviewed the symbology and descriptions for the map layers to confirm that their visual encoding matched the underlying data and intended message. Documenting the data sources, geocoding workflow, H3 aggregation, network analysis concepts, classification choices, and limitations helps users interpret results consistently and supports future maintenance of the platform.

## Video Demonstration
<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe
    src="https://www.youtube-nocookie.com/embed/wnCsVgRMriU"
    title="Peoria Fire and EMS GIS project demonstration"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
</div>

