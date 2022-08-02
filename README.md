[Research Track II](https://corsi.unige.it/en/off.f/2022/ins/60236)<br>
**Analyser:** [Ankur Kohli](https://github.com/ankurkohli007)<br>
[M.Sc Robotics Engineering](https://corsi.unige.it/corsi/10635)<br>
[University of Genoa (UniGe)](https://unige.it/en)<br>
**Supervisor:** [Prof. Carmine Tommaso Recchiuto](https://rubrica.unige.it/personale/UkNDWV1r)

# Statistical Analysis for Python Robotics Simulator

***Python Robotics Simulator: This is a simple, portable robot simulator. The objective of this assignemt is to develop a Python code script which is capable to behave correctly inside of a given environment. Additionally, this simulator is developed by [Studnet Robotics](https://studentrobotics.org/)***

## Abstarct

This analysis is about the **statistically analysis** to determine the superiority between two distinct algorithms (my algorithm and professor's algorithm) in accomplishing a specific task. The specific task in this case is a simulation of a robot in a ***pygame*** environment with the objective of completing laps through the designed track (circuit), while occasionally moving silver tokens through its lifting mechanism to a spot behind it, as it makes its way through the circuit. For this analysis, ***Jupyter Notebook*** is used to compute the statistical analysis of the behaviour of two different algorithms for the first assignment of ***Research Track I*** based on ***Python Robotics Simulator***.

## Introduction

Statistical analysis is the collection and interpretation of data in order to uncover patterns and trends. It is a component of data analytics. Statistical analysis can be used in situations like gathering research interpretations, statistical modeling or designing surveys and studies.

In this, the statistical analysis of two implementations (my code and professor code) are going to be studied. The main objective of this analysis is to drive a robot autonomously by grasping the \textit{\textbf{silver token}}, and putting them behind itself, and last but not the least robot should avoids the obstacles, which are \textit{\textbf{golden tokens}}. In figure below, the map of the circuit has been presented as well as the robot itself and tokens are shown.

![alt text](ImagesResults/circuit.png) 

## Description of the analysis

Given the python environment as shown in figure above, the two algorithms – One given by the professor, and one from a student (Which I will refer to as Professor Code and My Code respectively) - compared pass instructions to the robot in the simulated environment to move thought the circuit while grabbing and dropping silver tokens and avoiding golden tokens. A clear indication of performance – considering all environment variables remain constant (token positions and robot starting point) will be the time factor. A measure of the time between each silver token grabbing and releasing events can be measured, as they distinctively define the amount of distance travelled due to their being equally spaced within the environment, and the efficiency of task execution, and overall time taken to lap the circuit. For this experiment, we will consider the results with a level of significant of and above 5%.

For the analysis, clone [my code](https://github.com/ankurkohli007/Research_Track_I_Assignment_1.git) and [professor code](https://github.com/CarmineD8/python_simulator.git). After clonning the given repository, I prepared 4 ".txt" file named as "collision.txt", "collisionp.txt", "trajectory.txt", and "trajectoryp.txt". 

After that, I prepared the Jupyter Code for the Statistical Analysis. For the jupyter code [click here](StatisticsAnalysis.ipynb).

This Jupyter Code will describe the my approach towards the analysis.

## Results

For the results click on the given [link](StatisticalAnalysisReport_Ankur_Kohli.pdf). 

## Conclusion and Improvements

The main objective of this statistical part of the project is to find particular differences between my code and professor code that “guide” the robot inside the environment. I have taken lots of data, making sure to have the same condition during the acquisition, since I know results are non-deterministic, so I wanted to decrease the inconsistencies due to the performances of the PC (even if there are).

There are main improvements that I came up with, which are:

* Provide better interface for sequentially setting the goal
* Develop more structured code
