---
title: "The Curious Use Case of Load Shedding"
date: 2019-03-20
tags: ["use case", "learn"]
author: "Reuben Honigwachs"
draft: false
banner: "img/blog/load-shedding-candle-light.JPG"
---
South Africa is facing a power crisis for a [very long time now](https://en.wikipedia.org/wiki/2007-2019_South_African_energy_crisis). This is compensated for by **_load shedding_**, where the energy provider Eskom switches off sectors of the national grid. In March 2019 we have seen an extended period of _Stage 4_ whereby an area will be without power for three periods of 2.5 hrs per day.

This has a detrimental impact on daily life and citizen's basic needs. Even more so on IT infrastructure and IoT data back-haul. In this severe crisis of state capture, corruption, mismanagement, and plain incompetence on a national scale, on a positive note, as a TTN community network we were able to experience an interesting use case. 

Firstly, for a spatial understanding of how load shedding works, here the areas blacked out Wed March 20 08:00-16:30 in Cape Town Metro ([map](http://resource.capetown.gov.za/documentcentre/Documents/Procedures%2c%20guidelines%20and%20regulations/Load_Shedding_All_Areas_Schedule_and_Map.pdf)). Please note that Stellenbosch has it's own schedule not shown here.
 
![Load shedding map animatied](/img/blog/load-shedding-areas.gif)

You probably know this already, but to reiterate:
 
* **When a TTN node sends out a message it can be received by _multiple_ gateways and will be delivered to the network**. 

In effect this means a TTN node can utilise gateways that are outside of its immediate area. Far distant, in fact. Here a simple battery-powered node in Khayelitsha. It's within reach of four TTN gateways outside of its own area, at an average distance of 23km. 

![TTN node Khayelitsha](/img/blog/load-shedding-khayelitsha.png)

The Cape Town Metro TTN gateway infrastructure which is run by the community can hereby overcome obstacles put in its way by load shedding. Using LoRaWAN's **long distance** properties and TTN's **redundance by design**. Additionally, being **low power**, it allows for even more applications in this scenario... e.g. operating nodes entirely off-grid.  

### Appeal

> Running infrastructure volunteer-based and as a community of individuals has proven itself _challenging_ in the last year. For network coverage to become denser and more redundant we need strong partners with access to high sites, back-haul infrastructure, or funding. Please join us in our efforts to strengthen The Things Network, a free and open IoT network. 

<small>This article is licensed under CC BY-SA 3.0. Photo [Dittymathew](https://commons.wikimedia.org/wiki/File:Candle_Light.JPG).</small>

