---
layout: page
permalink: /patents/
title: Patents
description: Patent portfolio in intelligent diagnostics, multi-modal sensing, and power equipment monitoring.
nav: true
nav_order: 4
_styles: >
  .patents-page {
    --patent-chip-bg: linear-gradient(180deg, #ffffff 0%, #f8fbfd 100%);
    --patent-chip-border: color-mix(in srgb, var(--global-theme-color) 16%, #d9e3ec 84%);
    --patent-chip-text: color-mix(in srgb, var(--global-theme-color) 78%, var(--global-text-color) 22%);
    --patent-surface-bg:
      linear-gradient(180deg, rgba(255, 255, 255, 0.96) 0%, rgba(248, 251, 253, 0.96) 100%);
    --patent-surface-border: color-mix(in srgb, var(--global-divider-color) 82%, #d9e0e7 18%);
    --patent-surface-shadow: 0 14px 34px color-mix(in srgb, var(--global-theme-color) 10%, transparent 90%);
    --patent-image-bg: #f8fafc;
  }

  .patents-intro {
    font-size: 1rem;
    line-height: 1.7;
    color: var(--global-text-color-light);
    margin-bottom: 0;
    padding: 1.15rem 1.25rem 0;
    border: 1px solid var(--patent-surface-border);
    border-bottom: 0;
    border-radius: 18px 18px 0 0;
    background:
      linear-gradient(135deg, rgba(44, 62, 80, 0.06), rgba(255, 255, 255, 0) 58%),
      var(--patent-surface-bg);
  }

  .patents-cert-note {
    font-size: 0.88rem;
    line-height: 1.6;
    color: var(--global-text-color-light);
    margin-bottom: 1.15rem;
    padding: 0 1.25rem 1.15rem;
    border: 1px solid var(--patent-surface-border);
    border-top: 0;
    border-radius: 0 0 18px 18px;
    background:
      linear-gradient(135deg, rgba(44, 62, 80, 0.06), rgba(255, 255, 255, 0) 58%),
      var(--patent-surface-bg);
    box-shadow: var(--patent-surface-shadow);
  }

  h2 {
    margin-top: 1.7rem;
    margin-bottom: 0.75rem;
    padding-bottom: 0.35rem;
    border-bottom: 1px solid var(--global-divider-color);
    font-size: 1.35rem;
  }

  .post ul {
    padding-left: 1.2rem;
    margin-bottom: 0.95rem;
  }

  .post ul li {
    margin-bottom: 0.5rem;
    padding-left: 0.1rem;
  }

  .focus-badges {
    display: flex;
    flex-wrap: wrap;
    gap: 0.7rem;
    margin: 0.35rem 0 0.8rem;
  }

  .focus-badge {
    display: inline-flex;
    align-items: center;
    padding: 0.55rem 0.9rem;
    border: 1px solid var(--patent-chip-border);
    border-radius: 999px;
    background: var(--patent-chip-bg);
    color: var(--patent-chip-text);
    font-size: 0.92rem;
    line-height: 1.35;
    box-shadow: 0 8px 20px color-mix(in srgb, var(--global-theme-color) 8%, transparent 92%);
  }

  .patent-card-content {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 180px;
    gap: 1.25rem;
    align-items: start;
  }

  .patent-card-body {
    min-width: 0;
  }

  .patent-title {
    font-weight: 600;
    color: color-mix(in srgb, var(--global-theme-color) 86%, var(--global-text-color) 14%);
    margin-bottom: 0.3rem;
    line-height: 1.4;
    font-size: 1rem;
  }

  .patent-note {
    color: var(--global-text-color-light);
    line-height: 1.55;
    margin-bottom: 0;
  }

  .patent-application {
    color: var(--global-text-color-light);
    font-size: 0.92rem;
    margin-top: 0.35rem;
  }

  .patent-certificate {
    width: 180px;
    max-width: 100%;
    border: 1px solid var(--global-divider-color);
    border-radius: 6px;
    display: block;
  }

  .granted-patent-cards {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1.1rem;
    margin-bottom: 1.2rem;
  }

  .granted-patent-card {
    position: relative;
    overflow: hidden;
    border: 1px solid var(--patent-surface-border);
    border-radius: 18px;
    padding: 1.05rem 1rem 0.95rem;
    background: var(--patent-surface-bg);
    box-shadow: var(--patent-surface-shadow);
    min-height: 100%;
    display: flex;
    flex-direction: column;
  }

  .granted-patent-card::before {
    content: "";
    position: absolute;
    inset: 0 auto auto 0;
    width: 100%;
    height: 4px;
    background: linear-gradient(90deg, var(--global-theme-color) 0%, color-mix(in srgb, var(--global-theme-color) 45%, white 55%) 100%);
    opacity: 0.9;
  }

  .granted-patent-media {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 0.75rem;
    padding-top: 0.7rem;
    border-top: 1px solid color-mix(in srgb, var(--global-divider-color) 75%, white 25%);
  }

  .certificate-link {
    display: inline-flex;
    justify-content: center;
    border-radius: 16px;
    transition:
      transform 0.18s ease,
      opacity 0.18s ease,
      filter 0.22s ease,
      box-shadow 0.22s ease;
  }

  .certificate-link:hover {
    transform: translateY(-2px);
    opacity: 0.95;
    filter: brightness(1.03);
  }

  .certificate-link.is-activated {
    animation: patent-certificate-shake 0.5s ease;
    box-shadow:
      0 0 0 1px color-mix(in srgb, var(--global-theme-color) 24%, transparent 76%),
      0 0 26px color-mix(in srgb, var(--global-theme-color) 36%, transparent 64%);
    filter: brightness(1.07);
  }

  .certificate-link.is-activated .granted-patent-thumb,
  .certificate-link.is-activated .additional-patent-thumb {
    box-shadow:
      0 0 0 1px color-mix(in srgb, var(--global-theme-color) 30%, transparent 70%),
      0 0 22px color-mix(in srgb, var(--global-theme-color) 34%, transparent 66%),
      0 14px 32px color-mix(in srgb, var(--global-theme-color) 16%, transparent 84%);
  }

  .granted-patent-thumb {
    width: 100%;
    max-width: 128px;
    height: 168px;
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 76%, #d8dee5 24%);
    border-radius: 14px;
    display: block;
    background-color: var(--patent-image-bg);
    padding: 0.28rem;
    box-shadow: 0 12px 28px color-mix(in srgb, var(--global-theme-color) 11%, transparent 89%);
    object-fit: contain;
  }

  .additional-patents-intro {
    color: var(--global-text-color-light);
    line-height: 1.65;
    margin-bottom: 0.8rem;
  }

  .software-cards {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.1rem;
    margin-bottom: 1.2rem;
  }

  .additional-patent-item {
    margin-bottom: 0.8rem;
    padding: 0.75rem 0.9rem;
    border-left: 3px solid color-mix(in srgb, var(--global-theme-color) 20%, #dbe4ec 80%);
    background: color-mix(in srgb, var(--patent-surface-bg) 88%, transparent 12%);
    border-radius: 0 10px 10px 0;
  }

  .additional-patent-gallery {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 0.9rem;
    margin-top: 0.8rem;
  }

  .patent-applications {
    padding: 1rem 1.05rem;
    border: 1px solid var(--patent-surface-border);
    border-radius: 18px;
    background: var(--patent-surface-bg);
    box-shadow: var(--patent-surface-shadow);
  }

  .patent-applications ul {
    margin: 0;
  }

  .patent-applications li {
    color: var(--global-text-color);
  }

  .patent-group {
    padding: 1rem 1.05rem;
    border: 1px solid var(--patent-surface-border);
    border-radius: 18px;
    background: var(--patent-surface-bg);
    box-shadow: var(--patent-surface-shadow);
  }

  .additional-patent-thumb {
    width: 100%;
    max-width: 140px;
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 74%, #d6d9de 26%);
    border-radius: 8px;
    display: block;
    background-color: var(--patent-image-bg);
    padding: 0.2rem;
  }

  .additional-patent-thumb-wrap {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
    padding: 0.65rem 0.55rem;
    border: 1px solid color-mix(in srgb, var(--global-divider-color) 78%, #e2e6eb 22%);
    border-radius: 14px;
    background: var(--patent-surface-bg);
  }

  .additional-patent-thumb-title {
    font-size: 0.84rem;
    color: var(--global-text-color-light);
    text-align: center;
  }

  @keyframes patent-certificate-shake {
    0% {
      transform: translate3d(0, 0, 0) rotate(0deg) scale(1);
    }

    20% {
      transform: translate3d(-2px, 0, 0) rotate(-1.2deg) scale(1.01);
    }

    40% {
      transform: translate3d(2px, -1px, 0) rotate(1.1deg) scale(1.015);
    }

    60% {
      transform: translate3d(-1px, 1px, 0) rotate(-0.8deg) scale(1.01);
    }

    80% {
      transform: translate3d(1px, 0, 0) rotate(0.8deg) scale(1.005);
    }

    100% {
      transform: translate3d(0, 0, 0) rotate(0deg) scale(1);
    }
  }

  html[data-theme="dark"] .patents-page {
    --patent-chip-bg: linear-gradient(180deg, rgba(33, 43, 55, 0.96) 0%, rgba(24, 32, 42, 0.96) 100%);
    --patent-chip-border: rgba(179, 202, 224, 0.18);
    --patent-chip-text: #d9e7f3;
    --patent-surface-bg:
      linear-gradient(180deg, rgba(20, 27, 35, 0.98) 0%, rgba(14, 19, 26, 0.98) 100%);
    --patent-surface-border: rgba(201, 220, 237, 0.13);
    --patent-surface-shadow: 0 16px 38px rgba(0, 0, 0, 0.28);
    --patent-image-bg: #111820;
  }

  html[data-theme="dark"] .patents-cert-note {
    background:
      linear-gradient(135deg, rgba(174, 196, 218, 0.16), rgba(18, 24, 32, 0) 58%),
      var(--patent-surface-bg);
  }

  html[data-theme="dark"] .patents-intro {
    background:
      linear-gradient(135deg, rgba(174, 196, 218, 0.18), rgba(18, 24, 32, 0) 58%),
      var(--patent-surface-bg);
  }

  html[data-theme="dark"] .focus-badge {
    box-shadow: 0 12px 28px rgba(0, 0, 0, 0.24);
  }

  html[data-theme="dark"] .granted-patent-media {
    border-top-color: rgba(201, 220, 237, 0.1);
  }

  html[data-theme="dark"] .certificate-link.is-activated {
    box-shadow:
      0 0 0 1px rgba(191, 211, 230, 0.2),
      0 0 30px rgba(191, 211, 230, 0.28);
  }

  @media (max-width: 768px) {
    h2 {
      font-size: 1.2rem;
    }

    .patent-card-content {
      grid-template-columns: 1fr;
    }

    .granted-patent-cards,
    .additional-patent-gallery {
      grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    .granted-patent-cards {
      grid-template-columns: 1fr;
    }

    .software-cards {
      grid-template-columns: 1fr;
    }
  }
---

<div class="patents-page">
<div class="patents-intro">Inventor of 30+ patents in power systems, AI-driven diagnostics, and intelligent inspection technologies.</div>
<div class="patents-cert-note">All patents and software systems are certified by official intellectual property authorities in China.</div>

<h2><i class="fa-solid fa-crosshairs"></i> Focus Areas</h2>

<div class="focus-badges">
  <span class="focus-badge">Multi-modal sensing and data fusion (acoustic, infrared, UV, visible)</span>
  <span class="focus-badge">AI-based fault detection and asset diagnostics</span>
  <span class="focus-badge">Intelligent inspection and automation in substations</span>
  <span class="focus-badge">High-voltage equipment monitoring and reliability</span>
</div>

<h2><i class="fa-solid fa-certificate"></i> Selected Granted Patents</h2>

<div class="granted-patent-cards">
  <div class="granted-patent-card">
    <div class="patent-title">Multi-band Imaging and Fusion Method</div>
    <div class="patent-note">Enables multi-spectrum data fusion for power equipment condition monitoring, improving fault detection accuracy and supporting reliability assessment of high-voltage assets.</div>
    <div class="patent-application">Applied in power equipment condition monitoring and defect detection.</div>
    <div class="granted-patent-media">
      <a
        href="{{ '/assets/img/patents/multi-band-imaging-and-fusion-method.jpg' | relative_url }}"
        target="_blank"
        rel="noopener noreferrer"
        class="certificate-link"
        aria-label="Open large certificate for Multi-band Imaging and Fusion Method"
      >
        <img
          src="{{ '/assets/img/patents/multi-band-imaging-and-fusion-method.jpg' | relative_url }}"
          alt="Certificate for Multi-band Imaging and Fusion Method"
          class="granted-patent-thumb"
        >
      </a>
    </div>
  </div>
  <div class="granted-patent-card">
    <div class="patent-title">Intelligent Transformer Demagnetization Recorder</div>
    <div class="patent-note">Enables automated recording and control of transformer demagnetization processes, improving maintenance efficiency and supporting reliability of high-voltage equipment.</div>
    <div class="patent-application">Applied in transformer maintenance and reliability improvement.</div>
    <div class="granted-patent-media">
      <a
        href="{{ '/assets/img/patents/intelligent-transformer-demagnetization-recorder.jpg' | relative_url }}"
        target="_blank"
        rel="noopener noreferrer"
        class="certificate-link"
        aria-label="Open large certificate for Intelligent Transformer Demagnetization Recorder"
      >
        <img
          src="{{ '/assets/img/patents/intelligent-transformer-demagnetization-recorder.jpg' | relative_url }}"
          alt="Certificate for Intelligent Transformer Demagnetization Recorder"
          class="granted-patent-thumb"
        >
      </a>
    </div>
  </div>
  <div class="granted-patent-card">
    <div class="patent-title">Remote Pre-triggered Lightning Capture and Detection System</div>
    <div class="patent-note">Enables real-time capture of lightning events in transmission systems, supporting fault investigation, protection validation, and reliability of high-voltage assets.</div>
    <div class="patent-application">Applied in transmission system monitoring and lightning event analysis.</div>
    <div class="granted-patent-media">
      <a
        href="{{ '/assets/img/patents/remote-pre-triggered-lightning-capture-and-detection-system.jpg' | relative_url }}"
        target="_blank"
        rel="noopener noreferrer"
        class="certificate-link"
        aria-label="Open large certificate for Remote Pre-triggered Lightning Capture and Detection System"
      >
        <img
          src="{{ '/assets/img/patents/remote-pre-triggered-lightning-capture-and-detection-system.jpg' | relative_url }}"
          alt="Certificate for Remote Pre-triggered Lightning Capture and Detection System"
          class="granted-patent-thumb"
        >
      </a>
    </div>
  </div>
</div>

<h2><i class="fa-solid fa-laptop-code"></i> Software Systems &amp; Copyrights</h2>

<div class="software-cards">
  <div class="granted-patent-card">
    <div class="patent-title">GIS UV Online Monitoring System (V1.0)</div>
    <div class="patent-note">Developed for real-time detection of partial discharge and insulation defects in GIS equipment using UV sensing, supporting fault investigation and reliability assessment in high-voltage substations.</div>
    <div class="granted-patent-media">
      <a
        href="{{ '/assets/img/patents/gis-uv-online-monitoring-system-v1.jpg' | relative_url }}"
        target="_blank"
        rel="noopener noreferrer"
        class="certificate-link"
        aria-label="Open large certificate for GIS UV Online Monitoring System (V1.0)"
      >
        <img
          src="{{ '/assets/img/patents/gis-uv-online-monitoring-system-v1.jpg' | relative_url }}"
          alt="Copyright certificate for GIS UV Online Monitoring System (V1.0)"
          class="granted-patent-thumb"
        >
      </a>
    </div>
  </div>
  <div class="granted-patent-card">
    <div class="patent-title">AI-based Infrared Inspection System for Power Equipment (V1.0)</div>
    <div class="patent-note">Integrates deep learning with infrared inspection for automated defect detection, enabling fault investigation, condition assessment, and reliability improvement of power system assets.</div>
    <div class="granted-patent-media">
      <a
        href="{{ '/assets/img/patents/ai-based-infrared-inspection-system-v1.jpg' | relative_url }}"
        target="_blank"
        rel="noopener noreferrer"
        class="certificate-link"
        aria-label="Open large certificate for AI-based Infrared Inspection System for Power Equipment (V1.0)"
      >
        <img
          src="{{ '/assets/img/patents/ai-based-infrared-inspection-system-v1.jpg' | relative_url }}"
          alt="Copyright certificate for AI-based Infrared Inspection System for Power Equipment (V1.0)"
          class="granted-patent-thumb"
        >
      </a>
    </div>
  </div>
</div>

<h2><i class="fa-solid fa-file-signature"></i> Selected Patent Applications</h2>

<div class="patent-applications">
  <ul>
    <li>Multi-modal fault diagnosis for power equipment (infrared, acoustic, visual fusion)</li>
    <li>AI-based inspection robot fault recognition system</li>
    <li>Edge-computing-based defect detection in substations</li>
    <li>Infrared-UV-visible fusion diagnostics system</li>
    <li>Automatic annotation and recognition of power equipment using AI</li>
    <li>High-accuracy defect detection for transmission assets</li>
  </ul>
</div>

<h2><i class="fa-solid fa-layer-group"></i> Additional Patents</h2>

<div class="patent-group">
<div class="additional-patents-intro">Additional patents include utility models and industrial designs supporting system implementation and productization.</div>

<div class="additional-patent-item">
  <div class="patent-title">Embedded Device Battery Mounting Structure (Utility Model)</div>
  <div class="patent-note">Designed for stable integration of power modules in embedded inspection devices, supporting reliability and field deployment.</div>
</div>

<div class="additional-patent-item">
  <div class="patent-title">Power Equipment Structural Model (Utility Model)</div>
  <div class="patent-note">Provides structural optimization for power equipment representation and engineering applications.</div>
</div>

<div class="additional-patent-item">
  <div class="patent-title">Infrared Intelligent Inspection Device (Industrial Design)</div>
  <div class="patent-note">Design of an intelligent inspection device for power equipment, supporting infrared-based diagnostics in field environments.</div>
</div>

<div class="additional-patent-gallery">
  <div class="additional-patent-thumb-wrap">
    <a
      href="{{ '/assets/img/patents/embedded-device-battery-mounting-structure-utility-model.jpg' | relative_url }}"
      target="_blank"
      rel="noopener noreferrer"
      class="certificate-link"
      aria-label="Open large certificate for Embedded Device Battery Mounting Structure"
    >
      <img
        src="{{ '/assets/img/patents/embedded-device-battery-mounting-structure-utility-model.jpg' | relative_url }}"
        alt="Certificate for Embedded Device Battery Mounting Structure"
        class="additional-patent-thumb"
      >
    </a>
    <div class="additional-patent-thumb-title">Utility Model Patent Certificate (China)</div>
  </div>
  <div class="additional-patent-thumb-wrap">
    <a
      href="{{ '/assets/img/patents/power-equipment-structural-model-utility-model.jpg' | relative_url }}"
      target="_blank"
      rel="noopener noreferrer"
      class="certificate-link"
      aria-label="Open large certificate for Power Equipment Structural Model"
    >
      <img
        src="{{ '/assets/img/patents/power-equipment-structural-model-utility-model.jpg' | relative_url }}"
        alt="Certificate for Power Equipment Structural Model"
        class="additional-patent-thumb"
      >
    </a>
    <div class="additional-patent-thumb-title">Utility Model Patent Certificate (China)</div>
  </div>
  <div class="additional-patent-thumb-wrap">
    <a
      href="{{ '/assets/img/patents/infrared-intelligent-inspection-device-industrial-design.jpg' | relative_url }}"
      target="_blank"
      rel="noopener noreferrer"
      class="certificate-link"
      aria-label="Open large certificate for Infrared Intelligent Inspection Device"
    >
      <img
        src="{{ '/assets/img/patents/infrared-intelligent-inspection-device-industrial-design.jpg' | relative_url }}"
        alt="Certificate for Infrared Intelligent Inspection Device"
        class="additional-patent-thumb"
      >
    </a>
    <div class="additional-patent-thumb-title">Industrial Design Patent Certificate (China)</div>
  </div>
</div>
</div>

<script>
  document.addEventListener("DOMContentLoaded", () => {
    const certificateLinks = document.querySelectorAll(".certificate-link");

    certificateLinks.forEach((link) => {
      link.addEventListener("click", () => {
        link.classList.remove("is-activated");
        void link.offsetWidth;
        link.classList.add("is-activated");

        window.setTimeout(() => {
          link.classList.remove("is-activated");
        }, 650);
      });
    });
  });
</script>
</div>
