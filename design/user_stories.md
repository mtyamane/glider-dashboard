# User Stories
    - Who is the User.
    - What do they want to do with the tool.
    - What needs and desires do they want for the tool.
    - What is their skill level. 


### Tam, PNW Tribal Member
1. Tam is from a Pacific Northwest tribe and helps plan the annual canoe journey.
She wants to see how zooplanketon levels in July and August compare across past years, to inform timing decisions tied to whale presence.
She needs a map with a plain-language legend, clearly marked coverage gaps, and a visible data source.
She has no programing background and works only through the interface.


### Sammy, Sea Witch
2. Sammy is a self-proclaimed sea witch who plans her practice around the moon and the tides. 
She wants to see whether zooplankton activity in the water follows the lunar cycle. 
She needs a time series of zooplankton abundance with moon phase overlaid, the ability to separate day from night observations, and a way to compare several lunar cycles side by side. She also needs the tool to show how much data backs each pattern, so a few sparse observations don’t read as a trend. 
She is curious and detail-oriented but has no scientific or programming background, so she works only through the interface and needs plain-language labels.


### Zooey Plankton, Ocean Conservationist/Drag Queen
3. Zooey Plankton is a drag queen and an ocean conservation advocate, who loves devouring the phytoplankton runway. She also has a computer science background.
She is building a personal app that works as a tracker, calendar, and ocean health monitor, so she can update her routines according to “current” events.
To feed it recent glider observations, she needs a documented way to pull data programmatically, either an API or a downloadable export (CSV or JSON), with a data dictionary covering units, timestamps, and locations. She also needs to know how often the data updates, which measurements carry quality flags, and what attribution the data requires. 
She is comfortable with code and would rather read documentation than click through a dashboard.


### Nico, Surfer
4. Nico is an avid surfer who plans his sessions and trips around ocean conditions. 
He wants to know how El Niño and La Niña years change the water he surfs in, including temperature shifts, plankton blooms, and the odd glowing night. 
He needs to compare the same region and season across several years, filtered or colored by climate phase, with a plain-language note on what each pattern means for gear, water clarity, and bloom risk. He also needs the tool to show where glider coverage is thin, so he doesn’t treat a gap as a calm season. 
He has strong intuition about the ocean but no data background, so he works only through the interface.


### Namor, K'uk'ulkan (The Feathered Serpent God)
5. Namor (Marvel Cinamatic Universe) is the ruler of an underwater kingdom and is responsible for the health of the waters his people depend on. 
He wants to know whether phytoplankton and zooplankton levels across his territory are changing, so he can catch bloom crashes, harmful blooms, or shifts that surface-world activity might be causing. 
He needs a map of his territory with trends over time, a way to flag readings that fall outside the normal range, and clear marking of areas where glider coverage is thin. 
He has deep knowledge of the ocean but is not a data person, so he works only through the interface and needs plain-language labels.


### Carter, Policy Analyst
6. Carter is a policy analyst who briefs decision-makers on ocean and coastal issues. 
He wants to cite credible glider observations of plankton and ocean conditions when supporting climate-related policy proposals. 
He needs a simple summary view with a few clear charts, plain-language captions, one-click export of figures for slides and reports, and a visible data source and date range he can cite. He also needs the tool to state how much data backs each trend, so opponents can’t dismiss his claims over a thin record. 
He is comfortable with policy documents and basic charts but has no programming background, so he works only through the interface.


### Dr. Ellis, Marine Biologist
7. Dr. Ellis is a marine biologist in Alaska who studies how zooplankton distributions affect the fish, seabirds, and whales that feed on them. 
She wants to see zooplankton and environmental data from glider missions, both during a deployment (to decide whether to adjust the glider’s path or sampling) and afterward (to analyze patterns by season, year, and depth). 
She needs depth-resolved views along the glider’s track, not just a map, plus overlays of temperature, salinity, and other measured variables, filters for time of day and depth, and quality flags on every measurement. She also needs raw data export with sensor and processing details so she can verify results and run her own analysis in R or Python. 
She is an expert in her field and comfortable with code, but she will not trust a view that hides how the data was processed.


### Marcus, Commercial Fisherman
8. Marcus is a commercial fisherman who works from a boat offshore for days at a time. 
He wants to know where plankton-rich or unusually warm or cold water sits relative to where he plans to fish, since that can hint at where forage fish and the species he targets are gathering. 
He needs a view that loads on a slow satellite or spotty cell connection, reads clearly on a phone or tablet in sunlight, and shows the latest glider observations with their date and how old they are. He also needs coverage gaps marked plainly, so he doesn’t treat an unsampled area as empty water. 
He knows the water from experience but has no data background, so he works only through the interface and has little time to dig.

### Hank, Glider Operator
9. Hank is an experienced glider operator. He wants to check that the glider has enough battery to continue the deployment. He wants a desktop or mobile interface that displays the most recent battery level and battery level over time of the deployment. He is the director of operations for the lab and has many years of experience working with gliders, so he knows what battery levels are reasonable to maintain operation.

### Sally, Glider Operator
10. Sally is a new glider operator. She wants to check that the glider has enough battery to continue the deployment. She wants a desktop or mobile interface that displays the most recent battery level and either hints for reasonable battery levels or directly displays a warning/danger indicator if levels are too low. She is a recently hired operator and working on her first glider deployment.

