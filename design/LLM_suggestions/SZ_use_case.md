# Use Cases


## Summary

| # | Use Case | Users |
|---|---|---|
| 1 | Monitor glider health | Hank (9), Sally (10), Allen (18), Joe (26) |
| 2 | Monitor science data during a mission to direct the glider | Dr. Ellis (7), George (11), John (12), Sarah (19) |
| 3 | Compare historical patterns and spot trends or anomalies | Tam (1), Sammy (2), Nico (4), Namor (5), Carter (6), Dr. Rivera (15) |
| 4 | Find marine life hotspots | Marcus (8), Josh (16), Marcus (24), Sue (25) |
| 5 | Check current water conditions for recreation | Emma (22), Jake (23), Elmo (32) |
| 6 | Learn about gliders and the ocean | Linda (20), Paul (30), Elmo (32) |
| 7 | Download or programmatically access data | Zooey (3), Dr. Ellis (7), Jack (13), Dr. Rivera (15), Tim (17), Dakota (31) |
| 8 | Review mission and program performance | David (21), Derrick (27), Esme (29) |
| 9 | Map pollution against human activity | Nora (28) |
| 10 | Extend the dashboard with new data modules | Mark (14) |


# Use Case 1: Monitor Glider Health

### Who is the User?
* **Persona/Role:** Hank (9), Glider Operator; Sally (10), Glider Operator; Allen (18), Glider Pilot; Joe (26), Technician
* **Context:** Operators, pilots, and technicians who keep the glider running during a deployment, ranging from experienced (Hank) to first deployment (Sally).

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * Check the most recent battery level and battery level over time
  * Check that sensors are working and see any errors
  * Know when a value is unsafe
* **Operational Workflows:**
  1. Open the dashboard on desktop (office) or mobile (field).
  2. Check the latest battery level and when it was reported.
  3. Review the battery-over-time plot for the deployment.
  4. Check each sensor's status and any error messages.
  5. Respond to warning/danger indicators if levels are too low or a sensor fails.
  6. Leave the dashboard open as it refreshes automatically.

### What Needs and Desires Do They Have?
* Desktop and mobile interface
* Latest battery level and battery history
* Sensor status and error display
* Reasonable ranges and warning/danger indicators for less experienced users
* Display-only (no glider control) with automatic refresh

### What Is Their Skill Level?
* Experienced with glider hardware and operations; limited data processing or computer science skills. New operators need built-in guidance.


# Use Case 2: Monitor Science Data During a Mission to Direct the Glider

### Who is the User?
* **Persona/Role:** Dr. Ellis (7), Marine Biologist; George (11), Principal Investigator; John (12), Principal Investigator (Active Acoustics); Sarah (19), Marine Ecologist
* **Context:** Scientists who watch biological and environmental data during a deployment to decide where the glider should sample next, and review past deployments afterward.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * View multiple biological and environmental parameters together during a mission
  * Spot patches, fronts, or interesting features to revisit
  * Check data quality (including active acoustic data)
  * Review previous deployments
* **Operational Workflows:**
  1. Select the current or a previous deployment.
  2. View zooplankton biomass, temperature, salinity, chlorophyll, and acoustic data on the same screen.
  3. View depth-resolved sections along the glider track.
  4. Use a time slider and filters (time of day, depth) to focus on a subset.
  5. Check quality flags on measurements.
  6. Note the time and location of a feature and tell the pilot to send the glider back.

### What Needs and Desires Do They Have?
* Multiple parameters on one screen with a shared time/location axis
* Depth-resolved views, not just a map
* Time slider and filters for time of day and depth
* Quality flags and processing details on every measurement
* No coding needed during a mission

### What Is Their Skill Level?
* Domain experts comfortable reading scientific plots; some are comfortable with code but don't want to code mid-mission.


# Use Case 3: Compare Historical Patterns and Spot Trends or Anomalies

### Who is the User?
* **Persona/Role:** Tam (1), PNW Tribal Member; Sammy (2), Sea Witch; Nico (4), Surfer; Namor (5), K'uk'ulkan; Carter (6), Policy Analyst; Dr. Rivera (15), ER MD & Public Health Specialist
* **Context:** Non-technical users who want to compare ocean conditions across years, seasons, moon phases, or specific dates and places to inform decisions, policy, or hypotheses.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * Compare the same region and season across years (including by El Niño / La Niña phase)
  * View trends with overlays such as moon phase
  * Flag readings outside the normal range
  * Look back at conditions for a specific date range and area
  * Export figures for reports
