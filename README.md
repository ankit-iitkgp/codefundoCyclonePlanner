# codefundoCyclonePlanner
Overview

Hey! My project focuses on Tropical Cyclone Disaster which is caused due to Monsoon. In this I am going to make an app which takes input of current weather conditions and combine it with past statistics and few other interesting geographical factors to generate 3-level of alert. Subsequently, these level of alerts will help the user to to take measures to combat them.

Goals

To predict good result on the basis of past statistics using good machine learning method.
To combine it with present condition and produce different levels of warning.
To make a responsive app which could guide the user to take measures beforehand. 

Specifications

As this application is for Tropical Cyclone, its prime users to would be from the region which are mostly affected by it like Eastern Coastal region and Gujarat( relating only for India). So, the app will work on 3 parameters -

1) First, of all it will take the past year’s same location degree of severity as inputs. Apply recursively modelled linear regression algorithm(if get a better algorithm, then apply that). For example it will take past 20 year’s data. Then it will apply linear regression on 11th year by using first 10 years data. Then compare it with original data and include the error factor. Do the same thing for 12th year and so on to come to a very close estimate for present.

2) Now, this parameter includes two factors. First, the present weather conditions of the location. Tropical cyclones happens due to these developments-
Creation of low pressure area & high speed wind flowing over it
There is source of moist area derived from tropical oceans with sea surface temperature near to excess of 27 C.
Low wind shear allowing the storm clouds to rise vertically to high levels and coriolis force causing depression.
	By, taking these development and their distance from location, we can form the present case. Also taking the following into consideration-

<img src="brazil.png"> 
<img src="India.png>

These are the average precipitation of Brazil and India( both are due to monsoon). It can be noticed both are exactly opposite to each other and these are no coincidence. So, taking south american early month’s monsoon reports will also help us setting the present opinion for our location.

3) Next, we will form different level of alerts combining the above 2 parameters.  Each parameter will measured, say in 3 point scale - RED( extremely severe ), Yellow( little severe) , Green ( not at all severe ). For example, in the 2nd parameter, if the wind speed is less than 118 km/hr, its Green. If it is between 119-221 km/hr, Yellow and if it is beyond 221 Red. 

Next, if both are red, there will be highest level alert. If one of them is red, this will of middle level alert and if both are yellow there will be a minor alert.( If just 1 yellow and other is green, it would just be a warning). There will be a planner in the app. It will advice user for their travel plan, kind of items to shop and also a reminder for things like filling the water and electricity resources when alert is in middle zone. Other safety measures will be incorporated in the planner.

Moreover, for future recommendation only 1st parameter will be taken into account. So, all the future plannings could be done according to it. Also, by changing the location user can plan their travel plan and routes to be taken.
