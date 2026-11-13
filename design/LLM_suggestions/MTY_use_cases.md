# LLM Output

# ChatGPT (GPT-6)

This document groups the 32 supplied user stories into broader use cases for software-development planning, workflow documentation, and feature prioritization.

- **Clusters are the primary documentation units.** Each cluster represents a related user goal and the system capability needed to support it.
- **Stories may appear in more than one cluster.** This is intentional when a story describes several distinct goals (for example, live monitoring and historical data access).
- **Requirements below are derived from the supplied stories.** Where the stories do not specify behavior, thresholds, formats, or data sources, the item is marked **TBD** rather than assumed.
- **Feature priorities are not assigned yet.** The feature lists are candidates for later scoring across all clusters.

## Cluster index

| Use case | Cluster                                               | Primary user goal                                                                                 | Primary stories                                        |
|:---------|:------------------------------------------------------|---------------------------------------------------------------------------------------------------|:-------------------------------------------------------|
| UC-01    | Explore Ocean Conditions                              | Explore ocean conditions across locations, depths, and time                                       | US-01, US-02, US-04, US-05, US-15, US-22, US-23, US-32 |
| UC-02    | Identify Biological Hotspots                          | Locate plankton-rich areas and explore biological distributions                                   | US-08, US-16, US-24, US-25                             |
| UC-03    | Monitor Scientific Data and Support Adaptive Sampling | Monitor biological and environmental measurements during deployments to inform sampling decisions | US-07, US-11, US-19, US-31                             |
| UC-04    | Monitor Glider Health and Technical Status            | Assess battery, sensor operation, and technical errors                                            | US-09, US-10, US-18, US-26                             |
| UC-05    | Access, Retrieve, and Export Glider Data              | Retrieve historical or raw observations through an interface, export, or API                      | US-03, US-07, US-13, US-15, US-17, US-31               |
| UC-06    | Monitor and Explore Active Acoustic Data              | Monitor active acoustic data quality and explore current or previous deployments                  | US-12                                                  |
| UC-07    | Evaluate Mission and Operational Performance          | Summarize mission progress, maintenance, costs, and return on investment                          | US-21, US-27, US-29                                    |
| UC-08    | Extend the Dashboard with New Data Products           | Add new data products and visualizations without disrupting existing modules                      | US-14                                                  |
| UC-09    | Communicate Scientific Observations                   | Present observations through summaries, reports, and educational views                            | US-06, US-20, US-30                                    |
| UC-10    | Investigate Marine Pollution                          | Explore pollution locations and possible relationships with human activity                        | US-28                                                  |

## Cross-cluster feature backlog

The following is a consolidated starting point for prioritization. It groups similar capabilities that appear in multiple use cases. It is not a final implementation plan, and no scores have been assigned.

