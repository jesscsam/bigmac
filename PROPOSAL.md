# Programming project

Universiteit van Amsterdam 
Minor programmeren, Programming project
Jessica Sam, 10752498

## Problem statement
The rise in online communication has led to way lower transaction costs, and enables a larger number of people to be involved in illegal activities, including online sex work. Social media platforms, as a result, often function as a springboard for criminal activity. 
But how do you recognize individuals who are likely to enter into online sex trade? 

## Solution
A machine learning model by Kostakos et al.* has predicted the risk factor of 28,832 users of a specific adult online forum. The resulting dataset includes gender, age, sexual orientation, sexual polarity, amount of activity and interaction (chat time, comments, advertisements, amount of profile pictures, and number of offline meetings attended) and, of course, based on those variables, that individual's risk factor (high risk, low risk, no risk, unknown risk)

To bring insight into this data and thus into what individuals are more likely to enter online sex trade, I will create several visualisations: 
- Sun burst: the inner ring shows gender, middle ring sexual orientation, outer ring sexual polarity.
- Pie chart: when clicked on a sub category in the sunburst, a pie chart shows the distribution of risk factors within that group. This can be specified even further by selecting an age group through a drop-down menu. 
- Bar chart: when clicked on a gender in the sunburst, a bar chart shows the amount of interaction that each age group has with the forum. The user can select which type of interaction through a drop-down menu (comments, chat time etc.)

If I have the time, I might create:
- A network diagram showing friend groups within the forum, where the color of each node (person) shows their risk. That might show whether people with more friends on the forum have a higher, or lower risk to enter into online sex work.

## Sketch

![My project sketch](https://github.com/jesscsam/programmeerproject/blob/master/pictures/sketchklein.jpg)

As you can see, the sunburst diagram is the main visualisation. It will be larger when not hand-drawn. ;-) 
On page load (when the user has nothing selected yet), the pie chart will show the distribution of risk for all users and the bar chart will show the amount of comments posted per age group. 

## Prerequisites

### Data source
All data is from one dataset publicly available on [Kaggle](https://www.kaggle.com/panoskostakos/online-sex-work). The data was collected at one moment in time and comprises 28,832 users of an online adult forum. 

### External sources
For this project, I will need the following external resources: 
- D3, version 5
- The D3-tip library for tooltips in the bar chart 

