---
layout: default
title: Muntasim Ul Haque
description: Personal site of Muntasim Ul Haque - Telecommunications professional specializing in submarine cable infrastructure
---

<div class="intro">
  <p>With over 10 years of experience, I've worked across both power generation and telecommunications, now focused on securing Bangladesh's submarine cable infrastructure. From the power sector to the world of undersea cables, the mission has always been the same: keeping things connected and resilient.</p>
  
  <ul>
    <li>Deputy Manager (Development) at <a href="https://bsccl.com.bd/" target="_blank" rel="noopener noreferrer">Bangladesh Submarine Cables PLC (BSCPLC)</a></li>
    <li>Worked on SEA-ME-WE 5 and SEA-ME-WE 6 submarine cable projects</li>
    <li><a href="https://www.linkedin.com/posts/muntasimulhaque_i-am-honored-to-have-received-the-integrity-activity-7246364149318856704-aKEW" target="_blank" rel="noopener noreferrer">Integrity Award 2024</a> recipient from BSCPLC</li>
    <li>OIC Scholarship recipient during B.S. at <a href="https://www.iutoic-dhaka.edu/" target="_blank" rel="noopener noreferrer">Islamic University of Technology</a></li>
  </ul>
</div>

<div class="section">
  <h2>Experience</h2>
  
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-date">Jan 2025 – Present</div>
      <div class="timeline-content">
        <strong>Deputy Manager (Development)</strong><br>
        Bangladesh Submarine Cables PLC (BSCPLC)
      </div>
    </div>
    
    <div class="timeline-item">
      <div class="timeline-date">Oct 2022 – Jan 2025</div>
      <div class="timeline-content">
        <strong>Deputy Manager (SEA-ME-WE 6 Project), Additional Charge</strong><br>
        Bangladesh Submarine Cables PLC (BSCPLC)
      </div>
    </div>
    
    <div class="timeline-item">
      <div class="timeline-date">Oct 2022 – Jan 2025</div>
      <div class="timeline-content">
        <strong>Assistant Manager (Development)</strong><br>
        Bangladesh Submarine Cables PLC (BSCPLC)
      </div>
    </div>
    
    <!-- Add all other timeline items similarly -->
  </div>
</div>

<div class="section">
  <h2>Education</h2>
  <p>B.S. in Electrical and Electronic Engineering, Islamic University of Technology, 2014</p>
</div>

<div class="section">
  <h2>Skills</h2>
  <div class="skills">
    <span class="skill-chip">C</span>
    <span class="skill-chip">Python</span>
    <span class="skill-chip">MATLAB</span>
    <span class="skill-chip">GNU Octave</span>
    <span class="skill-chip">Bash</span>
    <span class="skill-chip">PSpice</span>
    <span class="skill-chip">HSPICE</span>
    <span class="skill-chip">GNS3</span>
    <span class="skill-chip">EVE-NG</span>
    <span class="skill-chip">Cisco Packet Tracer</span>
    <span class="skill-chip">Anaconda</span>
    <span class="skill-chip">Jupyter Notebook</span>
    <span class="skill-chip">Google Colab</span>
    <span class="skill-chip">UNIX/Linux</span>
    <span class="skill-chip">Networking</span>
    <span class="skill-chip">Cybersecurity Tools</span>
    <span class="skill-chip">LaTeX</span>
    <span class="skill-chip">Web Development</span>
  </div>
</div>

<div class="section">
  <h2>Publications</h2>
  <ul>
    <li>
      <a href="https://ijritcc.org/index.php/ijritcc/article/view/11127" target="_blank" rel="noopener noreferrer">
        Challenges in Implementing Machine Learning-Driven IoT Solutions
      </a> - IJIRTCC 2024
    </li>
    <li>
      <a href="https://doi.org/10.1109/ICISET.2016.7856490" target="_blank" rel="noopener noreferrer">
        Analysis of Charge-Shared Matchline Sensing Schemes
      </a> - ICISET 2016
    </li>
  </ul>
  <p>Details on <a href="https://scholar.google.com/citations?user=XO3Zz1EAAAAJ&hl=en" target="_blank" rel="noopener noreferrer">Google Scholar</a></p>
</div>

<!-- Other sections follow the same pattern -->

<div class="section">
  <h2>Blog Posts</h2>
  <div id="blog-posts">
    <ul>
      {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
      </li>
      {% endfor %}
    </ul>
  </div>
</div>