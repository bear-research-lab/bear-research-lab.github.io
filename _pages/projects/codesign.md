---
layout: page
title: ""
permalink: /projects/codesign/
---

### 1. Why are we interested in computational robot co-design?
Designing a robot can be understood as **optimizing its design for a given task**. How do humans do this optimization today? Usually, designers rely on **experience** and **intuition**. However, this process is often **time-consuming**, **expensive**, and **sub-optimal**.

Several successful robot design approaches include:

1. Bio-inspired design: This approach draws inspiration from nature to design robots that mimic the behavior and structure of biological organisms. Examples include robotic fish, birds, and insects. This approach builds on how living creatures have evolved to adapt to their environments.

2. Soft robotics: This approach focuses on designing robots with soft and flexible materials. The use of soft materials allows for more adaptable interaction with the external environment. This adaptability works especially well in unstructured environments. For example, a robot foot covered with soft material can adapt to different terrains and obstacles without requiring precise control or sensing. 

3. Modular robotics: This approach involves designing robots using modular components that can be easily reconfigured and combined to create different robot designs. This approach reduces the dimensionality of the design space and allows for more efficient exploration of this design space. 

Although these approaches have been very successful, they leave open questions: "How should the robot be controlled?", "Will the resulting design actually work well once a controller is added?", and "Can we find the best design without considering how it will be controlled?"

These questions lead us to the concept of **robot co-design**, which involves the simultaneous optimization of both the robot's physical embodiment (body) and its control strategy (brain). We can also consider the robot co-design as a *bioinspired robot design* approach, since in nature, the body and brain of animals have co-evolved to adapt to their environment and perform specific tasks effectively.

So, how can we achieve robot co-design? Should we wait thousands of years for evolution? Or should we rely on a huge amount of human effort to design and optimize the robot body and controller iteratively?

To answer these questions, consider recent trends in AI and robotics. AI has advanced significantly, especially in generative models and reinforcement learning. In robotics, physics simulation and optimization algorithms have also improved dramatically.

Motivated by these advances, our lab focuses on the **computational robot co-design** approach, which leverages the power of AI, optimization, and simulation to automate and scale the robot design process.

---

### 2. What have we done so far?

#### 2.1. Robot Co-Design through Diffusion-Based Generative Models
**Project Lead:** Tsun-Hsuan Wang

**Collaborators:** Juntian Zheng, Pingchuan Ma, Yilun Du, Byungchul Kim, Andrew Spielberg, Joshua B. Tenenbaum, Chuang Gan, Daniela Rus

**Conference:** NeurIPS 2023 (Oral)

**Links**: [Paper](https://bear-research-lab.github.io/assets/pub/Neurips_DBOT.pdf), [Video](https://www.youtube.com/watch?v=LSzasdvD3Ss)


##### Motivation  
Diffusion models can generate diverse 3D shapes, but shapes that look plausible are not necessarily robots that *work well*. We asked whether a generative model could be guided by **physics simulation** to produce soft robots that perform a given task.  

##### Method  
- A pretrained 3D diffusion model generates candidate robot shapes, which are converted into **soft robot bodies** (geometry, actuators, and stiffness).  
- Each robot is evaluated in a **differentiable physics simulator** on the target task.  
- The performance signal is fed back to the diffusion process, steering generation toward better-performing designs, while body and control are optimized together (**co-design**).  

##### Results  
- Generated soft robots for diverse tasks such as locomotion, manipulation, and passive dynamics.  
- Outperformed baseline design approaches in simulation.  
- A generated design was **fabricated and tested in the real world**.  

##### Contribution  
- Showed that large generative models can be combined with physics simulation for **task-driven robot design**, beyond generating shapes that only look plausible.  
- Received an **oral presentation** at NeurIPS 2023.  

---

#### 2.2. Jumping Robot Design through Evolution-Inspired Approach  
**Project Lead:** Byungchul Kim  

**Collaborators:** Tsun-Hsuan Wang, Daniela Rus  

**Conference:** ICRA 2025

**Links**: [Paper](https://bear-research-lab.github.io/assets/pub/2025_ICRA_GENJUMP.pdf), [Video](https://www.youtube.com/watch?v=g7mGls8oHj4)

##### Motivation  
Traditional gradient-based optimization, such as differentiable simulation, may struggle with the **high dimensionality and non-linearity of robot shape design**. We sought a method that could explore this vast space more broadly and discover **unconventional but effective morphologies**.  

##### Method  
We designed an **evolution-inspired design loop**:  
1. **Generation** – An initial population of ~500 candidate robots with random shapes is generated by a diffusion-based generative model.
2. **Evaluation** – Each design is tested in a physics simulator on the jumping and landing tasks.  
3. **Selection** – Only the **top 12 performers** are chosen based on metrics such as jump height and landing stability.  
4. **Reproduction** – These survivors guide the creation of the next generation of candidates.  

This cycle is repeated across **five generations**.  

##### Results  
- **+41% improvement** in jumping height.  
- **+210% improvement** in landing success rate.  
- Generation of **novel, non-intuitive morphologies** that outperform initial designs.  

##### Contribution  
This work builds on our previous work (Section 2.1), with two key differences:
- Human prior designs guide the initial generation. This makes the final designs fully manufacturable with 3D printing and off-the-shelf components, and significantly reduces the design search space, enabling more efficient exploration.
- It focuses on a specific task (jumping and landing) with clear performance metrics, allowing more targeted optimization and evaluation of designs.

---

#### 2.3. What's next? 
Our work so far has focused on robot shape design using diffusion-based generative models. Next, we plan to explore a richer design space that includes robot morphology (shape, structure, material), control (controller, policy), and fabrication (manufacturing process, cost), using more advanced AI, optimization, and simulation techniques.

---
This page was written with the help of a large language model (LLM).