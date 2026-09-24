---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div class="research-home">

<section class="research-hero">
  <p class="research-kicker">COMPUTATIONAL ACOUSTICS · VIRTUAL SENSING · EXECUTABLE DIGITAL TWINS</p>
  <h1>Physics-based models that are <span>fast enough to sense, predict, and interact.</span></h1>
  <p class="research-lead">
    My research develops efficient computational models for large-scale acoustic and vibro-acoustic systems,
    then connects those models with sparse measurements for virtual sensing, state reconstruction,
    data–physics fusion, and executable digital twins.
  </p>
  <div class="research-tags">
    <span>Model Order Reduction</span><span>Virtual Sensing</span><span>Computational Acoustics</span>
    <span>Data–Physics Fusion</span><span>Digital Twins</span>
  </div>
  <div class="research-actions">
    <a class="research-btn primary" href="#framework">Research framework</a>
    <a class="research-btn" href="https://scholar.google.be/citations?user=bu7Opp4AAAAJ&hl=en">Google Scholar</a>
  </div>
</section>

<section id="framework" class="research-section">
  <div class="section-label">RESEARCH FRAMEWORK</div>
  <h2>From high-fidelity simulation to real-time physical intelligence</h2>
  <p class="section-intro">
    The central question behind my work is how to transform accurate but computationally expensive
    physics-based models into compact, stable, and measurement-aware models that can operate online.
  </p>

  <div class="research-pipeline">
    <div class="pipeline-card">
      <b>01</b><h3>High-Fidelity Computational Acoustics</h3>
      <p>Model the wave physics that matter: structural–acoustic coupling, absorbing treatments,
      porous and poroelastic media, and open-domain acoustic radiation.</p>
    </div>
    <div class="pipeline-arrow">→</div>
    <div class="pipeline-card">
      <b>02</b><h3>Stability-Preserving Model Order Reduction</h3>
      <p>Project large systems onto low-dimensional spaces while retaining the dynamic behaviour,
      accuracy, and stability required for time-domain simulation.</p>
    </div>
    <div class="pipeline-arrow">→</div>
    <div class="pipeline-card">
      <b>03</b><h3>Virtual Sensing & Data Fusion</h3>
      <p>Combine reduced physics with limited measurements to reconstruct responses at unmeasured
      locations and estimate the system state.</p>
    </div>
    <div class="pipeline-arrow">→</div>
    <div class="pipeline-card">
      <b>04</b><h3>Executable Digital Twins</h3>
      <p>Build physics-based models that can run online, respond to measurements, and support
      prediction, monitoring, and engineering decisions.</p>
    </div>
  </div>
</section>

<section id="mor" class="research-section research-grid">
  <div>
    <div class="section-label">MODEL ORDER REDUCTION</div>
    <h2>Reducing complexity without reducing physical credibility</h2>
    <p class="section-intro">
      Large finite-element acoustic models are powerful, but their cost makes repeated simulation,
      optimization, estimation, and online prediction difficult. My work focuses on projection-based
      reduced-order modelling for time-domain vibro-acoustic systems, with particular emphasis on
      stability preservation.
    </p>
    <ul class="research-list">
      <li><strong>Stability.</strong> Reduced models for systems with admittance boundaries, absorbing treatments,
      porous/poroelastic media, and perfectly matched layers.</li>
      <li><strong>Dynamics.</strong> Preserve transient response and the relevant system behaviour over the frequency range of interest.</li>
      <li><strong>Efficiency.</strong> Move computational effort offline so repeated online evaluation becomes practical.</li>
      <li><strong>Generality.</strong> Extend reduced-order formulations across interior, exterior, and coupled vibro-acoustic problems.</li>
    </ul>
  </div>
  <div class="mor-diagram">
    <div class="diagram-caption">FULL-ORDER PHYSICS</div>
    <div class="equation">M ü + C u̇ + K u = f</div>
    <div class="diagram-step">↓ projection onto a reduced basis</div>
    <div class="basis">u ≈ Vq</div>
    <div class="diagram-step">↓</div>
    <div class="equation compact">Mᵣ q̈ + Cᵣ q̇ + Kᵣ q = fᵣ</div>
    <div class="diagram-pills"><span>same physical question</span><span>smaller state space</span></div>
  </div>
</section>

<section id="virtual-sensing" class="research-section soft-section research-grid">
  <div class="sensor-visual" aria-label="Virtual sensing concept">
    <div class="sensor-field"></div>
    <span class="real-sensor s1">S1</span><span class="real-sensor s2">S2</span><span class="real-sensor s3">S3</span>
    <span class="virtual-sensor v1">V</span><span class="virtual-sensor v2">V</span>
    <span class="virtual-sensor v3">V</span><span class="virtual-sensor v4">V</span>
  </div>
  <div>
    <div class="section-label">VIRTUAL SENSING</div>
    <h2>Recovering acoustic information where no sensor exists</h2>
    <p class="section-intro">
      Practical systems can only carry a limited number of microphones or vibration sensors.
      Quantities of interest, however, may lie at inaccessible, expensive, or uninstrumented locations.
      Reduced physical models provide a physically consistent way to propagate sparse measured information
      into the wider state of the system.
    </p>
    <div class="research-quote">A few physical sensors can support many physics-consistent virtual sensors.</div>
    <div class="mini-flow"><span>Sparse measurements</span><b>→</b><span>Reduced physics</span><b>→</b><span>State estimation</span><b>→</b><span>Virtual responses</span></div>
  </div>
