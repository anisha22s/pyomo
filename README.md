# pyomo
#Task Scheduling

In this repository, I have solved an optimization question related to task scheduling using Pyomo. The problem involves allocating parts to different machine setups in order to minimize the cost while ensuring that all parts are produced within a given time frame.

##Problem Description

As the operations manager of a manufacturing plant, I have a robot-operated machine that can run in four different setups, namely A, B, C, and D. Each setup has a specific cost per hour and a maximum number of hours it can run before maintenance is required. Additionally, there are four parts that need to be completed within the next two weeks, and each setup has a different production rate for each part.

##Problem Formulation

To solve this problem, I formulated it as a Linear Programming (LP) problem. Here are the key components of the formulation:

###Decision Variables
Allocate variables: I defined a binary decision variable for each part and setup combination to represent whether a part is allocated to a specific setup or not.
###Objective Function
Cost minimization: The objective is to minimize the total cost, which is the sum of the costs per hour for each setup multiplied by the allocated hours for that setup.
###Constraints
Production requirement: I ensured that all parts are produced by enforcing that each part must be allocated to at least one setup.
Setup availability: I limited the total hours allocated to each setup based on its maximum availability.
Production rate: I incorporated the production rate constraints to ensure that each part is produced within the estimated hours for each setup.
Solution in Pyomo

To solve this problem, I implemented the LP formulation using Pyomo, a Python-based optimization modeling library. The code for solving the problem can be found in the respective files.

Please note that the provided solution is for illustrative purposes and may require adaptation for specific use cases.

##Conclusion

By solving the task scheduling problem using Pyomo, I have demonstrated how to allocate parts to different setups while minimizing the cost. This optimization approach helps optimize resource utilization and production efficiency.
