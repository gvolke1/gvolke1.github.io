---
layout: single
title: "Master's Thesis Research: Baltimore Housing Typology"
permalink: /research/masters-thesis/
author_profile: true
---

# Mapping Baltimore’s Housing Markets: A Research Update

*Updated September 16, 2026 | Research stage: Data collection and preparation*

I have selected ten variables for my master’s thesis on Baltimore’s housing markets and am now collecting the data for principal component analysis and cluster analysis. The project examines how housing, neighborhood amenities, access to employment, and residential patterns can inform a complementary understanding of the city’s housing-market geography.

My central research question is: **How does Baltimore’s housing typology map change when neighborhood market conditions are measured differently?**

This question connects my interests in housing affordability, long-term disinvestment, and the distribution of public and private investment. Baltimore’s housing markets vary considerably across the city, as its existing housing-market typologies document. I am particularly interested in how the characteristics of historically disinvested neighborhoods can inform discussions about reinvestment and support for existing residents. A neighborhood may contain vacant land while also offering proximity to employment, parks, and everyday services. My research will examine how these characteristics appear together across Baltimore.

Baltimore already has an established foundation for this work. Its Housing Market Typology, developed through collaboration among the Department of Planning, the Department of Housing and Community Development, and The Reinvestment Fund, groups areas with similar housing-market conditions. The city’s [announcement of the 2017 update](https://s3.amazonaws.com/baltimorecity.gov.if-us-east-1/s3fs-public/2024-02/final_hmt2017_dataseries_0122.pdf) explains how the typology supports matching public resources to neighborhood housing market conditions. The Reinvestment Fund also provides a [map of Baltimore’s 2023 Housing Market Typology](https://www.reinvestment.com/wp-content/uploads/2025/04/Reinvestment-Fund_Baltimore_MVA-HMT2023.pdf).

In his explanation of Market Value Analysis (MVA), The Reinvestment Fund's founder Ira Goldstein writes:

> “TRF (The Reinvestment Fund) created the MVA to give public officials the basis for making informed, objective decisions about how to prioritize resources and services.” [Goldstein, 2012, “Overview of the MVA Approach.”](https://www.federalreserve.gov/publications/putting-data-to-work-market-value-analysis.htm)

The [published Baltimore MVA definitions](https://www.policymap.com/data/sources/trf-market-value-analyses-mvas) document indicators including sales prices, vacancy, permits, residential density, owner occupancy, and subsidized housing. My project builds on this tradition of using multiple indicators to understand local conditions. It adds a neighborhood-character perspective that can be considered alongside Reinvestment Fund’s established work.

The housing-submarket literature helps explain why the purpose of a classification matters.  state:

> “We maintain that the appropriate definition of submarkets depends on the use to which they will be put.” [Bourassa, Hoesli, and Peng, 2003; author manuscript, abstract.](https://access.archive-ouverte.unige.ch/access/metadata/b023cc99-18b7-4f6b-8013-cbf6ce517016/download)

In [*Do Housing Submarkets Really Matter?*](https://access.archive-ouverte.unige.ch/access/metadata/b023cc99-18b7-4f6b-8013-cbf6ce517016/download), Steven Bourassa, Martin Hoesli, and Vincent Peng  evaluate walk through different methods of classifying housing submarkets. My project will direct attention to historically disinvested areas of Baltimore city. That distinction will guide how I interpret the eventual results.

George Galster’s research on neighborhood character provides the conceptual foundation for selecting variables chosen to classify housing submarkets. He defines neighborhood (applicable to submarkets) as:

> “Neighbourhood is the bundle of spatially based attributes associated with clusters of residences, sometimes in conjunction with other land uses.” [Galster, 2001, p. 2112.](https://doi.org/10.1080/00420980120087072)

Galster’s framework includes building characteristics, demographic composition, public services, environmental conditions, and proximity to employment, shopping, and entertainment. It also considers how residents, property owners, businesses, and governments produce neighborhood change. I use this framework to select the ten variables below. 

| Selected variable                   | What I intend to measure and why it belongs in the analysis                                                                                                                                                                                                                             |
| ----------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Land-use mix**                    | The composition and balance of residential, commercial, industrial, and other categories. This helps distinguish different neighborhood settings.                   |
| **Residential permit activity**     | Residential construction and rehabilitation permits, adjusted for the size of the housing stock. Permits indicate investment in the built environment. The time window and treatment of permit values are being refined.                                                     |
| **Age-specific population density** | Residents ages 25–44 relative to land area, assembled from the 25–29, 30–34, 35–39, and 40–44 ACS categories. This adds a demographic dimension relevant to household formation and residential demand. 
| **Lifestyle amenities**             | The availability, variety, and proximity of destinations such as restaurants, bars, grocery stores, salons, theaters, museums, and libraries. These describe everyday services and activities available around residential areas.                                                       |
| **Job accessibility**               | The concentration of employment within a defined distance of residential locations. People live in areas close to their job and benefit from more choices.
| **Vacant land share**               | The prevalence of vacant land within the residential environment. This data will be handled very carefully because vacancy is a major issue and defining characteristic of Baltimore City's housing market.      |
| **Housing age**                     | The median age of single-family residential properties with usable construction dates. Housing age is one of the most common measurables in housing submarket literature and will point to a desire for Baltimore's distinct architectural form (e.g. rowhouses)                                           |
| **Recent residential mobility**     | The share of current residents age one and older who lived in a different home one year earlier. This captures recent residential movement and contributes a demographic measure of neighborhood change.                                                                                |
| **Parks and recreation**            | Proximity to parks and recreational spaces, with attention to entrances and the distance residents would need to travel. This adds a public-service and open-space dimension to the analysis.                                                                                           |
| **Housing-unit density**            | Housing units per acre of residential land. This describes the concentration of the housing stock and distinguishes built-form density.                                                                               |

These choices draw on several strands of my literature review. [Latham and Layton’s research on social infrastructure](https://doi.org/10.1111/gec3.12444) helps explain why everyday destinations and public spaces matter to neighborhood life. [Costello and colleagues’ study of housing-submarket change](https://doi.org/10.1111/geoj.12303) examines new housing supply, migration, and socioeconomic change. [Heckert and Mennis’s study of vacant-land greening in Philadelphia](https://journals.sagepub.com/doi/10.1068/a4595) shows why the treatment of vacant land matters when considering its relationship with surrounding property values. These studies inform the questions I ask of Baltimore’s data; their findings still need to be considered in their original local contexts.

I am now building the data workflow, drawing from Open Baltimore, city zoning and property records, OpenStreetMap, the American Community Survey, and Census employment data. Census tracts will provide the common geography for the analysis. Each tract will eventually have one row of comparable measurements, with documentation of the source, year, definition, and limitations of each variable.

At this stage, the variable selection is settled, while several measurement decisions remain under review. Zoning describes permitted uses, so a zoning-based mix indicator must be identified clearly when discussing actual land use. Amenity and park measures must also account for nearby destinations across tract boundaries, for example.

Once those measurements are ready, PCA will summarize patterns of variation across all ten variables. It will help show which characteristics tend to occur together and which describe separate dimensions of neighborhood difference.

I will then use the retained component scores for cluster analysis, grouping tracts with similar profiles. This sequence has a direct precedent in [Bourassa and colleagues’ *Defining Housing Submarkets*](https://abdn.elsevierpure.com/en/publications/defining-housing-submarkets/), which applies PCA and then clustering. I will examine how many components preserve useful information, compare possible cluster solutions, and check whether reasonable changes to measurement choices substantially alter the results. The groups and their descriptions will follow from that analysis.

The eventual outputs will include a documented dataset, maps of individual variables, an interpretation of the principal components, and a mapped neighborhood typology. Comparing that typology with Baltimore’s existing HMT will perhaps see shared patterns and additional information that will be useful for allocating public resources to historically disinvested areas.

For now, the work is in data collection and preparation. 