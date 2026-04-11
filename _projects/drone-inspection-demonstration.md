---
layout: page
title: Autonomous Control & Decision - Closed-loop Inspection - System-level Execution
description: Closed-loop inspection workflow integrating perception, control, and decision logic into one autonomous system.
img: assets/img/project-cases/drone-advanced/drone-third-cover.jpeg
importance: 3
category: "5-drone & advanced"
---

<div style="margin: 0.55rem 0 1.2rem; border: 1px solid rgba(148, 163, 184, 0.25); border-radius: 14px; overflow: hidden; background: #000;">
  <video controls preload="metadata" style="display: block; width: 100%; max-height: 520px;" src="{{ '/assets/files/project-cases/drone-advanced/drone-third.mp4' | relative_url }}">
    Your browser does not support the video tag.
  </video>
</div>

This case addressed inspection as a system-level execution problem. Instead of manually stitching together sensing, positioning, and judgment, it built a closed-loop process that connects perception, action, and diagnosis.

## Impact Highlights

- Closed-loop inspection (perception -> decision -> action)
- Autonomous target selection and adaptive positioning
- Reduced human dependency in inspection workflows
- Scalable multi-device inspection pipeline

<style>
  .system-wrap {
    margin: 0.95rem 0 0.7rem;
  }

  .system-heading {
    margin: 0 0 0.6rem;
    font-size: 1.05rem;
    font-weight: 700;
    letter-spacing: 0.01em;
    color: #dbeafe;
  }

  .system-container {
    padding: 1.35rem 1.2rem 1.15rem;
    background: linear-gradient(165deg, #071225 0%, #0b1528 100%);
    border: 1px solid rgba(96, 165, 250, 0.22);
    border-radius: 12px;
  }

  .system-row {
    display: flex;
    align-items: stretch;
    justify-content: center;
    gap: 0.8rem;
    flex-wrap: wrap;
  }

  .system-row + .system-row {
    margin-top: 0.8rem;
  }

  .layer-card {
    width: 190px;
    min-height: 132px;
    padding: 0.8rem 0.85rem 0.72rem;
    border-radius: 12px;
    background: linear-gradient(180deg, #12233f 0%, #0f1c33 100%);
    color: #ffffff;
    text-align: left;
    transition: all 0.3s ease;
    border: 1px solid rgba(96, 165, 250, 0.26);
    cursor: pointer;
  }

  .layer-card:hover,
  .layer-card.is-active {
    transform: translateY(-3px);
    box-shadow: 0 8px 24px rgba(59, 130, 246, 0.35);
    border-color: rgba(147, 197, 253, 0.9);
    background: linear-gradient(180deg, #173155 0%, #122643 100%);
  }

  .layer-tag {
    display: inline-block;
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: #93c5fd;
    margin-bottom: 0.35rem;
  }

  .layer-card h3 {
    margin: 0 0 0.34rem;
    font-size: 1.35rem;
    line-height: 1.18;
    font-weight: 700;
    color: #f8fafc;
  }

  .layer-card p {
    margin: 0;
    font-size: 1rem;
    line-height: 1.5;
    color: #dbeafe;
  }

  .arrow-h {
    width: 34px;
    height: 2px;
    background: linear-gradient(90deg, transparent, #60a5fa, transparent);
    align-self: center;
    animation: flow 2s infinite;
  }

  .branch {
    display: flex;
    justify-content: center;
    margin: 0.25rem 0 0.5rem;
  }

  .branch-line {
    width: 2px;
    height: 24px;
    background: linear-gradient(180deg, rgba(96, 165, 250, 0), rgba(96, 165, 250, 0.95), rgba(96, 165, 250, 0));
    animation: flow-v 2s infinite;
  }

  @keyframes flow {
    0% { opacity: 0; }
    50% { opacity: 1; }
    100% { opacity: 0; }
  }

  @keyframes flow-v {
    0% { opacity: 0.25; }
    50% { opacity: 1; }
    100% { opacity: 0.25; }
  }

  .caption {
    text-align: center;
    color: #9ca3af;
    margin-top: 8px;
    font-size: 0.96rem;
    line-height: 1.55;
  }

  @media (max-width: 880px) {
    .layer-card {
      width: 100%;
      min-height: auto;
    }

    .system-row {
      flex-direction: column;
      gap: 0.62rem;
    }

    .arrow-h {
      width: 2px;
      height: 18px;
      margin: 0 auto;
      background: linear-gradient(180deg, transparent, #60a5fa, transparent);
    }
  }
</style>

<div class="system-wrap">
  <p class="system-heading">System Architecture</p>
  <div class="system-container">
    <div class="system-row">
      <div class="layer-card sensing">
        <div class="layer-tag">Layer 1</div>
        <h3>Sensing</h3>
        <p>Visible · Thermal · Acoustic · UV</p>
      </div>

      <div class="arrow-h"></div>

      <div class="layer-card edge">
        <div class="layer-tag">Layer 2</div>
        <h3>On-device AI</h3>
        <p>Detection · Segmentation · PRPD</p>
      </div>

      <div class="arrow-h"></div>

      <div class="layer-card decision">
        <div class="layer-tag">Layer 3</div>
        <h3>Autonomous Decision</h3>
        <p>Target Selection · Path Planning</p>
      </div>
    </div>

    <div class="branch">
      <div class="branch-line"></div>
    </div>

    <div class="system-row">
      <div class="layer-card control">
        <div class="layer-tag">Layer 4</div>
        <h3>Control</h3>
        <p>Gimbal PID · UAV Motion</p>
      </div>

      <div class="arrow-h"></div>

      <div class="layer-card cloud">
        <div class="layer-tag">Layer 5</div>
        <h3>Cloud Platform</h3>
        <p>Data · Model · IoT</p>
      </div>
    </div>
  </div>
</div>

<p class="caption">
  End-to-end autonomous inspection system enabling real-time closed-loop execution from perception to action.
</p>

<script>
  document.querySelectorAll('.layer-card').forEach((layer) => {
    layer.addEventListener('click', () => {
      document.querySelectorAll('.layer-card').forEach((item) => item.classList.remove('is-active'));
      layer.classList.add('is-active');
    });
  });
</script>

## Core Loop

Scan -> Detect -> Select -> Position -> Inspect -> Diagnose

## What I Built

A closed-loop autonomous inspection system that integrates perception, control, and decision logic into one unified workflow.

## Evidence

- Gimbal control using PID for adaptive viewpoint adjustment
- Automatic target selection based on detection results
- Sequential inspection workflow across multiple devices
- System-level pipeline demonstrated in the inspection flow diagram

## Outcome

- Transformed inspection from manual operation to an autonomous system
- Reduced human dependency and operational variability
- Enabled scalable, repeatable inspection workflows
