---
layout: page
title: Facade definition  
subtitle: Facade definition and Material Choice   
---
### Grouping of Facades
To place the facades, we have defined three groups of programs: housing, parking, and others. *Housing* concerns the elderly, student, and starter accommodations. *Parking* concerns the bike, as well as car parking. *Others* concerns all other functions. 

For the housing, the sun analysis  is considered as a factor whether to place a balcony or a window. If there is more sun, a balcony is placed, if less, a window. The balcony requirements for the shared students are a total of 50, for the assisted elderly 80, for the independent elderly 120, and for the starters 200 (see figure below). Hence, there are a total of 450 balconies. To ensure that the sound reaching the housing dwellings is minimized, the type of material and the profile is considered. To secure the privacy of the residents, the type of material and the orientation is taken into consideration. 

To warrant that the parking maintains a level of ventilation, sound absorption and remains discreet, the material and the profile are considered. 

For the other programs, glass material is considered to make the programs more accessible and visible for the residents and users of the programs. 

Please see the image below for a schematic overview of the facade definition:

![Text_test](assets/img/facadedef2.png)

### Types of Facades 

To assign the facade with different elements, three main classes are created: (1) walls, (2) balconies, and (3) roofs. To classify the *walls*, there are walls with windows, sound walls, glass walls, car park walls with holes for ventilation, and green walls. Depending on the type and purpose of a function, the walls are assigned accordingly. The *balconies* can either be located in a corner, on or in somethings, and are placed accordingly. The *roofs* are either classed as a green roof, or a floor, also depending on the height of the building. 

See the image below for the different types of facade classes. 

![Text_test](assets/img/facadelement.png)

### Placement of Facade Elements 

The placement of the facades is based on the exposure of each facade element to sunlight. For this, each function is grown by function (as seen in the growing algorithm). Based on the sun analysis, the facade points are sorted based on their sunlight exposure. Each type of program (especially the housing functions) have a set requirement of balconies and windows, which is considered in the for the minimal assignment of balconies and windows. The best sun points are then chosen and assigned to balconies and windows. If the other points belong to a housing program, they are assigned to walls. All other points are assigned a different facade element dependent on the type of program the belong to. For example, the facade elements belong to the parking areas, a wall with holes is assigned.  

See the below image for an overview of the strategy used to assign facade elements based on sun position. 

![Text_test](assets/img/facade_strategy.png)

The types of material used can be seen in the following render of the building. In the render all types of building materials can be seen. Noteably, the communal space and other communal gathering points (such as the cafeteria) have glass facades enabling a clear flow between indoor and outdoor areas. Further, a lot of green walls and and green roofs were made use of. 

![Text_test](assets/img/facade_vis.png)