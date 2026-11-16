### Use Case 1: Explore Historical Ocean Conditions and Environmental Trends
Who is the User?
- Persona/Role: Tam (Tribal Member), Sammy (Sea Witch), Nico (Surfer), Namor (Ocean Steward)
- Context: Users interested in understanding how biological and environmental conditions change over time, including seasonal, annual, lunar, and climate-related patterns.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Compare historical plankton abundance and ocean conditions across years or seasons.
  - Identify trends, unusual observations, and relationships with environmental cycles.
  - Explore how factors such as lunar phases and El Niño/La Niña periods relate to ocean conditions.
- Operational Workflows:
  1. Select a geographic region and time range.
  2. Choose biological or environmental variables.
  3. Visualize historical measurements using maps and time-series charts.
  4. Compare different years, seasons, lunar phases, or climate conditions.
  5. Interpret patterns while considering data coverage and sample sizes.
Needs and Desires
- Interactive maps and historical time-series visualizations.
- Filters for location, time, season, and relevant environmental cycles.
- Optional lunar-phase overlays, day/night filters, and climate-phase comparisons.
- Clear legends, source information, and warnings about sparse observations.
Technical Skill Level
Low to moderate. Users understand their particular interests or ocean-related activities but generally have no programming experience.

Source user stories: #1, #2, #4, #5

### Use Case 2: Explore Recent Ocean Conditions for Recreational and Commercial Activities
Who is the User?
- Persona/Role: Marcus (Commercial Fisherman), Josh (Fisherman), Emma (Diver), Jake (Surfer), Marcus (Whale-Watching Fan), Sue (Travel Instructor), Elmo (Parent)
- Context: Members of the public and commercial users who want accessible information about recent ocean conditions to inform fishing, whale-watching, diving, surfing, and coastal outings.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Identify locations with high plankton biomass.
  - Check recent water temperatures and available environmental measurements.
  - Explore possible areas of fish or whale feeding activity.
  - Use ocean observations to inform recreational and commercial trip planning.
- Operational Workflows:
  1. Open the dashboard on a mobile device or computer.
  2. Select a coastal region or location of interest.
  3. View the latest available biological and environmental observations on a map.
  4. Examine color-coded plankton biomass, water temperature, or depth-specific measurements.
  5. Check observation timestamps and coverage gaps before planning activities.
Needs and Desires
- Simple, mobile-friendly maps with clear color legends.
- Easily accessible temperature and plankton measurements.
- Recent observation dates and indicators of data freshness.
- Lightweight views suitable for slow internet connections.
- Plain-language explanations of what measurements may indicate.
Technical Skill Level
Low. Most users have little scientific or computing experience and want information quickly without navigating complex plots.

Source user stories: #8, #16, #22, #23, #24, #25, #32

### Use Case 3: Investigate Environmental Anomalies and Potential Water Quality Concerns
Who is the User?
- Persona/Role: Namor (Ocean Steward), Dr. Rivera (Emergency Physician/Public Health Specialist), Nora (Pollution Researcher)
- Context: Users investigating unusual environmental conditions, ecosystem changes, or possible relationships between water conditions and human activities or health concerns.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Identify unusual biological and environmental measurements.
  - Examine conditions in particular geographic areas and time periods.
  - Investigate possible associations between ocean conditions and reported environmental or health events.
  - Retrieve relevant observations for further investigation.
- Operational Workflows:
  1. Select a geographic area and time period.
  2. Display available environmental and biological measurements.
  3. Compare observed values against historical measurements.
  4. Identify anomalies in temperature, salinity, chlorophyll, or plankton abundance.
  5. Examine geographic patterns and data coverage.
  6. Export relevant observations for further analysis.
Needs and Desires
- Spatial and temporal filtering.
- Maps and charts showing environmental anomalies.
- Historical comparisons and indicators of unusual readings.
- Data quality information, measurement sources, and coverage gaps.
- Downloadable observations for scientific or public health investigations.
Technical Skill Level
Mixed. Users may have substantial expertise in medicine, ocean science, or environmental research but varying levels of programming experience.

Source user stories: #5, #15, #28

Scope consideration: Detecting plastics, trash, pathogens, or determining whether water is safe for swimming requires additional measurements or datasets. Glider observations alone may support investigation but cannot establish pollution levels, health risks, or causation.

### Use Case 4: Monitor Scientific Observations During Active Glider Deployments
Who is the User?
- Persona/Role: Dr. Ellis (Marine Biologist), George (Principal Investigator), John (Acoustics Principal Investigator), Sarah (Marine Ecologist)
- Context: Scientists who monitor glider observations during active missions to assess data quality, identify interesting environmental features, and inform potential sampling adjustments.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Monitor recent biological and environmental measurements.
  - Identify plankton patches, temperature fronts, or unusual ocean conditions.
  - Assess whether the glider should revisit a particular area.
  - Monitor the quality of specialized measurements such as active acoustic data.