| Feature group                | Consolidated feature                               | Related use cases                        | Supporting stories                                                                               |
|:-----------------------------|:---------------------------------------------------|------------------------------------------|:-------------------------------------------------------------------------------------------------|
| Maps and spatial exploration | Interactive map with geographic selection          | UC-01, UC-02, UC-03, UC-05, UC-09, UC-10 | US-01, US-04, US-05, US-08, US-13, US-15, US-16, US-20, US-24, US-25, US-28, US-30, US-31, US-32 |
| Maps and spatial exploration | Glider location and trajectory display             | UC-03, UC-05, UC-09                      | US-07, US-13, US-20, US-30, US-31                                                                |
| Coverage and transparency    | Coverage-gap visualization                         | UC-01, UC-02                             | US-01, US-04, US-05, US-08, US-15                                                                |
| Time controls                | Date/time filtering and time slider                | UC-01, UC-03, UC-05, UC-06               | US-02, US-04, US-07, US-12, US-13, US-15, US-31                                                  |
| Comparison                   | Historical and seasonal comparisons                | UC-01                                    | US-01, US-02, US-04, US-05                                                                       |
| Comparison                   | Multi-parameter overlays and comparisons           | UC-01, UC-03                             | US-04, US-05, US-07, US-11, US-15, US-19, US-31                                                  |
| Biological data              | Plankton biomass/abundance visualization           | UC-01, UC-02, UC-03                      | US-01, US-02, US-04, US-05, US-08, US-16, US-19, US-24, US-25                                    |
| Depth                        | Depth-resolved measurement views                   | UC-01, UC-03, UC-09                      | US-07, US-22, US-30, US-31                                                                       |
| Data freshness               | Latest observation and data-age indicator          | UC-02, UC-04                             | US-08, US-16, US-18, US-26                                                                       |
| Data quality                 | Measurement quality flags and provenance           | UC-01, UC-03, UC-05, UC-09               | US-01, US-03, US-06, US-07, US-15, US-31                                                         |
| Data access                  | CSV/JSON/netCDF export                             | UC-05                                    | US-03, US-07, US-13, US-15, US-17, US-31                                                         |
| Data access                  | Programmatic API                                   | UC-05                                    | US-03, US-31                                                                                     |
| Data access                  | Data dictionary and technical documentation        | UC-05                                    | US-03, US-07, US-31                                                                              |
| Operational monitoring       | Battery status and history                         | UC-04                                    | US-09, US-10, US-18, US-26                                                                       |
| Operational monitoring       | Sensor status and error reporting                  | UC-04, UC-07                             | US-18, US-26, US-27                                                                              |
| Operational monitoring       | Automatic data refresh                             | UC-03, UC-04                             | US-07, US-11, US-18, US-19                                                                       |
| Reporting                    | Summary dashboard and report exports               | UC-07, UC-09                             | US-06, US-21, US-29                                                                              |
| Extensibility                | Modular data-product and visualization integration | UC-08                                    | US-14                                                                                            |
| Accessibility                | Plain-language labels, legends, and explanations   | UC-01, UC-02, UC-09                      | US-01, US-02, US-04, US-05, US-06, US-20, US-22, US-23, US-30, US-32                             |
| Responsive/field use         | Mobile-friendly and low-bandwidth interface        | UC-01, UC-02, UC-04, UC-09               | US-08, US-09, US-10, US-16, US-18, US-22, US-23, US-24, US-25, US-26, US-32                      |
| Operations analytics         | Mission, maintenance, and cost metrics             | UC-07                                    | US-21, US-27, US-29                                                                              |

## Traceability notes and decisions to validate

1.  **Stories are intentionally cross-referenced.** A story can support more than one use case because it may contain several goals. The cluster index lists primary placements; the detailed sections and cross-cluster backlog capture secondary relationships.
2.  **US-07 and US-15 span multiple capabilities.** Their monitoring, analysis, and export needs are separated across the relevant use cases.
3.  **US-31 spans scientific monitoring and data access.** Its combined map/timeline exploration is represented in UC-03, while raw download, API, and documentation needs are represented in UC-05.
4.  **US-28 is kept separate.** Pollution mapping and comparison with human activity require data sources and processing that are not established by the other stories.
5.  **US-12 is currently a standalone cluster.** It may later be combined with UC-03 if active acoustic monitoring is treated as one part of a broader scientific-data monitoring capability.
6.  **US-14 is an enabling/developer use case.** It supports the extensibility of the dashboard rather than a direct end-user scientific workflow.
7.  **No priority ranking is implied.** The stories do not provide enough information about project strategy, implementation effort, data readiness, or stakeholder weighting to rank features responsibly.

---
---

# Claude (Opus 5.5, medium)

Step 1 of the use case template applied to the 32 user stories in `user_stories.md`. Stories are grouped by **what the user wants to do with the tool**. Story IDs use the story numbers (US-01 = Tam, US-32 = Elmo).

---

## Step 1: Groups by goal