* **Operational Workflows:**
  1. Select a region (or draw an area) and a date range, season, or set of years.
  2. Choose a comparison: across years, by climate phase, or by lunar cycle.
  3. Optionally filter day vs. night observations.
  4. View maps and time series with plain-language legends and captions.
  5. Review flagged anomalies (blooms, temperature spikes, runoff signals).
  6. Check coverage gaps and how much data backs each pattern.
  7. Export figures with the data source and date range.

### What Needs and Desires Do They Have?
* Multi-year, seasonal, and lunar-cycle comparisons
* Plain-language legends, captions, and pattern explanations
* Flags for readings outside the normal range
* Clearly marked coverage gaps so missing data isn't read as calm or clean water
* A visible amount of data behind each trend
* Visible data source and one-click figure export

### What Is Their Skill Level?
* No programming or data background; they work only through the interface.


# Use Case 4: Find Marine Life Hotspots

### Who is the User?
* **Persona/Role:** Marcus (8), Commercial Fisherman; Josh (16), Fisherman; Marcus (24), Whale Watching Fan; Sue (25), Travel Instructor
* **Context:** Fishers, whale watchers, and tour planners who use plankton and biomass as a hint for where fish or whales are gathering.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * See where high plankton or biomass areas are on a map
  * See unusually warm or cold water
  * Know how recent the data is
* **Operational Workflows:**
  1. Find the dashboard (e.g., through Google search) and open it on a phone, tablet, or browser.
  2. View the map with plankton/biomass areas color-coded.
  3. Check the date and age of the latest observations.
  4. Note coverage gaps so unsampled areas aren't treated as empty water.
  5. Pick fishing spots, whale watching spots, or tour routes.

### What Needs and Desires Do They Have?
* Simple, color-coded map of plankton/biomass
* Latest observations with date and age
* Fast loading on slow connections and readable in sunlight
* Works on phone and tablet
* Plainly marked coverage gaps

### What Is Their Skill Level?
* No coding or data background; limited time to dig.


# Use Case 5: Check Current Water Conditions for Recreation

### Who is the User?
* **Persona/Role:** Emma (22), Diver; Jake (23), Surfer; Elmo (32), Parent
* **Context:** People planning dives, surf sessions, or family beach trips.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * Check the latest water temperature (near the coast or at different depths)
  * Estimate water clarity from chlorophyll
  * Check whether water near beaches is clean
* **Operational Workflows:**
  1. Open the site on a phone or tablet.
  2. Select a location or beach.
  3. Read the latest temperature as one number or color scale.
  4. Check clarity or cleanliness notes in plain language.
  5. Decide where and when to go.

### What Needs and Desires Do They Have?
* One quick number or simple color scale
* Temperature at different depths for divers
* Plain-language clarity and cleanliness notes
* Answer in a few seconds, no charts required

### What Is Their Skill Level?
* Comfortable with phone apps; no ocean science or coding background.


# Use Case 6: Learn About Gliders and the Ocean

### Who is the User?
* **Persona/Role:** Linda (20), High School Science Teacher; Paul (30), High School Student; Elmo (32), Parent
* **Context:** Teachers, students, and families using the dashboard to learn what gliders do and what lives in the ocean.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * See where the glider is now, the path it has traveled, and how deep it dives
  * View simple charts of temperature and plankton
  * Explore a kid-friendly view
* **Operational Workflows:**
  1. Open the dashboard on a projector, laptop, phone, or tablet.
  2. View the glider's current location and path on the map.
  3. View dive depth and simple charts of measurements by depth.
  4. Read tooltips explaining each measurement.
  5. Switch to a kid-friendly view with a moving glider icon and pictures of sea life.

### What Needs and Desires Do They Have?
* Simple map with the glider's path and current location
* Easy-to-read charts with plain explanations and no jargon
* Tooltips for each measurement
* Kid-friendly visuals
* Readable on a classroom projector and on mobile devices

