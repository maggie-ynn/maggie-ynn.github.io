---
layout: page
title: Projects
permalink: /projects/
description: Making electrical risks measurable, traceable, and actionable.
nav: true
nav_order: 2
display_categories:
  [
    "3-Multi-modal Imaging & AI Inspection",
    "5-drone & advanced",
    "1-cable&grounding diagnostics",
    "4-smart substation& online monitoring",
  ]
horizontal: false
_styles: >
  .post-description,
  .projects-intro-note {
    font-size: 1.02rem;
    line-height: 1.75;
    color: var(--global-text-color-light);
    margin: 0;
  }

  .post-description {
    margin-bottom: 0.2rem;
  }

  .projects-intro-note + .projects-intro-note,
  .post-description + .projects-intro-note {
    color: var(--global-text-color-light);
    margin-top: 0.2rem;
    margin-bottom: 1.7rem;
  }

  .projects-capability-map {
    margin: 1.35rem 0 2.3rem;
    padding: 1.45rem 1.45rem 1.15rem;
    border: 1px solid var(--global-card-border-color);
    border-radius: 1.85rem;
    background:
      radial-gradient(circle at top, rgba(71, 119, 151, 0.12), transparent 42%),
      linear-gradient(145deg, rgba(255, 255, 255, 0.82), rgba(245, 241, 234, 0.92));
    box-shadow: var(--global-card-shadow-strong);
  }

  html[data-theme='dark'] .projects-capability-map {
    background:
      radial-gradient(circle at top, rgba(82, 135, 171, 0.18), transparent 42%),
      linear-gradient(145deg, rgba(15, 23, 33, 0.92), rgba(11, 17, 25, 0.98));
    box-shadow: var(--global-card-shadow-strong);
  }

  .projects-capability-map svg {
    display: block;
    width: 100%;
    height: auto;
  }

  .projects-map-caption {
    margin: 0 0 1rem;
    color: var(--global-text-color-light);
    font-size: 0.95rem;
    line-height: 1.72;
    letter-spacing: 0.01em;
  }

  .capability-core-label {
    fill: #0f172a;
  }

  .capability-core-subtitle {
    fill: rgba(71, 85, 105, 0.88);
  }

  html[data-theme='dark'] .capability-core-label {
    fill: #ffffff;
  }

  html[data-theme='dark'] .capability-core-subtitle {
    fill: rgba(226, 232, 240, 0.82);
  }

  .capability-node rect {
    fill: rgba(255, 255, 255, 0.84);
    stroke: rgba(90, 108, 124, 0.22);
    transition: fill 0.25s ease, stroke 0.25s ease, transform 0.25s ease;
  }

  html[data-theme='dark'] .capability-node rect {
    fill: rgba(16, 25, 35, 0.84);
    stroke: rgba(159, 202, 232, 0.2);
  }

  .capability-node text {
    fill: #0f172a;
    pointer-events: none;
  }

  html[data-theme='dark'] .capability-node text {
    fill: #e2e8f0;
  }

  .capability-node:hover rect,
  .capability-node.is-active rect {
    fill: rgba(29, 79, 115, 0.14);
    stroke: rgba(29, 79, 115, 0.7);
    transform: translateY(-2px);
  }

  .capability-node:hover .node-label,
  .capability-node.is-active .node-label {
    fill: #123b59;
  }

  html[data-theme='dark'] .capability-node:hover .node-label,
  html[data-theme='dark'] .capability-node.is-active .node-label {
    fill: #e9f5ff;
  }

  .flow {
    stroke: rgba(83, 97, 112, 0.42);
    stroke-width: 1.8;
    stroke-dasharray: 5;
    fill: none;
    animation: flow 1.4s linear infinite;
  }

  .flow.active {
    stroke: #d1aa58;
    stroke-width: 2.6;
    filter: drop-shadow(0 0 5px rgba(209, 170, 88, 0.55));
  }

  .particle {
    fill: #d1aa58;
    filter: drop-shadow(0 0 5px rgba(209, 170, 88, 0.72));
  }

  @keyframes flow {
    from { stroke-dashoffset: 0; }
    to { stroke-dashoffset: -20; }
  }

  .capability-core-card {
    fill: rgba(255, 255, 255, 0.92);
    stroke: rgba(90, 108, 124, 0.24);
    stroke-width: 1.2;
    filter: drop-shadow(0 10px 16px rgba(69, 87, 104, 0.12));
  }

  html[data-theme='dark'] .capability-core-card {
    fill: rgba(14, 22, 31, 0.94);
    stroke: rgba(159, 202, 232, 0.18);
    filter: drop-shadow(0 10px 18px rgba(0, 0, 0, 0.28));
  }

  .projects .project-category-block {
    transition: all 0.4s ease;
    margin-top: 2.2rem;
    margin-bottom: 1.45rem;
    padding: 1.3rem 1.35rem 1.3rem;
    border-left: 3px solid transparent;
    border: 1px solid var(--global-card-border-color);
    border-radius: 1.25rem;
    background: var(--global-card-bg-color);
    box-shadow: var(--global-card-shadow);
  }

  .projects .project-category-block.active {
    background: color-mix(in srgb, var(--global-card-bg-color) 84%, rgba(29, 79, 115, 0.08));
    border-left-color: #1d4f73;
    box-shadow: var(--global-card-shadow-strong);
  }

  .projects .category {
    margin-top: 0;
    margin-bottom: 0.85rem;
    color: var(--global-text-color);
    font-size: 1.64rem;
    font-weight: 700;
    line-height: 1.18;
    letter-spacing: -0.02em;
    text-transform: none;
  }

  .projects .category-subtitle {
    margin: 0 0 1.25rem;
    color: var(--global-text-color-light);
    font-size: 0.97rem;
    line-height: 1.72;
  }

  .projects .card-title {
    font-size: 0.98rem;
    line-height: 1.38;
    font-weight: 700;
  }

  .projects .card-text {
    font-size: 0.9rem;
    line-height: 1.62;
  }

  .autonomous-flow {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    flex-wrap: wrap;
    gap: 0.8rem;
    margin: -0.1rem 0 1.35rem;
  }

  .autonomous-flow-step {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 54px;
    padding: 0.85rem 1.15rem;
    border-radius: 16px;
    border: 1px solid color-mix(in srgb, var(--global-theme-color) 16%, var(--global-card-border-color) 84%);
    background: color-mix(in srgb, var(--global-card-bg-color) 92%, white 8%);
    color: var(--global-text-color);
    font-size: 0.93rem;
    font-weight: 600;
    line-height: 1.35;
    box-shadow: 0 10px 22px color-mix(in srgb, var(--global-theme-color) 8%, transparent 92%);
  }

  .autonomous-flow-arrow {
    color: var(--global-theme-color);
    font-size: 1.15rem;
    font-weight: 700;
    line-height: 1;
  }

  .workflow-hint {
    margin: -0.2rem 0 1.2rem;
    color: var(--global-theme-color);
    font-size: 0.9rem;
    font-weight: 600;
    letter-spacing: 0.01em;
  }

  .cable-group-heading {
    margin: 1.1rem 0 0.9rem;
    color: var(--global-text-color);
    font-size: 1rem;
    font-weight: 700;
    letter-spacing: 0.02em;
    text-transform: none;
  }

  .projects .card figure,
  .projects .card figure picture,
  .projects .card .card-img-top {
    width: 97%;
    margin-left: auto;
    margin-right: auto;
  }

  .cable-primary-grid .card-title {
    font-size: 1.04rem;
    font-weight: 800;
  }

  .cable-primary-grid .card-text {
    min-height: 4.7em;
  }

  .cable-primary-grid .card-img-top,
  .cable-primary-grid figure,
  .cable-primary-grid figure picture {
    aspect-ratio: 4 / 3;
    min-height: 240px;
  }

  .cable-secondary-grid .card-title {
    font-size: 0.95rem;
  }

  .cable-secondary-grid .card-text {
    font-size: 0.86rem;
    line-height: 1.52;
  }

  .cable-secondary-grid .card-img-top,
  .cable-secondary-grid figure,
  .cable-secondary-grid figure picture {
    aspect-ratio: 4 / 3;
    min-height: 200px;
  }

  html[data-theme='dark'] .projects .category {
    color: #ffffff;
  }

  html[data-theme='dark'] .projects .category-subtitle {
    color: rgba(226, 232, 240, 0.82);
  }

  html[data-theme='dark'] .autonomous-flow-step {
    background: color-mix(in srgb, var(--global-card-bg-color) 96%, #0f1720 4%);
  }

  html[data-theme='dark'] .cable-group-heading {
    color: #ffffff;
  }

  @media (max-width: 767px) {
    .projects-capability-map {
      padding: 1rem 0.8rem;
      border-radius: 1.2rem;
    }

    .projects-map-caption {
      font-size: 0.92rem;
    }

    .projects .project-category-block {
      padding: 0.75rem 0.75rem 0.85rem;
    }

    .projects .category {
      font-size: 1.45rem;
    }

    .projects .category-subtitle,
    .projects-intro-note,
    .post-description {
      font-size: 0.94rem;
    }

    .projects .card-title {
      font-size: 0.98rem;
    }

    .autonomous-flow {
      gap: 0.55rem;
    }

    .autonomous-flow-step {
      width: 100%;
    }

    .autonomous-flow-arrow {
      display: none;
    }

    .cable-primary-grid .card-img-top,
    .cable-primary-grid figure,
    .cable-primary-grid figure picture,
    .cable-secondary-grid .card-img-top,
    .cable-secondary-grid figure,
    .cable-secondary-grid figure picture {
      min-height: 0;
    }
  }
---

<!-- pages/projects.md -->
<p class="projects-intro-note">From live-line diagnostics to AI-driven inspection in power systems (10kV-500kV).</p>
<div class="projects-capability-map">
  <p class="projects-map-caption">Trace how capabilities connect into real engineering systems.<br>Click a node to explore the flow.</p>
  <svg viewBox="0 0 800 260" role="img" aria-label="Interactive project capability map">
    <line id="p-ai" class="flow path-ai" x1="348" y1="104" x2="280" y2="45"></line>
    <line id="p-drone" class="flow path-drone" x1="348" y1="156" x2="280" y2="205"></line>
    <line id="p-cable" class="flow path-cable" x1="452" y1="104" x2="520" y2="45"></line>
    <line id="p-substation" class="flow path-substation" x1="452" y1="156" x2="520" y2="205"></line>

    <rect x="330" y="92" width="140" height="76" rx="24" class="capability-core-card"></rect>
    <text x="400" y="122" text-anchor="middle" font-size="15.5" font-weight="700" class="capability-core-label">Maggie</text>
    <text x="400" y="144" text-anchor="middle" font-size="11.5" class="capability-core-subtitle">Power Systems Portfolio</text>

    <a href="#ai" class="capability-node" data-flow-target="ai">
      <rect x="80" y="20" width="200" height="50" rx="12"></rect>
      <text x="180" y="50" text-anchor="middle" class="node-label" font-size="13">Multi-modal</text>
    </a>

    <a href="#drone" class="capability-node" data-flow-target="drone">
      <rect x="80" y="180" width="200" height="50" rx="12"></rect>
      <text x="180" y="210" text-anchor="middle" class="node-label" font-size="13">Drone &amp; Robot</text>
    </a>

    <a href="#cable" class="capability-node" data-flow-target="cable">
      <rect x="520" y="20" width="200" height="50" rx="12"></rect>
      <text x="620" y="50" text-anchor="middle" class="node-label" font-size="13">Cable</text>
    </a>

    <a href="#substation" class="capability-node" data-flow-target="substation">
      <rect x="520" y="170" width="200" height="50" rx="12"></rect>
      <text x="620" y="200" text-anchor="middle" class="node-label" font-size="13">Smart Substation</text>
    </a>
    <circle id="flow-particle" class="particle" r="3.2" visibility="hidden"></circle>
  </svg>
</div>

<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  {% assign anchor_id = category | slugify %}
  {% assign category_label = category %}
  {% assign category_subtitle = "Selected project cases." %}
  {% case category %}
    {% when "1-cable&grounding diagnostics" %}
      {% assign anchor_id = "cable" %}
      {% assign category_label = "Cable Fault Diagnostics & Localization" %}
      {% assign category_subtitle = "Non-intrusive diagnostics and precise fault localization for energized cable systems and groundings." %}
    {% when "3-Multi-modal Imaging & AI Inspection" %}
      {% assign anchor_id = "ai" %}
      {% assign category_label = "Multi-modal Sensing & Diagnostics" %}
      {% assign category_subtitle = "Integrating IR, visual, acoustic, UHF and ultrasonic sensing for cross-equipment intelligent fault diagnostics." %}
    {% when "4-smart substation& online monitoring" %}
      {% assign anchor_id = "substation" %}
      {% assign category_label = "Intelligent Substation Monitoring Systems" %}
      {% assign category_subtitle = "Digital inspection architectures, online monitoring concepts, and integrated warning workflows for utility operations." %}
    {% when "5-drone & advanced" %}
      {% assign anchor_id = "drone" %}
      {% assign category_label = "Autonomous Inspection" %}
      {% assign category_subtitle = "Autonomous inspection system integrating sensing, perception, and decision-making into a closed loop." %}
  {% endcase %}

  <section id="{{ anchor_id }}" class="project-category-block" data-flow-section="{{ anchor_id }}">
    <h2 class="category category-section">{{ category_label }}</h2>
    <p class="category-subtitle">{{ category_subtitle }}</p>
  {% if anchor_id == "cable" %}
    <p class="workflow-hint">Screening → Localization → Validation → Maintenance</p>
  {% endif %}
  {% if anchor_id == "drone" %}
    <div class="autonomous-flow" aria-label="Autonomous inspection system flow">
      <div class="autonomous-flow-step">Drone sensing</div>
      <div class="autonomous-flow-arrow" aria-hidden="true">→</div>
      <div class="autonomous-flow-step">AI perception</div>
      <div class="autonomous-flow-arrow" aria-hidden="true">→</div>
      <div class="autonomous-flow-step">Autonomous decision</div>
    </div>
  {% endif %}
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  {% if anchor_id == "cable" %}
  <div class="cable-group-heading">Core Workflow</div>
  <div class="row row-cols-1 row-cols-md-3 cable-primary-grid">
    {% for project in sorted_projects limit: 3 %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  <div class="cable-group-heading">Advanced Methods &amp; Engineering Validation</div>
  <div class="row row-cols-1 row-cols-md-3 cable-secondary-grid">
    {% for project in sorted_projects offset: 3 %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endif %}
  {% if anchor_id == "drone" %}
    <p class="category-subtitle">Inspection becomes a closed-loop system - sensing, acting, and deciding in one unified process.</p>
  {% endif %}
  </section>
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>

<script>
  (() => {
    const sections = Array.from(document.querySelectorAll('[data-flow-section]'));
    const nodes = Array.from(document.querySelectorAll('.capability-node'));
    const particle = document.getElementById('flow-particle');
    const flowMap = {
      cable: 'p-cable',
      ai: 'p-ai',
      substation: 'p-substation',
      drone: 'p-drone',
    };
    let activePathId = '';
    let particleProgress = 0;
    let activeTargetId = '';
    let previewTargetId = '';

    if (!sections.length || !nodes.length || !particle) return;

    const clearActiveState = () => {
      document.querySelectorAll('.flow').forEach((line) => line.classList.remove('active'));
      nodes.forEach((node) => node.classList.remove('is-active'));
      activePathId = '';
      particle.setAttribute('visibility', 'hidden');
    };

    function activateFlow(pathId) {
      document.querySelectorAll('.flow').forEach((p) => p.classList.remove('active'));
      const path = document.getElementById(pathId);
      if (path) {
        path.classList.add('active');
        activePathId = pathId;
        particleProgress = 0;
        particle.setAttribute('visibility', 'visible');
      } else {
        activePathId = '';
        particle.setAttribute('visibility', 'hidden');
      }
    }

    const animateParticle = () => {
      if (activePathId) {
        const path = document.getElementById(activePathId);
        if (path && typeof path.getTotalLength === 'function') {
          const length = path.getTotalLength();
          const point = path.getPointAtLength(particleProgress * length);
          particle.setAttribute('cx', point.x);
          particle.setAttribute('cy', point.y);
          particleProgress += 0.012;
          if (particleProgress >= 1) particleProgress = 0;
        }
      }
      requestAnimationFrame(animateParticle);
    };

    animateParticle();

    const activateTarget = (targetId, shouldScroll = true) => {
      const pathId = flowMap[targetId];
      if (!pathId) return;

      if (targetId !== activeTargetId) {
        activateFlow(pathId);
        activeTargetId = targetId;
      }

      const node = document.querySelector('.capability-node[data-flow-target="' + targetId + '"]');
      const section = document.querySelector('[data-flow-section="' + targetId + '"]');

      if (node) node.classList.add('is-active');
      sections.forEach((item) => item.classList.toggle('active', item === section));

      if (shouldScroll && section) {
        section.scrollIntoView({ behavior: 'smooth', block: 'start' });
      }
    };

    nodes.forEach((node) => {
      node.addEventListener('click', (event) => {
        event.preventDefault();
        const targetId = node.dataset.flowTarget;
        if (!targetId) return;

        // First click: preview flow only. Second click on same target: jump.
        if (previewTargetId !== targetId) {
          clearActiveState();
          activateTarget(targetId, false);
          previewTargetId = targetId;
          return;
        }

        clearActiveState();
        activateTarget(targetId, true);
      });
    });

    const syncActiveSection = () => {
      let current = '';
      sections.forEach((section) => {
        const rect = section.getBoundingClientRect();
        if (rect.top < window.innerHeight * 0.38 && rect.bottom > window.innerHeight * 0.18) {
          current = section.dataset.flowSection;
        }
      });
      if (current) {
        clearActiveState();
        activateTarget(current, false);
        previewTargetId = '';
      } else {
        clearActiveState();
        sections.forEach((item) => item.classList.remove('active'));
        activeTargetId = '';
        previewTargetId = '';
      }
    };

    let ticking = false;
    window.addEventListener('scroll', () => {
      if (ticking) return;
      ticking = true;
      window.requestAnimationFrame(() => {
        syncActiveSection();
        ticking = false;
      });
    }, { passive: true });

    syncActiveSection();
  })();
</script>
