# Narrative-visualization
Interactive slideshow using d3.js

### About the Visualization

The visualiation shown is an Interactive Slideshow. User can view the full data and intrepret it based on the categories of vehciles for whihc the emission stuy was done

The visualization is based on a dataset from the Environment Protection Agency which contains horsepower, CO2 emission and vehicle type information vehicles manufactured in 2015.

### Scenes

There are three scenes in the narrative visualization. They follow the same template and layout for visual consistency. The visualization displays data consistentently with frame of height 510px, width 980px.The axes used in the plot were made in linear scale. The ticks used in the plot are uniform in size and color for entire visualization.The scenes were designed for smoot transitions wihout any isntance when the user gets disoriented. The first scene highlight the overall trend of the data, second shows the trend in the data being consistent based , and finally in scene 3 ask the user to reflect on this trend and perhaps consider it when making his next vehicle purchase.

### Annotations

Annotations are used highlight trends and gain further in-depth insigts and conclusions from the data. They have been made bold and have unfirom font size across the entire narrative visualization. Visaulization's scene 1 has anntation to highlight the general trend in the data that increase in horsepower will increase the carbon dioxide emission. Visaulization's scene 2 allows for mouseover the data to see the trends for Cars, Trucks or both. Visaulization's scene 3 has annotation which helps user interact and make a decision about future purchase decisions. 

### Parameters

Parameters are used to engage the user in the narrative visualization and further explore the data. The parameter used in this visualization is the categorical variable vehicle "type". The user has the ability to examine the data of one vehicle type at a time (Car, Truck or SUV) by mousing over any data point belonging to that particular vehicle type. This allows the user to gain more information about the relationship between horsepower and CO2 output, not only as an overall trend, but based on vehicle type as well. 

The current state is controlled by this parameter vehicle "type". When mousing over a data point belonging to a particular vehicle type, the current state changes and the data points belonging to the other vehicle types are set to opacity = 0.01. When mousing off the data point the current state changes again and opacity for all data points for all vehicle types returns to 1.

### Triggers

Triggers are utilized in two ways for this visualization.

The buttons along the top of the visualization container are triggers to change scenes. The buttons are labelled such that their functions are made to be obvious: "Viz-Scene 1", "Viz-Scene 2", "Viz-Scene-3" and "About the Visualizaton".

The user event of clicking one of these buttons changes the current state of the visualization by changing the visualization scene. Affordance is used such that the button that represents the current state of the visualization is displayed with an increased brightness. When the user mouses over the other buttons they become temporarily highlighted which indicates to the user that they may be clicked. Upon clicking a button this triggers a change to the corresponding scene being displayed.

Triggers are also utilized with the data points.

The user event of "mouse over" a data point changes the current state of the chart by applying an opacity of 0.01 to all data not part of the vehicle type that is currently moused over. The user event of "mouse off" changes the current state of the chart by returning the opacity of all data points back to 1. This capability for the user event associated with data mouse over is communicated with an annotation.


### References

Tutorial for building a stepper page used as reference:
http://vallandingham.me/stepper_steps.html


