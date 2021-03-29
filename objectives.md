---
layout: page
title: Objectives
permalink: objectives.html
order: 1
---

By combining our respective and distinct expertise in Software Engineering and Resilient
Software on one side and AI-based Software Testing on the other side, we will address the
following challenges for resilient software:

# Challenge #1 Utilizing observation data for assessing resilience under varying conditions

There are a large number of varying conditions to operate an AS and it is impossible to
explore exhaustively these conditions in test environments. However, the observations made
on a given AS can be exploited to enhance the testing.
We plan to follow two directions: First, we leverage *Metamorphic Testing* [1] to address the
oracle problem of AS under varying conditions: How to test a program P, if for a given test
input x, we cannot exactly specify the expected outcome P(x)? A metamorphic relation
defines changes over both inputs and outputs, i.e. the AS environment and its behavior, and
the accepted variations in behavior. Recent works applied machine learning to select the
most likely fault-revealing metamorphic relations for a given test input [2]. We will follow the
general idea to identify meaningful metamorphic relations by mining input and output data. 
*Multimorphic testing* [6] will also be considered for assessing the effectiveness of performance test suites of software systems.
By analogy with mutation testing, the core idea of Multimorphic testing is to leverage the typical configurability of these systems, and to check whether it makes any difference in the outcome of the tests: i.e., are some tests able to "kill" underperforming system configurations?
Second, we can *amplify* the test inputs through the observation of how the system reacts. For
example, some execution traces of the system can show that some zones of the programs
have been neglected in terms of test coverage. This allows us to generate test scenarios in
simulation and the physical world that assess the limits of resilience. Hence an idea is to
either synthesize new test inputs or to expand an existing test input. In both cases, we 
believe AI has a role to play to exploit the output data and improve the testing resilience of
the system.

# Challenge #2 Digital twins for continuous improvement of resilient autonomous/smart systems

*Digital Twins (DT)* [3, 5] have emerged since the beginning of this millennium to better
support the management of systems based on (real-time) data collected in different parts of
the operating systems. The very essence of this new generation of systems requires
maximizing the use of data collected throughout the system life cycle, which needs to be
processed, organized and structured to help manage and improve the systems. Among
others, DTs are expected to improve the resilience of systems through online monitoring that
enables continuous improvements. However, their development, maintenance, and evolution
still face major challenges [4].
To help in the assimilation of the data, and to feed back the DT with relevant
recommendations and assistants supporting the continuous improvement of systems, we
propose to explore the integration of predictive models in the design and implementation of
DT. In particular, we are interested in i) exploring the required modeling languages for DTs,
ii) data-driven learning of digital twin models from historical and live data, iii) proposing an
architectural framework for implementing DTs that brings together data and models, and iv)
managing possible sources of uncertainty.

# Challenge #3 Resilient Autonomous Systems in the Digital and Physical World

For a thorough evaluation of the methods for testing and improving resilient autonomous
systems, it is necessary to make the transfer to the actual systems both in the digital world,
i.e. precise simulations, and the physical world, i.e. on the AS hardware.
In our joint work, we will utilize the available systems at both partners, e.g., a mobile rover
robot from DiverSE and a lightweight collaborative industrial robot from Simula (specifically, Aion Robotics R1: https://www.aionrobotics.com/r1-ardupilot-edition
Universal Robots UR3: https://www.universal-robots.com/products/ur3-robot/)
We aim to perform case studies on these systems to allow not only the evaluation of resilience using
digital twins, but also to assess the transferability of the methods onto the physical hardware.

[1] T. Y. Chen, F.-C. Kuo, H. Liu, P.-L. Poon, D. Towey, T. H. Tse, and Z. Q. Zhou. 2018.
Metamorphic testing: A review of challenges and opportunities. ACM Computing Surveys 51,
1 (2018), 4:1–4:27.
[2] Adaptive metamorphic testing with contextual bandits. H. Spieker, A. Gotlieb. Journal of
Systems and Software 165: 110574, 2020.
[3] Grieves M., Vickers J. (2017) Digital Twin: Mitigating Unpredictable, Undesirable
Emergent Behavior in Complex Systems. In: Transdisciplinary Perspectives on Complex
Systems. Springer, Cham.
[4] S. Ali and T. Yue, Handling Uncertainties in Cyber-Physical Systems during Their
Operations with Digital Twins, Presented at the Fifth Workshop on Monitoring and Testing of
Cyber-Physical Systems (MT-CPS) co-located with CPS-IoT Week, 2020.
[5] Francis Bordeleau, Benoit Combemale, Romina Eramo, Mark van den Brand, Manuel
Wimmer. Towards Model-Driven Digital Twin Engineering: Current Opportunities and Future
Challenges. ICSMM 2020 - International Conference on Systems Modelling and
Management, Jun 2020, Bergen, Norway.
[6] Paul Temple, Mathieu Acher, Jean-Marc Jézéquel. Empirical Assessment of Multimorphic
Testing. IEEE Transactions on Software Engineering (2020)
