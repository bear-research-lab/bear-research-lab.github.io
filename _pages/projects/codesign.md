---
layout: page
title: ""
permalink: /projects/codesign/
---

### 1. Why we are interested in computational robot co-design? 
Designing robots could be understood as a process of **optimizing robot design for the given task**. Following question could be: How does human optimize the robot design for a given task? One possible answer could be, the human often rely on **experience** and **intuition** to design robots. However, this process is often **time-consuming**, **expensive**, and **sub-optimal**.

Several successful robot design frameworks include:

1. Bio-inspired design: This approach draws inspiration from nature to design robots that mimic the behavior and structure of biological organisms. Examples include robotic fish, birds, and insects. In this approach, we often rely on how the creatures in nature have evolved to adapt to their environment.

2. Soft robotics: This approach focuses on designing robots with soft and flexible materials. The use of soft materials allows for more adaptable interaction with the external environment. This adaptability magically works well in unstructured environments. Assume a robot foot covered with soft materials, it can adapt to different terrains and obstacles without requiring precise control or sensing. 

3. Modular robotics: This approach involves designing robots using modular components that can be easily reconfigured and combined to create different robot designs. This approach reduces the dimensionality of the design space and allows for more efficent exploration of this design space. 

Although these approaches have shown great success in designing robots, following question could be "how can we control the robot?" or "how can we guarantee the obtained robot design will work appropriately considering the robot control?" or "can we find the best robot design without considering how it will be controlled?"

These questions lead us to the concept of **robot co-design**, which involves the simultaneous optimization of both the robot's physical embodiment (body) and its control strategy (brain). We can also consider the robot co-design as a *bioinspired robot design* approach, since in nature, the body and brain of animals have co-evolved to adapt to their environment and perform specific tasks effectively.

So, how can we achieve the robot co-design? Should we wait for thousands of years of evolution? Or should we rely on huge amount of human effort to design and optimize the robot body and controller iteratively?

To answer these questions, let's think about the current trend of AI and robot technology. We have seen significant advances in AI, especially in the field of generative models and reinforcement learning. From the robot technology perspective, we have seen significant advances in physics simulation and optimization algorithms. 

Form this hint, our lab will focus on the **computational robot co-design** approach, which leverages the power of AI, optimization, and simulation to automate and scale the robot design process.

---

### 2. What have we done so far?

#### 2.1. Jumping robot design through evolutionary approach
[Paper link](https://bear-research-lab.github.io/assets/pub/2025_ICRA_GENJUMP.pdf)
Our approach can be described as an evolution-inspired design loop, similar to natural selection. The first generation of robots is created with random shape (with zero guidance). Each robot is then evaluated in a physics simulator to assess its performance on the jumping/landing tasks. 

Based on their performance, only the top-peroforming robots (12 out of 500) are selected to "reproduce" and generate the next generation of robots. This reproduction process is done for five generations, showing 41% improvement in jumping height and 210% improvement in landing success rate. 

Our work demonstrates a new paradigm for robot design. Instead of relying on gradient signals propagated through differentiable simulators, which become difficult to scale for complex, high-dimensional shapes, we adopt a generative selection–optimization framework. In each generation, a large pool of candidate morphologies is produced, evaluated in physics simulation, and down-selected to the most promising designs. These survivors then guide the creation of subsequent generations. This process, inspired by evolutionary search, enables us to explore the design space broadly and discover unconventional robot morphologies that are unlikely to emerge from purely gradient-based optimization. By combining generative AI with selective refinement, our approach circumvents the limitations of direct shape differentiation while still leveraging simulation feedback to drive performance-oriented design.


#### 2.2. Robot co-design through diffusion based generative model
[Paper link](https://bear-research-lab.github.io/assets/pub/Neurips_DBOT.pdf)
The advance in generative models, espe

#### 2.3. What's next? 
Although we have made interesting results in computational robot co-design, our current works have only focused on robot shape design using diffusion-based generative models. However, we can explore more complex robot design space including robot morphology (shape, structure, material), robot control (controller, policy), and robot fabrication (manufacturing process, cost). Let's explore more complex robot design space using more advanced AI, optimization, and simulation techniques.

---
This page was written with the help of large language model (LLM).