- Operational Workflows:
  1. Select an active glider deployment.
  2. View recently received observations along the glider trajectory.
  3. Display multiple biological or environmental variables simultaneously.
  4. Use time and depth filters to investigate particular observations.
  5. Review acoustic data or other specialized sensor measurements as applicable.
  6. Identify areas of interest and communicate potential sampling changes to operators.
Needs and Desires
- Frequently updated scientific observations.
- Multiple synchronized charts and maps.
- Depth-resolved visualizations along the glider trajectory.
- Time sliders and variable selection.
- Sensor quality indicators and measurement timestamps.
- Access to both current and previous acoustic observations where relevant.
Technical Skill Level
High scientific expertise, with varying programming skills. Users prefer interactive visualizations when making time-sensitive decisions during deployments.

Source user stories: #7, #11, #12, #19

### Use Case 5: Conduct Detailed Scientific Analysis Across Glider Deployments
Who is the User?
- Persona/Role: Dr. Ellis (Marine Biologist), Tim (Oceanographer), Dakota (Graduate Student), Jack (Undergraduate Student)
- Context: Researchers and students analyzing historical glider observations to investigate relationships between ocean conditions, biological distributions, and glider operations.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Explore observations from current and historical deployments.
  - Analyze variations by time, location, depth, and glider.
  - Compare biological, environmental, and operational measurements.
  - Identify patterns, correlations, and potential measurement anomalies.
- Operational Workflows:
  1. Select one or multiple deployments.
  2. View deployment trajectories and available measurements.
  3. Filter data by time range, location, depth, or measurement type.
  4. Display selected variables on synchronized maps and charts.
  5. Compare measurements across deployments or environmental conditions.
  6. Examine quality flags and operational context to interpret findings.
Needs and Desires
- Flexible multi-variable scientific visualizations.
- Maps, time-series charts, and depth-resolved plots.
- Historical deployment browsing.
- Advanced filtering and comparison tools.
- Measurement quality flags and processing information.
- Access to raw data for independent analysis.
Technical Skill Level
Moderate to high. Includes students who are new to glider data and experienced researchers proficient in scientific programming.

Source user stories: #7, #13, #17, #31

### Use Case 6: Monitor Glider Technical Health and Maintenance Needs
Who is the User?
- Persona/Role: Hank (Experienced Glider Operator), Sally (New Glider Operator), Allen (Glider Pilot), Joe (Maintenance Technician), Derrick (Maintenance Manager)
- Context: Personnel responsible for monitoring glider operational health, identifying technical problems, and maintaining reliable deployments.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Check glider battery status and remaining operational capacity.
  - Monitor sensor functionality and technical errors.
  - Identify potential failures or maintenance needs.
  - Review historical technical problems to improve maintenance practices.
- Operational Workflows:
  1. Select a glider from the operational dashboard.
  2. View its most recent battery and sensor status.
  3. Examine battery trends and technical indicators over time.
  4. Identify warnings, errors, or unusual conditions.
  5. Review historical technical issues by time and location.
  6. Use the information to inform operational or maintenance decisions.
Needs and Desires
- Automatically refreshed operational status.
- Battery indicators and historical trends.
- Low-battery warnings and understandable status explanations.
- Sensor health and technical error indicators.
- Historical error timelines and geographic visualizations.
- Desktop and mobile access.
- Read-only monitoring without glider-control functionality.
Technical Skill Level
Mixed. Ranges from newly hired operators to experienced technicians and financially focused maintenance managers.

Source user stories: #9, #10, #18, #26, #27

### Use Case 7: Evaluate Glider Mission Performance and Operational Efficiency
Who is the User?
- Persona/Role: David (Research Lab Director), Derrick (Maintenance Manager), Esme (National Institute of Science Staff)
- Context: Managers and administrators responsible for monitoring mission progress, evaluating resource utilization, and reporting the performance and value of glider operations.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Monitor mission progress and operational performance.
  - Compare mission duration, distance traveled, data collected, and downtime.
  - Review maintenance trends and operational efficiency.
  - Evaluate financial metrics and return on investment.
- Operational Workflows:
  1. Open the mission performance dashboard.
  2. Select an individual glider or group of deployments.
  3. Review mission duration, distance, technical health, and data collection metrics.
  4. Compare performance across gliders or time periods.
  5. Examine downtime, maintenance records, and available cost information.
  6. Export summary information for administrative reporting.
Needs and Desires
- High-level mission performance summaries.
- Comparisons across gliders and deployments.
- Operational and maintenance statistics.
- Cost and efficiency metrics, including cost per day of useful data.
- Exportable charts and tables.
- Clear presentations without excessive scientific detail.
Technical Skill Level
Low to moderate. Users understand scientific program management, finances, or basic charts but generally do not perform advanced data analysis.

Source user stories: #21, #27, #29

Data dependency: Cost, repair, and some downtime metrics require administrative or maintenance records beyond scientific glider observations.

