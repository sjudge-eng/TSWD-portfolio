| [home page](https://sjudge-eng.github.io/TSWD-portfolio/) | [data viz examples](https://sjudge-eng.github.io/TSWD-portfolio/#data-viz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Outline
 
The title of this project could be boiled down to: Where in Pittsburgh does pedestrian safety risks appear highest and what street conditions seem to contribute to that?

At a high level, this project explores where pedestrian safety risks appear to be concentrated in Pittsburgh and attempts to identify what characteristics these high-risk locations share. Rather than trying to evaluate every aspect of walkability in the city, the project focuses on pedestrian-involved crash patterns and a small set of related street-condition variables, such as whether crashes occur at intersections, whether those intersections are signalized, posted speed limits, lighting conditions, and other roadway features. This narrower focus helps keep the project specific enough to tell a clear story while still using public data to investigate an important question.

The goal is not simply to map where crashes happen, but to show that pedestrian risk is not evenly distributed across the city. Instead, the project aims to look more closely at hotspots in and around Pittsburgh and explore what factors may be contributing to them. I also plan to incorporate time-based patterns over a longer period in order to see whether certain years, seasons, or time conditions help explain some of these hotspots. By combining crash records with a few street-condition measures, this project will help visualize where Pittsburgh appears to be more dangerous for pedestrians and what may be contributing to that pattern.

I selected this topic in part because of the contrast I have personally experienced as a pedestrian in Pittsburgh. Before moving here, I lived in Kirkland, Washington, where walking felt significantly safer and more predictable. Drivers there seemed more cautious and more respectful of pedestrian right-of-way. In Pittsburgh, my experience has often felt like the opposite. Drivers frequently move through crosswalks, ignore pedestrian priority, and create a more dangerous overall environment. While this project will focus primarily on pedestrian conditions in Pittsburgh, I may briefly reference Kirkland as a point of personal contrast to help explain why this question matters to me.

## Project Structure

Setup
Walking in Pittsburgh often feels unpredictable and unsafe, especially when compared to other places I have lived. That personal experience raises a larger question: does public crash data support the idea that pedestrians face heightened risk in certain parts of the city, and if so, where is that risk concentrated?

Conflict
This project begins with the idea that pedestrian risk is not evenly distributed across Pittsburgh. Some locations appear to experience more pedestrian-involved crashes than others, suggesting that certain street environments may create more dangerous conditions for pedestrians.

Investigation
To explore this pattern, the project will examine Pittsburgh pedestrian crash records in order to identify a small set of street-condition variables and general locations associated with heightened pedestrian risk. These variables may include factors such as intersection type, presence of signals, speed limit, and lighting conditions. As an extension of this analysis, I may also examine especially unusual or high-crash locations more closely to consider what physical or environmental factors may be contributing to those events.

Resolution
By identifying where pedestrian crash hotspots appear and what those locations have in common, the project has two main goals. First, it aims to show that pedestrian risk is shaped not only by driver behavior, but also by location-specific roadway and intersection conditions. Second, it aims to help readers better understand what kinds of environments appear to create greater pedestrian dangers.

Putting it all together
The final story will argue that pedestrian safety in Pittsburgh is not just a matter of individual driver behavior, nor simply a byproduct of general city conditions, but is closely tied to street design and location-based infrastructure. Looking at crash patterns can help reveal where these risks are concentrated and what factors may be contributing to them. The narrative will introduce the problem, use visualizations to make the conflict clear and understandable, investigate patterns in the data, and then bring those findings together into a cohesive explanation of where pedestrian risk appears highest in Pittsburgh.

## Initial sketches
> Post images of your anticipated data visualizations (sketches are fine). They should mimic aspects of your outline, and include elements of your story.  

Below is an initial rough sketch of my anticipated visualization. This map shows pedestrian crash density in Pittsburgh over a 5 year period (2020 -2024) and is intended to help identify areas where crash risk appears to be concentrated. In later versions of the project, I plan to refine this view and pair it with additional charts that help explain what street conditions may be associated with these hotspots.

![Rough sketch of pedestrian crash hotspots in Pittsburgh](pittsburgh_pedestrian_crash_sketch.png)

# The data

My primary data source for this project is the Western Pennsylvania Regional Data Center's cumulative Allegheny County crash dataset. I plan to use this as the main crash-record source because it provides a large, public dataset that can be filtered down to Pittsburgh and then narrowed further to pedestrian=involved crashes. Since the file is countywise rather than city-only, I will use the PennDOT data dictionary and minicipality code reference to isolate Pittsburgh records. In the PennDOT documentation, MUNICIPALITY is a coded field, and Pittsburgh City is listed as code 02301. The same documentation also confirms that PennDOT's public crash files are organized into multiple related tables and that the crash data comes from police crash reports, driver-reported forms, and calculated fields in PennDOT's crash analysis system.

After filtering the crash data to Pittsburgh, I plan to use the pedestrian and roadway fields to explore where pedestrian safety risks appear highest and what street conditions seem to be associated with those crashes. The PennDOT dictionary confirms that the data includes the pedestrian flag, as well as roadway and intersection variables that are useful for this project, including whether a crash took place at a signalized, stop-controlled, or unsignalized intersection. I expect to use this dataset mainly for mapping pedestrian crash hotspots and for comparing crashes across a small number of explanatory variables, such as intersection type, traffic control, and other potentially impacting conditions. The City of Pittsburgh also publicizes a crash dashboard that will serve as a secondary exploratory source that helps me potentially isolate patterns, confirm hotspot areas, and compare my own filtered results to current public-facing visualizations.

| Name | URL | Description |
|------|-----|-------------|
| Allegheny County Crash Data (WPRDC) | [Allegheny County Crash Data](https://data.wprdc.org/sk/dataset/allegheny-county-crash-data/resource/2c13021f-74a9-4289-a1e5-fe0472c89881?filters=) | Main crash dataset for the project. I will use this countywide crash file as the primary source, then filter it to Pittsburgh and pedestrian-involved crashes. |
| PennDOT Open Data Portal Data Dictionary (07-24) | [PennDOT Data Dictionary (PDF)](https://gis.penndot.gov/gishub/crashZip/Open%20Data%20Portal%20Data%20Dictionary%20(07-24).pdf) | Reference document used to interpret the crash dataset fields and codes, including pedestrian indicators, intersection variables, and the municipality code needed to isolate Pittsburgh records. |
| City of Pittsburgh Crash Data Dashboard | [Crash Data Dashboard](https://experience.arcgis.com/experience/854cc687784c461caef34a41f68f2b69) | Secondary exploratory source used to view public crash patterns, identify hotspots, and compare my filtered results with an official city dashboard. |

# Method and medium
For this project, I plan to complete the final as a digital, story-driven presentation that combines map-baed visualizations of Pittsburgh and supporting charts. I plan to use Tableau to clean, filter, and visualize crash data and potentially pair those visualizations with live photos from these hotspot areas to help build explanations into the visuals being shown to the readers. The goal is to create comparable, visualization-based, patterns across high-risk locations that call out intersection type, presence of signals, speed limit, and lighting conditions (to name a few). I then plan to use Shorthand to present this information as one cohesive narrative rather than just a group of standalone dashboards.

## References
[Allegheny County Crash Data](https://data.wprdc.org/sk/dataset/allegheny-county-crash-data/resource/2c13021f-74a9-4289-a1e5-fe0472c89881?filters=) 

[PennDOT Data Dictionary (PDF)](https://gis.penndot.gov/gishub/crashZip/Open%20Data%20Portal%20Data%20Dictionary%20(07-24).pdf)

[Crash Data Dashboard](https://experience.arcgis.com/experience/854cc687784c461caef34a41f68f2b69)

## AI acknowledgements
AI was involed in the initial ideation phase for this project. Initially, I had quite a bit of difficulty putting together a project-based topic that was not only interesting to me, but something that I could actually get the data for. After working with AI to land on this being the topic I wanted to pursue, I also turned to AI to specifically locate this dataset ([Allegheny County Crash Data](https://data.wprdc.org/sk/dataset/allegheny-county-crash-data/resource/2c13021f-74a9-4289-a1e5-fe0472c89881?filters=)). Finding usable, reliable, and long-running data has represented one of the most difficult aspects of this project thus far, so AI was very impactful in finding a very hidden, and incredibly useful, dataset on the Allegheny Regional Data Center webpage. 
