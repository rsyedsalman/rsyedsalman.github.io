---
layout: page
title: Projects
---


<br />

#### Need For Speed Wearable Health Tracker

The objective of this project was to build a wearable speedometer which can calculate velocity by measuring angular velocities available
from the built-in gyroscope (L3GD20) in STM32F429 - without a GPS.

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


<!-- .png
![Drag System](../img/drag_system.png){: .center : width="80%" !important}
![Apogee Prediction](../img/apogee.png){: .center : width="40%"}
 -->