### Use Case 8: Retrieve and Integrate Glider Data for External Analysis and Applications
Who is the User?
- Persona/Role: Zooey Plankton (App Developer), Dr. Ellis (Marine Biologist), Jack (Undergraduate Student), Tim (Oceanographer), Dakota (Graduate Student)
- Context: Developers, researchers, and students who need raw glider observations for independent analysis, research projects, or integration into external applications.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Download observations from selected glider deployments.
  - Retrieve data programmatically through an API.
  - Access sensor and processing metadata.
  - Integrate glider observations into external analytical tools or software applications.
- Operational Workflows:
  1. Browse available deployments and datasets.
  2. Select variables, date ranges, depths, or geographic areas.
  3. Choose a supported export format, such as CSV, JSON, or netCDF.
  4. Download the selected observations or access them through an API.
  5. Review data dictionaries, quality flags, and processing details.
  6. Import the data into external applications or analytical software.
Needs and Desires
- Downloadable raw observations in standard formats.
- Documented programmatic access.
- Data dictionaries including units, timestamps, and locations.
- Sensor calibration, processing, and quality information.
- Clear data update frequency and attribution requirements.
- Easy data selection for users with different technical backgrounds.
Technical Skill Level
Mixed, ranging from beginners exploring data portals to proficient developers and scientists using Python, R, and APIs.

Source user stories: #3, #7, #13, #17, #31

### Use Case 9: Communicate and Educate Using Glider Observations
Who is the User?
- Persona/Role: Carter (Policy Analyst), Linda (High School Science Teacher), David (Research Lab Director), Paul (High School Student), Elmo (Parent)
- Context: Users who want to present glider observations to nontechnical audiences, including policymakers, funders, students, and families.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Explore and explain glider missions and ocean measurements.
  - Communicate scientific findings through accessible visualizations.
  - Create charts and summaries for presentations or reports.
  - Use glider observations for educational activities.
- Operational Workflows:
  1. Select a glider, deployment, geographic area, or measurement.
  2. View simplified maps, trajectories, and ocean measurements.
  3. Explore concise explanations of scientific variables and patterns.
  4. Review data sources, observation dates, and supporting sample counts.
  5. Export relevant charts or figures for reports, presentations, or educational materials.
Needs and Desires
- Simple and engaging interactive visualizations.
- Plain-language captions, tooltips, and explanations.
- Maps showing glider positions, trajectories, and diving depths.
- Clearly presented environmental and biological measurements.
- Visible data provenance and observation coverage.
- Presentation-ready figures and export capabilities.
- Compatibility with mobile devices and classroom projectors.
Technical Skill Level
Low to moderate. Users generally have basic computer skills and may have educational, policy, or scientific backgrounds, but do not need programming functionality.

Source user stories: #6, #20, #21, #30, #32

### Use Case 10: Extend the Dashboard with New Data Products and Visualizations
Who is the User?
- Persona/Role: Mark (Software Developer)
- Context: Developers who create new sensor processing outputs and need to integrate additional data products into the existing glider dashboard.
What Do They Want to Do with the Tool?
- Primary Tasks:
  - Access newly processed glider sensor data.
  - Add new visualizations and data products to the dashboard.
  - Integrate additional functionality without disrupting existing modules.
- Operational Workflows:
  1. Access existing sensor datasets and processing outputs.
  2. Review documentation for the dashboard's data interfaces.
  3. Develop or configure a visualization for a new data product.
  4. Integrate the visualization into the dashboard.
  5. Test the new component and confirm compatibility with existing functionality.
Needs and Desires
- Clear developer documentation.
- Consistent and documented data interfaces.
- Modular dashboard architecture.
- Straightforward integration of new plots or figures.
- Isolation of functionality to minimize impacts on existing dashboard components.
Technical Skill Level
Moderate to high. Comfortable with software development and data visualization but relatively new to implementing dashboard modules.

Source user story: #14

### Summary of the Final 10 Use Cases
#	Use case	Original user stories
1	Explore Historical Ocean Conditions and Environmental Trends	1, 2, 4, 5
2	Explore Recent Ocean Conditions for Recreational and Commercial Activities	8, 16, 22, 23, 24, 25, 32
3	Investigate Environmental Anomalies and Potential Water Quality Concerns	5, 15, 28
4	Monitor Scientific Observations During Active Glider Deployments	7, 11, 12, 19
5	Conduct Detailed Scientific Analysis Across Glider Deployments	7, 13, 17, 31
6	Monitor Glider Technical Health and Maintenance Needs	9, 10, 18, 26, 27
7	Evaluate Glider Mission Performance and Operational Efficiency	21, 27, 29
8	Retrieve and Integrate Glider Data for External Analysis and Applications	3, 7, 13, 17, 31
9	Communicate and Educate Using Glider Observations	6, 20, 21, 30, 32
10	Extend the Dashboard with New Data Products and Visualizations	14