### George, Principal Investigator
11. George is a principal investigator. He wants to see if there are any interesting features from environmental/biological data that the glider should revisit to increase sampling resolution in those areas. He wants a desktop or mobile interface that allows for the display of multiple environmental/biological parameters over time of the deployment. He is the director of operations for the lab and has many years of experience working with gliders and familiar with the multiple dashboards serving glider data.

### John, Principal Investigator
12. John is a principal investigator focused on active acoustics. He wants to monitor the quality of active acoustic data during deployment and view previous deployment data. He wants a desktop dashboard that can serve current and previous deployment active acoustic data with a time slider for viewing subsets of the timeseries data. He is a domain expert on active acoustics with some familiarity of glider operations.

### Jack, Curious Undergrad
13. Jack is an undergraduate student interested in data from autonomous platforms. He wants to retrieve data from past deployments to perform his own exploratory data analysis. He wants a desktop dashboard with a map to understand where the deployment trajectories were, a time slider to select data from a time range of interest, and the ability to download data from the selected range in csv or netCDF format. He is unfamiliar with data portals, dashboards, and underwater gliders.

### Mark, Software Developer
14. Mark is a software developer who added image processing to the plankton camera on an underwater glider. He wants to be able to add optical data products to the desktop or mobile interface.  He wants a way to easily pull data and integrate new plots or figures to the dashboard in a way that won’t mess up the other modules. He is familiar with data visualizations and using dashboards but new to programming them.

### Dr. Rivera, ER MD & Public Health Specialist
15. Dr. Rivera is an emergency physician and public health specialist who has noticed more open water swimmers arriving in the ER with gastrointestinal, skin, or respiratory illness. She wants to look back at conditions in the water around the dates and places where swimmers got sick, to generate hypotheses about what changed, such as a bloom, a temperature anomaly, or a freshwater runoff signal. She needs to select a date range and area, see temperature, salinity, and chlorophyll or other biological measurements for that window, and export the data with sensor and quality details to share with epidemiologists and water quality agencies. She also needs coverage gaps shown clearly, so a lack of data is never read as clean water. She is an expert in medicine and epidemiology but has no oceanography or programming background, and she understands this tool describes water conditions, not the cause of illness

### Josh, Fisher man
Josh is a fisher man. He want to know where the fish at for him to catch. He need the data of where the fish is at with the latest data from the bio sensor, but in a way of easy showing bio mass and location. No coding skills nor high level of computer using, are accessing the data from webstie from phone.

### Tim, Oceanographers
Tim is a Oceanographers, he wants to learn the temperature changes of the ocean. He needs as much data point from the temperature sensor as possible. Fancy dashboard are not needed, need all the raw data from the glider. He is good with coding and experience with data processing.

### Allen, glider pilot
Allen is a glider pilot. He is using the dashboard to see the if the sensor are working properly and the how much battery left in the glider. He need a dashboard that don't need to control but showing the data on it and refresh it automatically. He has experience with pilot the glider, but less skills in processing the data. 

### Sarah marine ecologist
Sarah is a marine ecologist who studies zooplankton. She wants to watch the biological and environmental data while the glider is out at sea so she can decide where it should go next. She needs to see zooplankton biomass next to temperature and chlorophyll on the same screen, so she can spot patches and fronts quickly and tell the pilot to send the glider back to an interesting area. She is an expert in ocean science and comfortable reading scientific plots, but does not want to write code in the middle of a mission.

### Linda, high school science teacher
Linda is a high school science teacher. She wants to show her students what an underwater robot is doing in the ocean right now. She needs a simple map of the glider's path, its current location, and easy-to-read charts with plain explanations and no jargon. She has basic computer skills, no coding experience, and uses the website on a classroom projector.

### David, head of the reasearch lab
David is the head of the research lab that runs the glider program. He wants a quick summary of how each mission is going so he can report progress to funders and plan future deployments. He needs an overview page showing how long the glider has been out, how far it has traveled, whether it is healthy, and a few key highlights from the data. He has a strong science background but is very busy, so he only wants the big picture and doesn't want to dig through detailed plots.

### Emma, diver
Emma is a weekend scuba diver. She wants to check how warm the water is and how clear it might be before she plans a dive trip. She needs a simple view of the latest water temperature at different depths and the chlorophyll level, since lots of plankton can make the water cloudy. She is comfortable using apps on her phone but has no background in ocean science or coding.

### Jake, surder
Jake is a surfer who goes out almost every morning. He wants to know the water temperature near the coast so he can pick the right wetsuit before leaving home. He needs one quick number or a simple color scale that shows if the water is cold or warm today, without having to read any charts. He has basic phone skills and wants to get the answer in a few seconds.

### Marcus, whale watching fan
Marcus is a kayaker and whale-watching fan. He has heard that whales follow zooplankton because it is their food, and he wants to see where large patches of zooplankton are showing up. He needs a map that highlights areas with high zooplankton biomass so he can guess where whales might be feeding. He enjoys learning about the ocean but has no coding skills and uses the website on his phone or tablet.
