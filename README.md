# Introduction
This was part of my proposal to the IEEE Empower a Billion Lives Competition in 2018. A Secondary (voltage) controller was also developed to go along with this.

The goal of the competition was to reach the next billion people who didn't have access to  electricity in the 21st Century.

This was part of a vision where Renewable Power produced in a village is optimised and delivered by offloading some components to RL based agents thereby reducing the need for complex Microgrid equipment.

# A Tertiary controller
* Here MADDPG is used to train 4 agents which try to optimise the demand at any instant of time (Demand Response)
* A custom environment is created here to simulate the load of a village
* Note: The time interval for tertiary control is quite large compared to Voltage control. Hence the step interval in the custom env is large


## Learnings
* Creating a custom environment due to lack of anything comarable in OpenAI Gym in 2018
* Training and optimising for the number of agents in MADDPG
