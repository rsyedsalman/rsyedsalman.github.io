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


Simple Moving Average = `(A1 + A2 + …… + An) / n`
where, A = Average in period n, n  = Number of time period

![Moving_Average](/assets/img/MovingAv.png){: .center_wide}

I found some great results with above 90% accuracy, for a distance covered in 20 seconds.

The figure on the below left shows what distance were covered by the user every 2.5s.
The figure on the right indicates total distance (m) during a time period of 20 seconds. The graph depicts an increased trend for distance traveled beginning at 0 seconds.

<div id="image-table">
    <table>
	    <tr>
    	    <td style="padding:10px">
        	    <img src="/assets/img/RTES_StepDist.png" width="350"/>
      	    </td>
            <td style="padding:10px">
            	<img src="/assets/img/RTES_20s.png" width="350"/>
            </td>
            </tr>
    </table>
</div>

You can find the full code for the project, here [Here](https://github.com/srsyed2/RealTimeEmbeddedSystems)

<br />

---

<br />

#### Recycling Stations in NYC

<p>New York residents are estimated to produce approximately 12,000 tonnes of waste everyday. Each year a significant amount of the tax has to be allocated for collection, disposal and sending of waste to landfills. Landfills are responsible for 36% of all methane emissions in the US, one of the most potent contributors to global warming. In the light of the exorbitant and long term environmental and economical effects, New York City has declared a 20 year Solid Waste Management Plan to reduce its waste disposal.</p>

<p>Currently, recycling stations are situated around the different boroughs of New York City. In this case study, I examined the distribution of different types recycle stations across New York City's 5 boroughs and attempt to design a strategy for where to add more recycle stations in general and recommendations for deployment of specific waste recycling stations to fulfill inadequacies in each boroughs.</p>

<u>Dataset</u>

The dataset used for this case study is a compilation of multiple datasets consisting data on different types of recycling stations from *The City of New York, Department of Sanitation (DSNY)*.

The dataset consists of: 1. Name of the site of the recycling station, 2. Borough the station is situated at, 3. Specific address in text, 4. Longitude and Latitude coordinates of the station,    5. Type of recycling station.

1. [https://data.cityofnewyork.us/Environment/Electronics-Drop-Off-Locations-in-NYC/wshr-5vic](https://data.cityofnewyork.us/Environment/Electronics-Drop-Off-Locations-in-NYC/wshr-5vic)

2. [https://data.cityofnewyork.us/Environment/Public-Recycling-Bins/sxx4-xhzg](https://data.cityofnewyork.us/Environment/Public-Recycling-Bins/sxx4-xhzg)

3. [https://data.cityofnewyork.us/Environment/Food-Scrap-Drop-Off-Locations-in-NYC-Map-/qfn2-4jea](https://data.cityofnewyork.us/Environment/Food-Scrap-Drop-Off-Locations-in-NYC-Map-/qfn2-4jea)

The compiled dataset can be found here: [Dataset](shorturl.at/xyJMQ)

<p> By figuring out the ratio of recycling station to the population of each borough, we can find the disparity in the distribution. The two figures below shows the distrubitions of Recycle Bins normalized to population and the distribution of different types of recycle bins around all boroughs of New York City </p>

<div id="image-table">
    <table>
	    <tr>
    	    <td style="padding:10px">
        	    <img src="/assets/img/RecBin_PopToBin.png" width="310"/>
      	    </td>
            <td style="padding:10px">
            	<img src="/assets/img/RecBin_TypeDis.png" width="310"/>
            </td>
        </tr>
    </table>
</div>


I created an user interactive interface based on Dash Plotly where people can hover on different areas of NYC and find where current recycle bins are located.

<div style="display:flex">
     <div style="flex:1;padding-right:10px;">
          <img src="/assets/img/RecBin_Disp.png" width="800"/>
     </div>
</div>

You can find the full code for the project, [Here](https://github.com/srsyed2/RecycleStationsNYC/blob/main/Final_Project_SyedSalmanN13866121.ipynb)

<br />

---

<br />

#### ProxIPS

ProxIPS is a RSSI based indoor positioning system based on Bluetooth Low Energy (BLE). ProxIPS is different from other distance proximity algorithms because it uses ML (k-nearest neighbour) instead of traditional triangulation procedures.
ProxIPS is a full solution because it includes both a web-based application for corporate user analytics and a mobile phone app for customers who want to get user-specific content streams.

<div style="display:flex">
     <div style="flex:1;padding-right:10px;">
          <img src="/assets/img/ProxIPS_Arch.png" width="480"/>
     </div>
	<div style="flex:1;padding-right:10px;">
          <img src="/assets/img/ProxIPSdash.png" width="480"/>
     </div>
</div>

The Minister of Energy, Science, and Technology of Malaysia presented ProxIPS with the award for third place in the Grand Challenges Competition 2019.

<div style="display:flex">
     <div style="flex:1;padding-right:10px;">
          <img src="/assets/img/proxips4.jpeg" width="700"/>
     </div>
</div>
<br/>

<iframe width="560" height="315" src="https://www.youtube.com/embed/s0d7O8f3QRE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br />

---

<br />

#### Microfluidic based Dielectrophoretic Cell Sorter for Real-time Cancer Detection

<p> Microfluidic based Dielectrophoresis (DEP) is a label-free, non-invasive method used for biological cell sorting by many researchers. This method is concisely utilized in the segregation of cancerous cells from normal, healthy cells which canhelp in the diagnosis in real-time. With the aid of dielectrophoretic field-flow-fractionation (DEP-FFF) using a low voltage of 10 Volts, the device was successful in separating a total of 48 samples of Circulating Tumor Cells (CTCs) from a total mixture sample of 52, at a rate of 87% in 118 seconds.</p>
<p> The complete study was simulated on *COMSOL Multiphysics 5.3A* through which the comparison study on characterization of the designs in terms of electric potential,pressure, fluid flow of the particles and separation was carried out.</p>

<div style="display:flex">
	 <div style="flex:1;padding-right:10px;">
          <img src="/assets/img/oneS.jpeg" width="500"/>
     </div>
     <div style="flex:1;padding-right:10px;">
          <img src="/assets/img/graph.PNG" width="450"/>
     </div>
</div>
<br />

<iframe width="580" height="325" src="https://www.youtube.com/embed/BWHUgXOqAms" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<br />

---

<br />
