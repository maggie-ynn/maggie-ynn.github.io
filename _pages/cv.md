---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 6
description: Professional experience, education, publications, and technical strengths in power systems, asset reliability, and grid modernization.
---

<style>
  .cv-page {
    --cv-surface-bg: linear-gradient(180deg, #ffffff 0%, #fbfcfe 100%);
    --cv-surface-bg-strong:
      linear-gradient(135deg, rgba(44, 62, 80, 0.06), rgba(255, 255, 255, 0) 58%),
      linear-gradient(180deg, #ffffff 0%, #f8fbfd 100%);
    --cv-surface-border: color-mix(in srgb, var(--global-divider-color) 84%, #dbe3ea 16%);
    --cv-surface-shadow: color-mix(in srgb, var(--global-theme-color) 7%, transparent 93%);
    --cv-chip-bg: linear-gradient(180deg, #ffffff 0%, #f8fbfd 100%);
    --cv-chip-border: color-mix(in srgb, var(--global-theme-color) 16%, #d9e3ec 84%);
    --cv-chip-text: color-mix(in srgb, var(--global-theme-color) 78%, var(--global-text-color) 22%);
    --cv-item-border: color-mix(in srgb, var(--global-divider-color) 70%, white 30%);
    --cv-muted-panel-bg: #fbfcfd;
    --cv-muted-panel-border: color-mix(in srgb, var(--global-divider-color) 78%, #dce5ec 22%);
  }

  .cv-page {
    display: flex;
    flex-direction: column;
    gap: 1.2rem;
  }

  .cv-hero {
    display: flex;
    flex-direction: column;
    gap: 0.8rem;
  }

  .cv-name {
    margin: 0;
    color: var(--global-theme-color);
    font-size: 1.95rem;
    line-height: 1.15;
    letter-spacing: 0.01em;
  }

  .cv-role {
    margin: 0;
    color: var(--global-text-color);
    font-size: 1.02rem;
    font-weight: 600;
    line-height: 1.5;
  }

  .cv-meta {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem 0.75rem;
    color: var(--global-text-color-light);
    font-size: 0.92rem;
  }

  .cv-meta a {
    color: inherit;
  }

  .cv-lead {
    color: var(--global-text-color);
    font-size: 0.98rem;
    line-height: 1.72;
    margin: 0;
  }

  .cv-highlights {
    display: flex;
    flex-wrap: wrap;
    gap: 0.7rem;
    margin-top: 0.9rem;
  }

  .cv-highlight {
    display: inline-flex;
    align-items: center;
    padding: 0.45rem 0.82rem;
    border: 1px solid var(--cv-chip-border);
    border-radius: 999px;
    background: var(--cv-chip-bg);
    color: var(--cv-chip-text);
    font-size: 0.88rem;
    line-height: 1.35;
    box-shadow: 0 8px 20px color-mix(in srgb, var(--global-theme-color) 8%, transparent 92%);
  }

  .cv-section {
    border: 1px solid var(--cv-surface-border);
    border-radius: 18px;
    background: var(--cv-surface-bg);
    padding: 1.25rem 1.2rem 1.15rem;
    box-shadow: 0 14px 36px var(--cv-surface-shadow);
  }

  .cv-section h2 {
    margin: 0 0 1rem;
    padding-bottom: 0.45rem;
    border-bottom: 1px solid var(--global-divider-color);
    color: var(--global-theme-color);
    font-size: 1.2rem;
  }

  .cv-entry {
    padding: 0.2rem 0 1.05rem;
    margin-bottom: 1.05rem;
    border-bottom: 1px solid var(--cv-item-border);
  }

  .cv-entry:last-child {
    padding-bottom: 0;
    margin-bottom: 0;
    border-bottom: 0;
  }

  .cv-entry-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 1rem;
    margin-bottom: 0.55rem;
  }

  .cv-entry-title {
    color: var(--global-text-color);
    font-size: 1rem;
    font-weight: 600;
    line-height: 1.4;
    margin: 0;
  }

  .cv-entry-org {
    color: var(--global-theme-color);
    font-size: 0.95rem;
    margin-top: 0.1rem;
  }

  .cv-entry-date {
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    white-space: nowrap;
    padding-top: 0.1rem;
  }

  .cv-entry-subsection {
    margin: 0.3rem 0 0.55rem;
    color: var(--global-theme-color);
    font-size: 0.9rem;
    font-weight: 600;
    letter-spacing: 0.01em;
  }

  .cv-section ul,
  .cv-section ol {
    margin: 0.2rem 0 0;
    padding-left: 1.2rem;
  }

  .cv-section li {
    margin-bottom: 0.45rem;
    line-height: 1.6;
    color: var(--global-text-color);
  }

  .cv-section li:last-child {
    margin-bottom: 0;
  }

  .cv-skills {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 0.8rem;
  }

  .cv-skill {
    padding: 0.85rem 0.9rem;
    border: 1px solid color-mix(in srgb, var(--global-theme-color) 16%, var(--cv-surface-border) 84%);
    border-radius: 14px;
    background: var(--cv-muted-panel-bg);
    color: var(--global-text-color);
    font-size: 0.9rem;
    font-weight: 600;
    line-height: 1.45;
  }

  .cv-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
  }

  .cv-link-item {
    flex: 1 1 220px;
    padding: 0.8rem 0.9rem;
    border-radius: 14px;
    background: var(--cv-muted-panel-bg);
    border: 1px solid var(--cv-muted-panel-border);
  }

  .cv-link-item strong {
    display: block;
    margin-bottom: 0.2rem;
    color: var(--global-theme-color);
  }

  .cv-link-item a {
    color: var(--global-text-color);
    word-break: break-word;
  }

  .cv-section.links-section .cv-link-item strong {
    color: var(--global-text-color);
  }

  .cv-section.links-section .cv-link-item a {
    color: var(--global-text-color);
  }

  .cv-section.languages-section .cv-highlight {
    color: var(--global-text-color);
  }

  .cv-footer-note {
    margin-top: 0.15rem;
    color: var(--global-text-color-light);
    font-size: 0.88rem;
    text-align: center;
  }

  html[data-theme="dark"] .cv-page {
    --cv-surface-bg:
      linear-gradient(180deg, rgba(20, 27, 35, 0.98) 0%, rgba(14, 19, 26, 0.98) 100%);
    --cv-surface-bg-strong:
      linear-gradient(135deg, rgba(174, 196, 218, 0.16), rgba(18, 24, 32, 0) 60%),
      linear-gradient(180deg, rgba(22, 29, 38, 0.99) 0%, rgba(13, 18, 24, 0.99) 100%);
    --cv-surface-border: rgba(201, 220, 237, 0.13);
    --cv-surface-shadow: rgba(0, 0, 0, 0.34);
    --cv-chip-bg: linear-gradient(180deg, rgba(33, 43, 55, 0.96) 0%, rgba(24, 32, 42, 0.96) 100%);
    --cv-chip-border: rgba(179, 202, 224, 0.18);
    --cv-chip-text: #d9e7f3;
    --cv-item-border: rgba(201, 220, 237, 0.1);
    --cv-muted-panel-bg: linear-gradient(180deg, rgba(25, 33, 43, 0.96) 0%, rgba(18, 24, 32, 0.96) 100%);
    --cv-muted-panel-border: rgba(201, 220, 237, 0.11);
  }

  html[data-theme="dark"] .cv-section:first-child {
    background: var(--cv-surface-bg-strong);
  }

  html[data-theme="dark"] .cv-highlight {
    box-shadow: 0 12px 28px rgba(0, 0, 0, 0.24);
  }

  html[data-theme="dark"] .cv-skill,
  html[data-theme="dark"] .cv-link-item {
    box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.02);
  }

  @media (max-width: 768px) {
    .cv-section {
      padding: 1rem 0.95rem;
    }

    .cv-entry-header {
      flex-direction: column;
      gap: 0.25rem;
    }

    .cv-name {
      font-size: 1.6rem;
    }

    .cv-entry-date {
      white-space: normal;
    }

    .cv-skills {
      grid-template-columns: 1fr;
    }

    .cv-link-item {
      flex-basis: 100%;
    }
  }
</style>

<div class="cv-page">
  <div class="cv-section">
    <div class="cv-hero">
      <h1 class="cv-name">Maggie Nannan Yan</h1>
      <p class="cv-role">Substation Engineer | Electrical Engineer | Protection System &amp; Control</p>
      <div class="cv-meta">
        <span><a href="mailto:nannanyan.fudan@outlook.com">nannanyan.fudan@outlook.com</a></span>
        <span>|</span>
        <span>Richmond Hill, Ontario</span>
      </div>
      <p class="cv-lead">
        Electrical Engineer with 10+ years of experience in high-voltage substations (110kV-500kV AC, HVDC), specializing in protection &amp; control systems, commissioning, and pre-energization testing. Hands-on experience in protection relay validation, IEC 61850 configuration, and substation system testing including transformers, GIS, and protection schemes. Strong background in system reliability, fault analysis, and field technical execution. Currently pursuing P.Eng (PEO), seeking to further specialize in relay testing, protection systems, and commissioning in North America.
      </p>
    </div>
    <div class="cv-highlights">
      <span class="cv-highlight">10+ Years in High-Voltage Substations</span>
      <span class="cv-highlight">Protection Relay Validation</span>
      <span class="cv-highlight">IEC 61850, GOOSE, MMS</span>
      <span class="cv-highlight">High-Voltage AC and HVDC Systems</span>
      <span class="cv-highlight">Commissioning &amp; Pre-Energization</span>
      <span class="cv-highlight">P.Eng (PEO) Application in Progress</span>
    </div>
  </div>

  <div class="cv-section">
    <h2>Core Competencies</h2>
    <div class="cv-skills">
      <div class="cv-skill">Protection &amp; Control (GE, Siemens, ABB)</div>
      <div class="cv-skill">Relay Testing &amp; Validation</div>
      <div class="cv-skill">Commissioning &amp; Pre-Energization</div>
      <div class="cv-skill">IEC 61850 (GOOSE, MMS)</div>
      <div class="cv-skill">Substation Engineering (HV AC/HVDC)</div>
      <div class="cv-skill">SCADA &amp; RTU Integration</div>
      <div class="cv-skill">Transformer &amp; GIS Testing</div>
      <div class="cv-skill">Grounding &amp; Lightning Protection</div>
      <div class="cv-skill">High-Voltage Diagnostics (PD, Infrared, UV, Acoustic)</div>
    </div>
  </div>

  <div class="cv-section">
    <h2>Professional Experience</h2>
    <div class="cv-entry">
      <div class="cv-entry-header">
        <div>
          <div class="cv-entry-title">Electrical Engineering Research &amp; Asset Analytics</div>
          <div class="cv-entry-org">Shanghai Energy Internet Research Institute (State Grid Corporation of China)</div>
        </div>
        <div class="cv-entry-date">Jan 2019 - Jan 2025</div>
      </div>
      <ul>
        <li>Led development of intelligent operation and maintenance (O&amp;M) solutions integrating condition monitoring and asset health data.</li>
        <li>Established and managed a high-voltage diagnostics and digital asset evaluation laboratory, directing technical framework development, system implementation, and operational governance.</li>
        <li>Supported implementation of digital asset management and smart O&amp;M systems for transmission infrastructure.</li>
        <li>Designed and implemented data-driven asset health assessment methodologies and failure risk prediction models.</li>
        <li>Applied AI-based modeling and analytics to partial discharge (PD), infrared thermography, and acoustic diagnostic datasets.</li>
        <li>Performed electromagnetic field (EMF) simulation and grounding system modeling for safety and compliance evaluation.</li>
        <li>Contributed to technical standards and documentation for smart grid and asset analytics programs.</li>
      </ul>
    </div>

    <div class="cv-entry">
      <div class="cv-entry-header">
        <div>
          <div class="cv-entry-title">Transmission Asset &amp; Reliability Engineer</div>
          <div class="cv-entry-org">Shanghai Electric Power Company (State Grid Corporation of China)</div>
        </div>
        <div class="cv-entry-date">Jan 2012 - Dec 2019</div>
      </div>
      <div class="cv-entry-subsection">Transmission Asset Governance &amp; Reliability</div>
      <ul>
        <li>Served as electrical testing subject-matter expert within a transmission asset governance program covering 128 substations (&ge;110kV).</li>
        <li>Assessed equipment condition and provided risk-based corrective action recommendations.</li>
        <li>Developed inspection standards, evaluation criteria, and testing guidelines for regional transmission departments.</li>
        <li>Contributed to structured equipment health scoring methodologies supporting asset health and compliance improvement.</li>
      </ul>
      <div class="cv-entry-subsection">Field Commissioning &amp; Technical Responsibility</div>
      <ul>
        <li>Led and supported commissioning activities, including protection verification, system readiness checks, and coordination for safe energization.</li>
        <li>Performed protection relay testing and validation, including functional verification of protection schemes for transformers, feeders, and substation systems.</li>
        <li>Worked with IEC 61850-based substation communication systems, including configuration and validation of GOOSE messaging.</li>
        <li>Conducted grounding system analysis and lightning protection compliance verification.</li>
        <li>Executed advanced high-voltage diagnostics including partial discharge (PD), infrared thermography, UV corona, and acoustic monitoring.</li>
      </ul>
    </div>
  </div>

  <div class="cv-section">
    <h2>Education</h2>
    <div class="cv-entry">
      <div class="cv-entry-header">
        <div>
          <div class="cv-entry-title">Visiting Researcher, Energy Storage</div>
          <div class="cv-entry-org">University of Waterloo, Canada</div>
        </div>
      </div>
    </div>

    <div class="cv-entry">
      <div class="cv-entry-header">
        <div>
          <div class="cv-entry-title">Ph.D., Intelligent Electronic Information</div>
          <div class="cv-entry-org">Fudan University</div>
        </div>
      </div>
    </div>

    <div class="cv-entry">
      <div class="cv-entry-header">
        <div>
          <div class="cv-entry-title">Ph.D., High Voltage &amp; Insulation</div>
          <div class="cv-entry-org">Shanghai Jiao Tong University</div>
        </div>
      </div>
    </div>

    <div class="cv-entry">
      <div class="cv-entry-header">
        <div>
          <div class="cv-entry-title">M.Sc., Electric Power System</div>
          <div class="cv-entry-org">Zhejiang University</div>
        </div>
      </div>
    </div>

    <div class="cv-entry">
      <div class="cv-entry-header">
        <div>
          <div class="cv-entry-title">B.Sc., Electrical Engineering</div>
          <div class="cv-entry-org">Zhejiang University</div>
        </div>
      </div>
    </div>

    <div class="cv-entry">
      <div class="cv-entry-header">
        <div>
          <div class="cv-entry-title">ITP, Chu Kochen Honors College</div>
          <div class="cv-entry-org">Zhejiang University</div>
        </div>
      </div>
    </div>
  </div>

  <div class="cv-section">
    <h2>Professional Registration</h2>
    <div class="cv-links">
      <div class="cv-link-item">
        <strong>Professional Engineers Ontario</strong>
        <span>P.Eng application in progress</span>
      </div>
      <div class="cv-link-item">
        <strong>Senior Electrical Engineer</strong>
        <span>Certified Senior Test Technician</span>
      </div>
      <div class="cv-link-item">
        <strong>Certified Carbon Verifier</strong>
        <span>China Carbon Market Institute</span>
      </div>
      <div class="cv-link-item">
        <strong>Executive Committee Member</strong>
        <span>IoT &amp; Automation Subcommittee, IEEE PES China</span>
      </div>
    </div>
  </div>

  <div class="cv-section links-section">
    <h2>Links</h2>
    <div class="cv-links">
      <div class="cv-link-item">
        <strong>Website</strong>
        <a href="https://maggie-ynn.github.io" target="_blank" rel="noopener noreferrer">https://maggie-ynn.github.io</a>
      </div>
      <div class="cv-link-item">
        <strong>LinkedIn</strong>
        <a href="https://www.linkedin.com/in/maggie-yan-612a01385/" target="_blank" rel="noopener noreferrer">https://www.linkedin.com/in/maggie-yan-612a01385/</a>
      </div>
      <div class="cv-link-item">
        <strong>Google Scholar</strong>
        <a href="https://scholar.google.com/citations?user=TPQtOSMAAAAJ&hl=en&oi=sra" target="_blank" rel="noopener noreferrer">https://scholar.google.com/citations?user=TPQtOSMAAAAJ</a>
      </div>
      <div class="cv-link-item">
        <strong>GitHub</strong>
        <a href="https://github.com/maggie-ynn" target="_blank" rel="noopener noreferrer">https://github.com/maggie-ynn</a>
      </div>
    </div>
  </div>

  <div class="cv-section languages-section">
    <h2>Languages</h2>
    <div class="cv-highlights">
      <span class="cv-highlight">English</span>
      <span class="cv-highlight">Mandarin Chinese</span>
      <span class="cv-highlight">French (basic proficiency)</span>
    </div>
  </div>
</div>
