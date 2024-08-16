# Models and Analyses for Robots’ Messy Reality

From self-driving cars to factory and surgical robots, robotic and autonomous systems are transforming the ways that humans travel, manufacture, and perform their jobs. Broadly, robotics autonomous systems (RAS) sense, process, and (often autonomously) interact with the physical world, usually to assist or automate some human task. As such systems grow more prevalent, assuring that they operate safely, with acceptable risk to humans and the environment becomes ever more important.

Unfortunately, applying the extant analysis techniques and tools that reason about the correctness of RAS remains challenging for at least three key high-level reasons. First, in practice, most RAS are implemented via large, complex, distributed, and sophisticated code bases decoupled from models where analyses can be exercised. Second, the physical environments in which RAS operate are so complex that checking for whole system properties is largely performed through simulation. Even the best simulator, however, just approximates the real environment, causing what is commonly known as the simulation-reality gap where failures that manifest in simulation are not always even possible in the field, and vice versa. Third, robot systems evolve in diverse ways that exacerbate the code-model decoupling and the simulation-reality gap issues, and make it difficult to understand the impact of and validate changes.

This proposal’s goal is to enable the development of domain-specific analyses techniques to detect RAS faults by inferring useful models from code artifacts and real world inputs, even in the presence of changes. Our key insights are two-fold. First, although robotics code is often messy and complex, model- relevant behavior is typically implemented via a subset of APIs and configuration files with clearly-specifiable semantics. Second, field data encode key spatial-temporal physical constraints imposed by the real world which provides hints on how to steer simulation to reduce the gap with reality. We propose to leverage these insights to effectively lift useful models from real code to detect compositional faults, identify and construct simulation scenarios that capture constraints imposed by the real world, and inform and validate the evolution of robotic systems.
Crucially, our collaboration brings together experts in software engineering and robotics to bear domain- specific modeling and analysis techniques to state-of-the-art RAS.

# Investigators

+ [Sebastian Elbaum](www.virginia.edu/~se4ja) ([UVA](virginia.edu)  [LESSLAB](https://less-lab-uva.github.io/)), 
+ [Claire Le Guoes](https://clairelegoues.com/) (CMU [Squares Lab](https://squareslab.github.io/)), 
+ [Changliu Liu](https://www.cs.cmu.edu/~cliu6/) (CMU)

# Sponsor: 

NSF, Collaborative Research: SHF: Medium: Models and Analyses for Robots’ Messy Reality, Grant #

# Relevant Papers

+ Software Engineering for Robotics: Future Research Directions; Report from the 2023 Workshop on Software Engineering for Robotics
Claire Le Goues, Sebastian Elbaum, David Anthony, Z. Berkay Celik, Mauricio Castillo-Effe, Nikolaus Correll, Pooyan Jamshidi, Morgan Quigley , Trenton Tabor, Qi Zhu.  https://arxiv.org/abs/2401.12317

+ Canelas, P., Tabor, T., Ore, J.-P., Fonseca, A., Le Goues, C., & Timperley, C. S. (2024). Is it a Bug? Understanding Physical Unit Mismatches in Robot Software. International Conference on Robotics and Automation, 1–7.

+ Dürschmid, T., Timperley, C. S., Garlan, D., & Le Goues, C. (2024). ROSInfer: Statically Inferring Behavioral Component Models for ROS-based Robotics Systems. Proceedings of the IEEE/ACM 46th International Conference on Software Engineering. https://doi.org/10.1145/3597503.3639206
