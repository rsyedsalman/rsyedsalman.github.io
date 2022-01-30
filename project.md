---
layout: page
title: Projects
---

<br/>

#### Need For Speed Wearable Distance Tracker

<p> The objective of this project was to build a wearable speedometer which can calculate velocity by measuring angular velocities available
from the built-in gyroscope (L3GD20) in STM32F429 - without a GPS.</p>

Few of the mentionable features of the projects are: 1. Made a tailor made driver for the L3GD20 sensor. 2. SPI communication was used to read data from the sensor at a frequency of 2 Hz. 
3. For error reduction the Moving Average Filter was used, where the latest 5 sensor data were averaged out to correct the values.
4. Python was used to illustrate relevant data visualization.


Simple Moving Average = (A1 + A2 + …… + An) / n
where, A = Average in period n, n  = Number of time period

![Moving_Average](/assets/img/MovingAv.png){: .center_wide}

I found some great results with above 90% accuracy, for a distance covered in 20 seconds.

The figure below shows what distance were covered by the user every 2.5s.

![Step_Distance](/assets/img/RTES_StepDist.png){: .center_wide}

This graph indicates total distance (m) during a time period of 20 seconds. The graph depicts an increased trend for distance traveled beginning at 0 seconds.

![Final_Distance](/assets/img/RTES_20s.png){: .center_wide}

You can find the full code for the project, here [Here](https://github.com/srsyed2/RealTimeEmbeddedSystems)


#### Recycling Stations in NYC

New York residents are estimated to produce approximately 12,000 tonnes of waste everyday. Each year a significant amount of the tax has to be allocated for collection, disposal and sending of waste to landfills. Landfills are responsible for 36% of all methane emissions in the US, one of the most potent contributors to global warming. In the light of the exorbitant and long term environmental and economical effects, New York City has declared a 20 year Solid Waste Management Plan to reduce its waste disposal. Recycling is undoubtedly one of the most vital part in order to achieve this goal. Currently it is found out that residential recycling rate stands at around 18%. Currently, recycling stations are situated around the different boroughs of New York City. In this case study, I will examine the distribution of different types recycle stations across New York City's 5 boroughs and attempt to design a strategy for where to add more recycle stations in general and recommendations for deployment of specific waste recycling stations to fulfill inadequacies in each boroughs.



<!-- .png
![Drag System](../img/drag_system.png){: .center : width="80%" !important}
![Apogee Prediction](../img/apogee.png){: .center : width="40%"}
 -->



