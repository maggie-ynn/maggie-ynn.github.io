---
layout: page
title: Frequency-domain Fault Mapping
description: Frequency-domain cable diagnostics using wideband impedance sensing and IFFT-based defect localization.
img: assets/img/project-cases/cable-grounding/cable-case-6.png
_styles: >
  .defect-gallery {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
    margin: 1rem 0 1.35rem;
  }

  .defect-card {
    border: 1px solid rgba(148, 163, 184, 0.24);
    border-radius: 1rem;
    overflow: hidden;
    background: rgba(248, 250, 252, 0.72);
  }

  html[data-theme='dark'] .defect-card {
    background: rgba(15, 23, 42, 0.64);
    border-color: rgba(148, 163, 184, 0.18);
  }

  .defect-card img {
    display: block;
    width: 100%;
    max-height: 220px;
    object-fit: contain;
    background: rgba(255, 255, 255, 0.92);
    padding: 0.6rem;
  }

  .defect-card-title {
    padding: 0.55rem 0.8rem 0.75rem;
    font-size: 0.82rem;
    font-weight: 700;
    color: var(--global-text-color);
    text-align: center;
  }

  @media (max-width: 767px) {
    .defect-gallery {
      grid-template-columns: 1fr;
    }
  }

  .method-figure {
    margin: 1rem 0 1.35rem;
    border: 1px solid rgba(148, 163, 184, 0.24);
    border-radius: 1rem;
    overflow: hidden;
    background: rgba(248, 250, 252, 0.72);
  }

  html[data-theme='dark'] .method-figure {
    background: rgba(15, 23, 42, 0.64);
    border-color: rgba(148, 163, 184, 0.18);
  }

  .method-figure img {
    display: block;
    width: 100%;
    max-height: 440px;
    object-fit: contain;
    background: rgba(255, 255, 255, 0.96);
    padding: 0.65rem;
  }

  .method-figure-caption {
    padding: 0.6rem 0.9rem 0.8rem;
    font-size: 0.84rem;
    color: var(--global-text-color-light);
    text-align: center;
  }
importance: 6
category: "1-cable&grounding diagnostics"
case_logic_step: Advanced Methods
---

This case introduced a frequency-domain perspective into practical cable diagnostics. Instead of waiting for obvious failure signatures, the workflow aimed to detect earlier-stage degradation and convert spectral response into spatial fault insight.

## Problem

Cable defects, including joint degradation and shielding failure, are difficult to detect early using conventional time-domain methods.

<div class="defect-gallery">
  <div class="defect-card">
    <img src="{{ '/assets/img/project-cases/cable-grounding/defects/electrical-tree.png' | relative_url }}" alt="Electrical treeing defect example">
    <div class="defect-card-title">Electrical Treeing</div>
  </div>
  <div class="defect-card">
    <img src="{{ '/assets/img/project-cases/cable-grounding/defects/insulation-breakdown.png' | relative_url }}" alt="Insulation breakdown defect example">
    <div class="defect-card-title">Insulation Breakdown</div>
  </div>
  <div class="defect-card">
    <img src="{{ '/assets/img/project-cases/cable-grounding/defects/corroded-conductor.png' | relative_url }}" alt="Corroded conductor defect example">
    <div class="defect-card-title">Corroded Conductor</div>
  </div>
  <div class="defect-card">
    <img src="{{ '/assets/img/project-cases/cable-grounding/defects/joint-degradation.png' | relative_url }}" alt="Joint degradation defect example">
    <div class="defect-card-title">Joint Degradation</div>
  </div>
</div>

## Method

Utilized wideband impedance spectroscopy with frequency-sweep excitation, combined with IFFT-based signal reconstruction, to map defects in the spatial domain.

<div class="method-figure">
  <img src="{{ '/assets/img/project-cases/cable-grounding/defects/wideband-principle.png' | relative_url }}" alt="Wideband impedance spectroscopy principle diagram">
  <div class="method-figure-caption">Wideband sensing principle and reflected-signal interpretation for spatial defect mapping.</div>
</div>

## Evidence

- Multi-frequency acquisition in the 10 to 20 MHz range
- Identified a defect at approximately 705 meters associated with shield corrosion and breakage
- Accurate localization of multiple joints along a 1.5 km cable

## Outcome

- Enabled early-stage defect detection before failure
- Provided full-length cable condition visibility
- Introduced frequency-domain analysis into practical field diagnostics