</section>

<section id="acoustics" class="research-section">
  <div class="section-label">COMPUTATIONAL ACOUSTICS</div>
  <h2>The physical backbone of the digital twin</h2>
  <p class="section-intro">
    Reduced models are only useful when the underlying full-order model captures the relevant physics.
    My computational acoustics work therefore addresses challenging time-domain systems that combine
    wave propagation, complex material behaviour, structural coupling, and unbounded domains.
  </p>
  <div class="topic-grid">
    <div class="topic-card"><b>01</b><h3>Vibro-Acoustic Coupling</h3><p>Transient interaction between vibrating structures and surrounding acoustic fields.</p></div>
    <div class="topic-card"><b>02</b><h3>Absorbing Materials</h3><p>Admittance boundaries, non-locally reacting treatments, and porous/poroelastic media.</p></div>
    <div class="topic-card"><b>03</b><h3>Exterior Acoustics & PML</h3><p>Time-domain radiation problems with perfectly matched layers for efficient open-domain simulation.</p></div>
    <div class="topic-card"><b>04</b><h3>Large-Scale Simulation</h3><p>Finite-element models whose fidelity is high enough for engineering prediction but too costly for online use.</p></div>
  </div>
</section>

<section id="fusion" class="research-section dark-section">
  <div class="section-label">DATA–PHYSICS FUSION</div>
  <h2>Making simulation models respond to the real system</h2>
  <p class="section-intro">
    A digital twin should not be a static simulation. The model must be continuously interpretable in the context
    of measured behaviour. My research uses compact physics-based state spaces as a bridge between sensing and prediction.
  </p>
  <div class="fusion-grid">
    <div><strong>Physics model</strong><span>Provides structure, causality, wave propagation, and physical constraints.</span></div>
    <div><strong>Reduced model</strong><span>Makes repeated estimation and prediction computationally feasible.</span></div>
    <div><strong>Measurements</strong><span>Anchor the model to the actual operating system.</span></div>
    <div><strong>Fusion / estimation</strong><span>Reconstruct hidden states and update quantities that cannot be measured directly.</span></div>
  </div>
</section>

<section id="digital-twin" class="research-section">
  <div class="section-label">EXECUTABLE DIGITAL TWINS</div>
  <h2>A unified direction for simulation, sensing, and prediction</h2>
  <div class="impact-grid">
    <div><strong>Physics-aware</strong><p>Built on interpretable governing equations rather than purely black-box correlations.</p></div>
    <div><strong>Fast enough to execute</strong><p>Reduced state spaces make online prediction, reconstruction, and repeated evaluation possible.</p></div>
    <div><strong>Connected to measurements</strong><p>Real sensor data can be fused with the model to estimate unmeasured acoustic information.</p></div>
  </div>
</section>

<section id="research-track" class="research-section">
  <div class="section-label">SELECTED RESEARCH TRACK</div>
  <h2>How the methodology has developed</h2>
  <div class="research-timeline">
    <article><span>2023</span><h3>Virtual sensing with reduced vibro-acoustic models</h3><p>Time-domain reduced modelling with admittance boundary conditions for virtual sensing applications.</p></article>
    <article><span>2023–2024</span><h3>Complex acoustic treatments</h3><p>Extension to non-locally reacting absorbers and poroelastic materials while retaining efficient time-domain simulation.</p></article>
    <article><span>2024</span><h3>Open-domain acoustics</h3><p>Model order reduction for time-domain acoustic finite-element simulations with perfectly matched layers.</p></article>
    <article><span>2025–2026</span><h3>Toward robust executable models</h3><p>Efficient stability-preserving reduction and integration of computational acoustics, virtual sensing, and measurement-aware digital twins.</p></article>
  </div>
  <p class="research-note">Publications are evidence of this methodology rather than the structure of the website. For the full publication list, see <a href="https://scholar.google.be/citations?user=bu7Opp4AAAAJ&hl=en">Google Scholar</a>.</p>
</section>

<section id="about" class="research-section about-panel">
  <div>
    <div class="section-label">ABOUT</div>
    <h2>Yinshan Cai</h2>
    <p class="section-intro">
      I am a postdoctoral researcher at KU Leuven working on computational vibro-acoustics, model order reduction,
      virtual sensing, and physics-based digital twins. I received my PhD in Mechanical Engineering from KU Leuven
      and my M.Sc. and B.Eng. degrees from Xi'an Jiaotong University.
    </p>
  </div>
  <div class="contact-panel">
    <strong>Research interests</strong>
    <p>Computational acoustics · Model order reduction · Virtual sensing · Data fusion · Digital twins</p>
    <a href="mailto:yinshan.cai@kuleuven.be">yinshan.cai@kuleuven.be</a><br>
    <a href="https://scholar.google.be/citations?user=bu7Opp4AAAAJ&hl=en">Google Scholar</a> ·
    <a href="https://orcid.org/0000-0001-5839-934X">ORCID</a> ·
    <a href="https://github.com/cyanshane">GitHub</a>
  </div>
</section>

</div>
