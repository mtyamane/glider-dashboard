# Glider Data Dashboard — 5 Consolidated Use Cases

## Use Case 1: Explore and Analyze Ocean Observations

### Who is the User?

- **Persona/Role:** General public, recreational ocean users, commercial fishermen, researchers, environmental scientists, educators, and public health specialists.
- **Context:** Users interested in exploring biological and environmental observations to understand ocean conditions, identify patterns, investigate unusual events, support scientific research, or inform recreational and commercial activities.

### What Do They Want to Do with the Tool?

**Primary Tasks:**

- Explore biological and environmental observations from current and historical glider deployments.
- Compare ocean conditions across different locations, times, depths, or environmental cycles.
- Identify patterns, trends, anomalies, and areas with high plankton abundance.
- Use available observations to inform scientific investigations, ocean-related activities, and educational exploration.

**Operational Workflows:**

1. **Select a glider deployment, geographic region, and time period.** All users; support selection of current or historical deployments, including multiple deployments for comparison.
2. **Choose biological, environmental, or operational measurements to display.** Examples include temperature, salinity, chlorophyll, phytoplankton, zooplankton biomass, depth, and relevant glider operational information.
3. **Visualize selected observations using maps and charts.** Provide geographic maps, time-series plots, and depth-resolved visualizations where appropriate. Offer simplified views for nontechnical users and detailed views for researchers.
4. **Apply filters and comparisons relevant to the user's goals:**

   - Compare different years and seasons (stories #1, #4, #5, #7).
   - Compare El Niño and La Niña periods (#4).
   - Overlay lunar phases and filter day/night measurements (#2).
   - Filter measurements by depth, location, and glider (#7, #13, #31).
   - View recent plankton biomass hotspots or temperature conditions (#8, #16, #22–25).
   - Compare observations with historical conditions to identify environmental anomalies (#5, #15, #28).
5. **Explore and interpret observations.** Examine selected values, trends, spatial distributions, and possible relationships among measurements.
6. **Assess the reliability and relevance of observations.** Review timestamps, data sources, quality flags, sample counts, and geographic or temporal coverage gaps, as applicable.

### Needs and Desires

- Interactive maps, time-series charts, and depth-resolved visualizations.
- Flexible geographic, temporal, depth, and variable filters.
- Historical and environmental-cycle comparison tools.
- Color-coded plankton and temperature visualizations.
- Visible measurement timestamps, quality indicators, and coverage gaps.
- Plain-language explanations for nontechnical audiences.
- Detailed scientific visualizations and metadata for advanced users.
- Mobile-friendly access, including lightweight views for limited connectivity.

### Technical Skill Level

Ranges from nontechnical public users to experienced researchers with advanced scientific and programming skills. The interface should support both accessible exploration and detailed scientific analysis.

Original user stories: #1, #2, #4, #5, #7, #8, #13, #15, #16, #17, #22, #23, #24, #25, #28, #30, #31, #32

---

## Use Case 2: Monitor Active Glider Deployments

### Who is the User?

- **Persona/Role:** Glider operators, maintenance technicians, principal investigators, marine scientists, and maintenance managers.
- **Context:** Users responsible for monitoring active deployments, ensuring gliders are operating as expected, assessing sensor measurements, and identifying situations requiring operational attention.

### What Do They Want to Do with the Tool?

**Primary Tasks:**

- Monitor the operational status and health of deployed gliders.
- Assess incoming biological, environmental, and technical observations.
- Detect technical problems and identify scientifically interesting areas that may warrant additional sampling.
- Review historical status and error information when investigating potential problems.

**Operational Workflows:**

1. **Select an active glider deployment.** Display the glider's latest reported location, observation time, and mission status.
2. **Select operational, environmental, or biological measurements to monitor:**

   - Battery level and historical battery trends (#9, #10, #18, #26).
   - Sensor status and technical errors (#18, #26, #27).
   - Temperature, chlorophyll, zooplankton biomass, and other scientific measurements (#7, #11, #19).
   - Active acoustic measurements and their quality (#12).
3. **Visualize selected measurements over time.** Use automatically updated status indicators, maps, time-series plots, and depth-resolved visualizations as appropriate.
4. **Identify conditions that require attention:**

   - Low battery levels or abnormal technical status (#9, #10, #18, #26).
   - Repeated technical errors or maintenance-related patterns (#26, #27).
   - Unusual biological or environmental features that could benefit from additional sampling (#7, #11, #19).
   - Potential acoustic data quality issues (#12).
5. **Review measurements in greater detail.** Examine time-specific observations, historical trends, quality flags, and relevant technical information.
6. **Use the observations to inform operational decisions.** Determine whether maintenance attention, further investigation, or adjusted sampling should be recommended. The dashboard supports monitoring and decision-making rather than directly controlling the glider.

### Needs and Desires

- Automatically refreshed measurements with visible timestamps.
- Current battery levels, trends, and configurable warnings or guidance.
- Sensor status and technical error indicators.
- Historical error information by time and location.
- Synchronized scientific measurements for active mission monitoring.
- Specialized acoustic visualizations where applicable.
- Desktop and mobile access.
- Clear status indicators for novice operators and detailed data for experienced personnel.

### Technical Skill Level

Moderate to high operational or scientific expertise, although some users are novice glider operators or have limited programming and data-processing experience.

Original user stories: #7, #9, #10, #11, #12, #18, #19, #26, #27

---

## Use Case 3: Access, Download, and Integrate Glider Data

### Who is the User?

- **Persona/Role:** Researchers, students, data scientists, software developers, and external application developers.
- **Context:** Users who need to retrieve glider observations and metadata for independent research, exploratory analysis, or integration with external applications.

### What Do They Want to Do with the Tool?

**Primary Tasks:**

- Retrieve raw or processed glider data.
- Download selected observations in standard data formats.
- Access glider datasets programmatically.
- Obtain metadata necessary to interpret, validate, and reuse the data.

**Operational Workflows:**

1. **Select a dataset or glider deployment.** Browse available historical and current deployment data.
2. **Specify the required observations.** Filter by geographic region, time range, depth, glider, and measurement type as needed.
3. **Select a method of data retrieval:**

   - Download datasets in CSV, JSON, or netCDF formats where supported (#3, #7, #13, #17, #31).
   - Retrieve data programmatically through a documented API (#3, #31).
4. **Retrieve the selected data and associated metadata.** Include relevant information about measurement units, timestamps, locations, sensor details, processing, and quality flags.
5. **Review data documentation.** Identify data update frequency, processing methods, calibration information, and attribution requirements where relevant.
6. **Use the retrieved data in external applications or analytical environments.** Examples include R, Python, and independently developed software.

### Needs and Desires

- Standardized downloadable data formats.
- Documented API access where available.
- Flexible data selection and filtering.
- Data dictionaries and metadata.
- Sensor calibration, processing information, and quality flags.
- Data provenance, update frequency, and attribution requirements.
- Accessible workflows for both novice and advanced users.

### Technical Skill Level

Ranges from undergraduate students unfamiliar with data portals to experienced developers and researchers proficient in scientific programming.

Original user stories: #3, #7, #13, #15, #17, #31

---

## Use Case 4: Evaluate and Communicate Glider Mission Performance and Findings

### Who is the User?

- **Persona/Role:** Research lab directors, maintenance managers, funding administrators, policy analysts, educators, and students.
- **Context:** Users who need to summarize glider observations or mission performance and communicate findings to decision-makers, funders, policymakers, students, or the general public.

### What Do They Want to Do with the Tool?

**Primary Tasks:**

- Review summaries of glider missions and scientific observations.
- Evaluate mission performance and operational efficiency.
- Prepare visualizations and summaries for reports or presentations.
- Communicate scientific observations to audiences with varying levels of technical expertise.

**Operational Workflows:**

1. **Select the relevant glider deployment, geographic area, or time period.**
2. **Choose the information to summarize:**

   - Mission duration, distance traveled, and operational status (#21, #29).
   - Amount of biological and environmental data collected (#21, #29).
   - Maintenance downtime, technical errors, and operational costs (#27, #29).
   - Biological or environmental observations and trends (#6, #20, #30).
3. **View summarized metrics and visualizations.** Display appropriate charts, tables, maps, or high-level indicators.
4. **Apply comparisons appropriate to the reporting objective:**

   - Compare multiple gliders or deployments (#21, #29).
   - Analyze trends in maintenance issues or operational efficiency (#27, #29).
   - Calculate cost per day of useful data when relevant financial records are available (#29).
   - Summarize environmental trends or glider observations for policy or educational purposes (#6, #20, #30).
5. **Review supporting information.** Examine data sources, observation dates, sample sizes, and relevant limitations.
6. **Export or present the results.** Generate charts and tables suitable for reports, presentations, classroom activities, or discussions with stakeholders.

### Needs and Desires

- High-level summary dashboards.
- Configurable key performance indicators and comparisons.
- Mission statistics, technical status, and data collection summaries.
- Operational and financial information where available.
- Presentation-ready charts, maps, and tables.
- Clear data provenance and observation coverage.
- Accessible, plain-language explanations and educational tooltips.
- Compatibility with desktop, mobile, and classroom displays.

### Technical Skill Level

Low to moderate. Users generally have basic computer and chart-reading skills, with some having specialized scientific, financial, or policy expertise.

Original user stories: #6, #20, #21, #27, #29, #30, #32

---

## Use Case 5: Extend Dashboard Functionality with New Data Products

### Who is the User?

- **Persona/Role:** Software developer.
- **Context:** Developers responsible for incorporating newly processed glider sensor outputs or additional visualization capabilities into the existing dashboard.

### What Do They Want to Do with the Tool?

**Primary Tasks:**

- Integrate new sensor data products.
- Add visualizations to existing dashboard functionality.
- Ensure that new components do not disrupt existing modules.

**Operational Workflows:**

1. **Identify the new data product or visualization to integrate.** For example, optical measurements generated through plankton camera image processing.
2. **Access the relevant sensor data and integration documentation.**
3. **Develop or configure the new visualization module.**
4. **Connect the module to the appropriate data source.**
5. **Integrate the module into the dashboard's existing structure.**
6. **Test the new functionality and verify that existing dashboard modules continue working correctly.**

### Needs and Desires

- Modular dashboard architecture.
- Clear developer documentation.
- Consistent and documented data interfaces.
- Straightforward procedures for adding visualization components.
- Isolation of components to prevent unintended effects on existing functionality.

### Technical Skill Level

Moderate to high. Comfortable with software development and visualization tools, but potentially unfamiliar with the dashboard's architecture.

Original user story: #14

### Summary of the Final 5 Use Cases

| # | Use case | Original user stories |
|---|---|---|
| 1 | Explore and Analyze Ocean Observations | 1, 2, 4, 5, 7, 8, 13, 15, 16, 17, 22, 23, 24, 25, 28, 30, 31, 32 |
| 2 | Monitor Active Glider Deployments | 7, 9, 10, 11, 12, 18, 19, 26, 27 |
| 3 | Access, Download, and Integrate Glider Data | 3, 7, 13, 15, 17, 31 |
| 4 | Evaluate and Communicate Glider Mission Performance and Findings | 6, 20, 21, 27, 29, 30, 32 |
| 5 | Extend Dashboard Functionality with New Data Products | 14 |
