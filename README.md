# Open Research Projects

*None of my research will ever attempt to improve personal gambling payouts from sports betting. My goal is to understand the strategy that actually plays out and understand the underlying mechanisms.*

## The Hot Hand Project

The "hot hand" issue has been widely addressed in so many different sports with so many different approaches, assumptions, and conclusions.

It is clear that the null hypothesis - that there is no hot hand - corresponds to independence between shots. In other words, score a goal on this shot has nothing to do with whether you scored a goal in the previous shot (or shots). 

The central problem is this: What's the alternative hypothesis? Is it that scoring a goal on the previous shot increases the probability of making the current shot? Is it that the previous 2 shots, or three shots, etc. influence the current shot? Is there a corresponding "cold hand"?

The goal of this umbrella project is to provide a taxonomy and replication of existing methods, possibly contributing some of our own. This will be done across sports, and will require a thorough literature review (if published, we will start with a review paper) followed by re-implementation of all methods we find with all the data we find.

## General Projects

### Explain the Score: Explainable Machine Learning for predicting whether a team is leading
**Main Idea**: what exactly does a team do differently when it's leading compared to when it's tied or trailing? 
- The model will try and predict whether a team is leading (binary), or whether it's leading, tied, or trailing (multi-class classification). The methods will be machine learning agorithms that provide explanations for their predictions, allowing us to investigate what is different about leading versus trailing.
**Required Knowledge**: Data science or regression, basic R or python programming.

### Quantifying the changing graph structure of a moving team
**Main Idea**: For each frame of the game, and for each player, draw a line to their three closest teammates (or to all teammates within a given radius). Quantify the graph properties of this graph, including distances and angles to other players as well as standard graph theory metrics. Watch as these properties change throughout the game, using this to characterize a team's play style.
- Extension: Have a two-colour graph that characterizes both teams. 
**Required Knowledge**: Basic graph theory, good R or python programming.

### Development of a Spatially Referenced Network of Event Locations 
**Main Idea**: Teams record the locations of "Events" (passes, shots, penalties, etc.) during a game, and advanced statistical models try to characterize the spatial aspects of sports. A grid of $(x,y)$ locations results in many, many locations in which very little happens, and a small number of locations where lots of things happen. Instead of the exact locations, we could transform the playing area to a "web" or "mesh" of locations. This will reduce the number of locations required for spatial modelling without compromising the results. 
![232](Figs/SpatialNetwork%201.jpeg)
- Deliverable: An R or python package that converts coordinates to nodes in a mesh network. From there, models can simply use the nodes as a simplified set of coordinates. A technical report showing that models perform similarly on the simpler coordinates would be nice too.
- Future work: develop versions of spatial models that over a network, rather than a grid.
**Required Knowledge**: Good R or python programming, some data science or statistics.

### Record Breaking Achievements as Maximum Observed Values
**Main Idea:** In track and field, records represent the highest achievement thus far in that sport. In other words, it's the maximum observed value from a probability distribution; the largest deviation from the mean. By considering records over time, we can try to quantify the change in the mean of the distribution over time as well as the size of each deviation.
- If a record stands for 10 years, it was probably a very large deviation from the mean. If it only stands for 1 season, it was probably a small deviation.
- The underlying mean of the distribution might increase slowly over time, or it might have sudden jumps (e.g. from new techniques or materials, such as the Fosbury flop).
- Records might come from track and field (e.g. the 100m or high jump or marathon time), or they might come from team sports. However, team sports will be difficult to quantify since the deviation from the mean depends on teammates/opponents' deviation from the man or a changing mean. 
**Required Knowledge:** Strong probability and statistics background.
