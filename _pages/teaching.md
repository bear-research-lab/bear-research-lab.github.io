---
layout: page
permalink: /teaching/
---

Courses taught by Prof. Byungchul Kim at SKKU.

### 1. Introduction to Robotics
<div class="project-card">
  <div class="project-text">
    <p>This course covers the fundamentals of robot manipulators:</p>
    <ul>
      <li><strong>Forward and inverse kinematics</strong> using the <strong>product of exponentials (PoE)</strong> formula</li>
      <li>How to <strong>design a robot</strong></li>
      <li>How to <strong>run robot simulations</strong></li>
    </ul>
    <p><strong>Final project: RB5 pipetting.</strong> In teams of two, students program a
    Rainbow Robotics RB5 cobot in a <strong>MuJoCo</strong> simulation to do a pipetting task.
    The project has three parts, each building on the one before:</p>
    <ul>
      <li><strong>Forward kinematics</strong>: derived by hand in NumPy and checked against MuJoCo</li>
      <li><strong>Inverse kinematics</strong>: the Jacobian and an IK solver that move the robot through the task</li>
      <li><strong>Pipetting hand</strong>: a hand design that grasps the pipette, presses its bulb, and returns it
      reliably despite errors in the pipette holder's position, evaluated in simulation and designed in 3D CAD</li>
    </ul>
    <p>The reference video below shows what each part looks like when it works.</p>
    <div class="video-embed">
      <iframe src="https://www.youtube.com/embed/VN9uyTWR938"
              title="Reference output for the Introduction to Robotics Final Project: a RB5 cobot doing a pipetting task"
              allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
    <a href="https://github.com/bear-research-lab/Class_IR" class="btn" target="_blank" rel="noopener">Final Project (GitHub)</a>
    <a href="https://www.youtube.com/watch?v=VN9uyTWR938" class="btn" target="_blank" rel="noopener">Reference Video (YouTube)</a>
  </div>
</div>

### 2. Robot System and Application
<div class="project-card">
  <div class="project-text">
    <p>This course covers how to build and control real robot hardware:</p>
    <ul>
      <li><a href="https://www.youtube.com/playlist?list=PLRPVUUEpZCYk" target="_blank" rel="noopener">Designing PCBs</a> (KiCad lecture videos on YouTube)</li>
      <li><strong>CAN</strong> &amp; <strong>CANopen</strong></li>
      <li>Motor basics</li>
      <li>Transmissions, including tendon transmission</li>
    </ul>
    <p>In parallel, we explore the enabling technologies and fields of robotics by reviewing the <em>Springer Handbook of Robotics</em>. Our chapter reviews are collected on the Notion page below.</p>
    <a href="https://thankful-argument-4e8.notion.site/Robotics-Handbook-Study-fe695bc491ec830fa9ec016c120cd4f5" class="btn" target="_blank" rel="noopener">Robotics Handbook Study (Notion)</a>
  </div>
</div>

### 3. AI for Robot Control
<div class="project-card">
  <div class="project-text">
    <p>This course covers how robots learn to act:</p>
    <ul>
      <li><strong>Imitation learning</strong></li>
      <li><strong>Reinforcement learning</strong>, including <strong>PPO</strong> and <strong>TRPO</strong></li>
      <li><strong>Robot foundation models</strong>, such as <strong>Vision-Language-Action (VLA)</strong> models</li>
    </ul>
  </div>
</div>
