# Markov Decision Process

This repository contains the code implementation my project for my Artificial Intelligence course at Universidad Carlos III de Madrid.


Implementing Markov Decision Process to control the traffic flow of an intersection with 3 directions and 3 traffic lights

We face the following problem: 
We need to control the traffic on an intersection that can be approached by 3 directions (North, West and South). Each traffic light has two states: green or red. An operator must select every 20 seconds which of the three traffic lights to turn green: the other two will automatically turn red. Sensors measure the level of traffic in each direction prior to the intersection. The values can be: High or Low. 
We also know that when a traffic light is green, the level of traffic can only decrease or  stay the same (only increasing in some exceptions). When the traffic light is red, the level of traffic can only increase or stay the same.

The objective is to obtain an optimal policy or strategy to make the most efficient decision when it comes to knowing which  traffic light to put in green in order to control the traffic flow. We propose the design of  an automaton using a Markov Decision Process. Organising the problem as an MDP allows us to represent each possible traffic situation as a state ( for instance High;Low;High would mean High traffic on the North direction, Low traffic on the East and High traffic on the West ) and apply a decision/action (i.g turn the West traffic light green) for each of those states/situations. This way and by executing the Bellman Equations algorithm that we developed in a Python program we will be able to obtain the optimal policy for each different traffic case.
