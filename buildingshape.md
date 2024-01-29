---
layout: page
title: Building Shape & Circulation 
subtitle: Chosen building shape and circulation of residents   
---
As discussed in the previous page, the final building shape was chosen based on the scenario F (see an image below). In the image you also see the programs color coordinated. 

![Text_test](assets/img/final_shape.png)

After all the functions are placed in the building, the circulation of the residents in the building is looked into. For this, we have created two elevator shafts in the building. These elevator shafts are placed according to the best position. The best position is defined as the elevator reach a maximal height, whilst crossing as many functions as possible. 

### Elevator Shafts 

To define the optimal positions for the elevators all the ground points of the building are selected. For each ground point the vertical height and the number of functions above the ground point are calculated. Then, the different ground points are scored and the ground point with the best scores is chosen for the location of one of the elevators. To get the spot for the second elevator points that are close to the first elevator are deleted and the place with the highest score after the deletion is chosen for the second elevator. Next, the elevator ground points are extended into the height. To generate a hallway between the two elevators points which are close to the outside of the building are given a higher cost than points in the middle of the floor, this means that the hallway will want to generate in the middle of the building. Finally, the shortest path between the two elevators is calculated to best represent the circulation between the two elevators in relation to the programs. 

Below is a depiction of the created workflow: 
![Text_test](assets/img/elevator_workflow.png)

The following elevator shaft placement and shortest path resulted from this: 
![Text_test](assets/gif/hallway_generation.gif)

### Circulation in the building 

According to the elevator and program placement, the different user experiences and scenarios are visualized. Each type of resident moves differently throughout the building. 

Below is an flow diagram of how the elderly (independent and assisted) move through the building: 

![Text_test](assets/img/elderly_circulation.png)

Below is an flow diagram of how the students (starters and studios) move through the building: 

![Text_test](assets/img/student_circulation.png)

Below is an flow diagram of how the starters move through the building: 

![Text_test](assets/img/starter_circulation.png)


 