| Group ID | Shared goal (verb + object) | Story IDs | Users involved | Skill levels covered |
|---|---|---|---|---|
| G-01 | **Monitor glider health during a deployment** | US-09, US-10, US-18, US-26 | Hank, Sally, Allen, Joe | Novice (Sally) to Expert (Hank); domain-skilled, not data-skilled (Allen, Joe) |
| G-02 | **Watch science data live to steer the glider** | US-07, US-11, US-12, US-19 | Dr. Ellis, George, John, Sarah | Expert scientists; do not want to code mid-mission |
| G-03 | **Download or pull glider data for own analysis** | US-03, US-07, US-13, US-15, US-17, US-31 | Zooey, Dr. Ellis, Jack, Dr. Rivera, Tim, Dakota | Novice to portals (Jack, Rivera) to expert coders (Zooey, Ellis, Tim, Dakota) |
| G-04 | **Compare ocean and plankton patterns across time** | US-01, US-02, US-04, US-07, US-12, US-31 | Tam, Sammy, Nico, Dr. Ellis, John, Dakota | Interface-only, no data background (Tam, Sammy, Nico) to expert (Ellis, John, Dakota) |
| G-05 | **Find where plankton or biomass is concentrated now** | US-08, US-16, US-24, US-25 | Marcus (fisherman), Josh, Marcus (whale fan), Sue | Non-technical, mostly on phones |
| G-06 | **Check current water conditions before going in the water** | US-22, US-23, US-32 | Emma, Jake, Elmo | Non-technical, phone users who want a fast answer |
| G-07 | **Investigate unusual water conditions in an area** | US-05, US-15 | Namor, Dr. Rivera | Domain experts with no data/oceanography background |
| G-08 | **Get a summary of findings to report or cite** | US-06, US-21 | Carter, David | Comfortable with charts; want the big picture only |
| G-09 | **Evaluate glider costs, reliability, and maintenance** | US-27, US-29 | Derrick, Esme | Non-technical; finance/ROI focused |
| G-10 | **Learn what the glider is doing and finding** | US-20, US-30, US-32 | Linda, Paul, Elmo | Basic to comfortable with apps; no science training |
| G-11 | **Add a new data product to the dashboard** | US-14 | Mark | Knows dashboards; new to building them |
| G-12 | **Map pollution and relate it to human activity** | US-28 | Nora | Fairly tech-savvy |

### Stories placed in more than one group

| Story | Groups | Why |
|---|---|---|
| US-07 Dr. Ellis | G-02, G-03, G-04 | Watches data during deployment, analyzes afterward, and wants raw export |
| US-12 John | G-02, G-04 | Monitors acoustic data quality live and reviews past deployments |
| US-15 Dr. Rivera | G-07, G-03 | Looks back at conditions near illness cases, then exports data to share |
| US-31 Dakota | G-03, G-04 | Explores patterns on the dashboard and downloads raw data / API |
| US-32 Elmo | G-06, G-10 | Checks beach conditions and explores the ocean with his kids |


## Cross-cutting needs (apply to many use cases)

These came up in many stories. List them as non-functional requirements in each related use case rather than as separate use cases.

| Need | Stories |
|---|---|
| Mark coverage gaps so missing data isn't read as "calm," "empty," or "clean" | US-01, 02, 04, 05, 08, 15 |
| Show how much data backs a pattern or trend | US-02, 06 |
| Visible data source, date range, and attribution | US-01, 03, 06 |
| Quality flags and processing details | US-03, 07, 15, 31 |
| Plain-language labels, no jargon | US-01, 02, 04, 05, 06, 20, 30, 32 |
| Works on phone/tablet | US-08, 09, 10, 16, 22–26, 30, 32 |
| Works on slow connections; readable in sunlight | US-08 |
| Show how old the latest data is | US-08 |
| Export figures or data | US-03, 06, 07, 13, 15, 29, 31 |


## Open questions

- **US-16 Josh** and **US-08 Marcus** want fish locations. The glider measures plankton/acoustic biomass, not fish directly. Should the use case say the tool shows conditions that *may* attract fish?
- **US-28 Nora** and **US-32 Elmo** want trash/plastic or "clean water" data. Do the gliders measure pollution? If not, G-12 may be out of scope, and Elmo's "clean water" may need to become "chlorophyll/bloom level."
- **US-25 Sue** wants the dashboard findable on Google. This is a site requirement, not a use case step.
- **US-03 Zooey** and **US-31 Dakota** both ask for an API. Is an API planned, or only file downloads?
- **US-05 Namor** is a fictional (Marvel) character. Keep the story as written, or rename to a generic "underwater community steward"?