### What Is Their Skill Level?
* Basic computer and app skills; no coding or oceanography background.


# Use Case 7: Download or Programmatically Access Data

### Who is the User?
* **Persona/Role:** Zooey (3), Ocean Conservationist/Drag Queen; Dr. Ellis (7), Marine Biologist; Jack (13), Curious Undergrad; Dr. Rivera (15), ER MD & Public Health Specialist; Tim (17), Oceanographer; Dakota (31), Graduate Student
* **Context:** Users who want to analyze glider data in their own tools, apps, or reports.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * Select data by deployment, time range, location, depth, and variable
  * Download raw data (CSV, JSON, netCDF) or access it through an API
  * Understand units, calibration, processing, and quality flags
* **Operational Workflows:**
  1. Read the API and data dictionary documentation.
  2. Select a deployment on the map and a time range with the time slider.
  3. Filter by date, location, depth, glider, and variable.
  4. Download full-resolution raw data or query the API.
  5. Check sensor, processing, and quality flag details.
  6. Check operational data (errors, battery) to explain gaps or odd values.

### What Needs and Desires Do They Have?
* Raw, full-resolution data export in CSV, JSON, or netCDF
* Documented API with update frequency and attribution requirements
* Data dictionary covering units, timestamps, locations, calibration, and quality flags
* Map and time slider for selecting data (for less experienced users)

### What Is Their Skill Level?
* Ranges from expert programmers (Zooey, Tim, Dakota, Dr. Ellis) to beginners new to data portals (Jack) and non-programmers who share exports with others (Dr. Rivera).


# Use Case 8: Review Mission and Program Performance

### Who is the User?
* **Persona/Role:** David (21), Head of the Research Lab; Derrick (27), Maintenance Team Boss; Esme (29), Staff at National Institute of Science
* **Context:** Leaders and funders who report progress, manage maintenance costs, and track return on investment.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * See a summary of each mission and glider
  * See where and when technical errors happen
  * Compare gliders and track costs over time
  * Export charts and tables for reports
* **Operational Workflows:**
  1. Open the overview page on an office computer.
  2. View days deployed, distance traveled, health, data collected, downtime, and costs per glider.
  3. View a map and trend of technical errors by time and location.
  4. Compare gliders and time periods (e.g., cost per day of useful data).
  5. Export charts and tables for funders and leadership.

### What Needs and Desires Do They Have?
* Big-picture overview, no detailed plots
* Per-glider summary numbers and cost metrics
* Error trends by time and location
* Exportable charts and tables

### What Is Their Skill Level?
* Strong science or finance background, comfortable with spreadsheets and charts; not technical in data science.


# Use Case 9: Map Pollution Against Human Activity

### Who is the User?
* **Persona/Role:** Nora (28), Researcher
* **Context:** Researches seawater pollution from trash and plastics.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * See locations most polluted by trash and plastics
  * Compare polluted locations to where human activity takes place
* **Operational Workflows:**
  1. Open the dashboard in a web browser.
  2. View the map of polluted water.
  3. Overlay or compare locations of human activity.
  4. Collect the data for further analysis.

### What Needs and Desires Do They Have?
* Map of polluted water in a web browser
* A way to compare pollution with human activity locations

### What Is Their Skill Level?
* Relatively tech-savvy; can handle some data acquisition such as web scraping.


# Use Case 10: Extend the Dashboard with New Data Modules

### Who is the User?
* **Persona/Role:** Mark (14), Software Developer
* **Context:** Added image processing to the glider's plankton camera and wants to add optical data products to the dashboard.

### What Do They Want to Do with the Tool?
* **Primary Tasks:**
  * Pull optical data from the glider
  * Add new plots or figures without breaking other modules
* **Operational Workflows:**
  1. Read the developer documentation for adding a module.
  2. Pull data using the provided data access functions.
  3. Build a new plot module from the existing module template.
  4. Register the module so it appears in the dashboard.
  5. Run tests to confirm other modules still work.

### What Needs and Desires Do They Have?
* Easy data access
* Modular structure so new plots don't break other modules
* Works in the desktop and mobile interface

### What Is Their Skill Level?
* Familiar with data visualizations and using dashboards, but new to programming them.
