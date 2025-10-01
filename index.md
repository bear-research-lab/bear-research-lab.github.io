---
layout: page
title: BEAR Lab @ SKKU
subtitle: Bioinspired Embodied AI and Robotics Lab
permalink: /
---


<div class="jumbotron-main">
  <div class="lab-photo"></div>
</div>

# Welcome to the BEAR Lab 🐻
At the **Bioinspired Embodied AI and Robotics (BEAR) Lab**, we envision a world where robots and AI serve as agents that support and empower people.

---
## News 
- **[03/2026]** The Bioinspired Embodied AI and Robotics (BEAR) Lab at SKKU is established!

---
<!-- ===== Research Areas (Cards with Nested Sub-Cards) ===== -->
## Research Areas
We build robots that help people and the methods that make them possible.  
For details, see our <a href="/projects/">Projects</a> page.

<style>
  /* ---- Card Grid ---- */
  .research-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 18px;
    margin: 18px 0 8px;
  }
  @media (min-width: 720px) {
    .research-grid { grid-template-columns: repeat(2, 1fr); }
  }
  @media (min-width: 1100px) {
    .research-grid { grid-template-columns: repeat(3, 1fr); }
  }

  /* ---- Top-level Cards ---- */
  .research-card {
    background: var(--card, #fff);
    border: 1px solid var(--border, #e6e6e6);
    border-radius: 16px;
    box-shadow: var(--shadow, 0 2px 6px rgba(0,0,0,.05));
    overflow: hidden;
    display: flex;
    flex-direction: column;
  }
  .research-card__body {
    padding: 16px 16px 8px 16px;
  }
  .research-card h3 {
    margin: 0 0 8px 0;
    font-size: 1.15rem;
  }
  .research-card p {
    margin: 0 0 10px 0;
    color: var(--muted, #666);
    line-height: 1.5;
  }

  /* ---- Sub-card Grid ---- */
  .subgrid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 10px;
    padding: 0 16px 16px 16px;
  }
  @media (min-width: 720px) {
    .subgrid { grid-template-columns: 1fr; } /* keep tall cards readable */
  }

  /* ---- Sub-cards ---- */
  .subcard {
    background: var(--pill-bg, #fafafa);
    border: 1px solid var(--pill-border, #d8d8d8);
    border-radius: 12px;
    overflow: hidden;
    display: grid;
    grid-template-columns: 92px 1fr;  /* image left, text right */
    gap: 12px;
    align-items: center;
    transition: transform .06s ease;
  }
  .subcard:hover { transform: translateY(-2px); }

  .subcard img {
    width: 100%;
    height: 82px;
    object-fit: cover;
    display: block;
  }
  .subcard__img {
    aspect-ratio: 1 / 1; /* keeps square-ish thumbnails if height not fixed */
    background: #eee;
  }
  .subcard__body {
    padding: 10px 12px 10px 0;
  }
  .subcard__title {
    margin: 0 0 4px 0;
    font-weight: 600;
    font-size: 0.98rem;
    color: var(--text, #222);
  }
  .subcard__text {
    margin: 0;
    font-size: 0.92rem;
    color: var(--muted, #666);
  }
</style>

<div class="research-grid">

  <!-- 1) Robotics for Human Assistance -->
  <section class="research-card">
    <div class="research-card__body">
      <h3>Robotics for Human Assistance</h3>
      <p>
        Systems that support daily living, rehabilitation, and healthcare—with
        an emphasis on usability, safety, and reliability in real environments.
      </p>
    </div>

    <div class="subgrid">
      <!-- Wearable Robots -->
      <article class="subcard">
        <div class="subcard__img">
          <img src="/assets/img/research/wearable_robots.webp" alt="Wearable robots thumbnail">
        </div>
        <div class="subcard__body">
          <h4 class="subcard__title">Wearable Robots</h4>
          <p class="subcard__text">Soft/underactuated hands, tendon-driven gloves, and assistive exosystems for mobility and manipulation.</p>
        </div>
      </article>

      <!-- Home-Assistive Robots -->
      <article class="subcard">
        <div class="subcard__img">
          <img src="/assets/img/research/home_assist.webp" alt="Home-assistive robots thumbnail">
        </div>
        <div class="subcard__body">
          <h4 class="subcard__title">Home-Assistive Robots</h4>
          <p class="subcard__text">Domestic manipulation and user-in-the-loop autonomy to enhance independence and quality of life.</p>
        </div>
      </article>
    </div>
  </section>

  <!-- 2) Bioinspired Design -->
  <section class="research-card">
    <div class="research-card__body">
      <h3>Bioinspired Design</h3>
      <p>
        From nature’s “good-enough” solutions to algorithmic pipelines that make bioinspiration
        systematic, testable, and scalable.
      </p>
    </div>

    <div class="subgrid">
      <!-- Evolutionary Robot Design -->
      <article class="subcard">
        <div class="subcard__img">
          <img src="/assets/img/research/evolutionary_design.webp" alt="Evolutionary robot design thumbnail">
        </div>
        <div class="subcard__body">
          <h4 class="subcard__title">Evolutionary Robot Design</h4>
          <p class="subcard__text">Search over morphologies and routings using evolutionary operators and constraint-aware objectives.</p>
        </div>
      </article>

      <!-- Bio-Mechanism Abstraction -->
      <article class="subcard">
        <div class="subcard__img">
          <img src="/assets/img/research/bio_principles.webp" alt="Bio-mechanism abstraction thumbnail">
        </div>
        <div class="subcard__body">
          <h4 class="subcard__title">Bio-Mechanism Abstraction</h4>
          <p class="subcard__text">Extracting reusable tendon, linkage, and surface-contact principles from biological exemplars.</p>
        </div>
      </article>
    </div>
  </section>

  <!-- 3) AI for Embodied Robotics -->
  <section class="research-card">
    <div class="research-card__body">
      <h3>AI for Embodied Robotics</h3>
      <p>
        Generative and physical AI for co-designing body & control and adapting to uncertain, real-world environments.
      </p>
    </div>

    <div class="subgrid">
      <!-- Generative Co-Design -->
      <article class="subcard">
        <div class="subcard__img">
          <img src="/assets/img/research/generative_codesign.webp" alt="Generative co-design thumbnail">
        </div>
        <div class="subcard__body">
          <h4 class="subcard__title">Generative Co-Design</h4>
          <p class="subcard__text">Diffusion/LLM pipelines that jointly optimize morphology, materials, and controllers.</p>
        </div>
      </article>

      <!-- Learning for Control -->
      <article class="subcard">
        <div class="subcard__img">
          <img src="/assets/img/research/learning_control.webp" alt="Learning for control thumbnail">
        </div>
        <div class="subcard__body">
          <h4 class="subcard__title">Learning for Control</h4>
          <p class="subcard__text">Model-based + RL policies, simulation-to-real transfer, and constraint-aware adaptation.</p>
        </div>
      </article>
    </div>
  </section>

</div>

<!-- Call-to-action (kept centered) -->
<div align="center" style="margin-top: 18px;"><strong>
If you are interested in joining our lab,<br>
please check out the <a href="/opportunities/">Opportunities</a> page for more information.
</strong></div>


<!-- ## Research Areas
For more details, see our [Projects](/projects/) page.

1. **Robotics for Human Assistance**  
   We design and build robots that support people in daily life, rehabilitation, and healthcare. Current directions include **wearable robots** for mobility and rehabilitation, as well as **home-assistive robots** that enhance independence and quality of life.

2. **Bioinspired Design**  
   Nature often provides elegant “local minimum” solutions to complex engineering challenges. We aim to make bioinspiration more **systematic and computational**, leveraging algorithms and simulations to uncover design principles from biology.

3. **AI for Embodied Robotics**  
   Artificial intelligence—particularly **generative AI and physical AI**—offers new ways to design and control robots. We study how AI can:  
   - **Design robots** (shaping morphology and mechanisms)  
   - **Control robots** (adapting to uncertain, real-world environments)  
   - **Co-design body and brain** simultaneously, optimizing robots for task-specific performance. -->

---
<div align="center"><strong>
If you are interested in joining our lab,<br>
please check out the <a href="/opportunities/">Opportunities</a> page for more information.
</strong></div>