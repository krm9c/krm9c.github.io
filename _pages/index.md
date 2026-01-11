---
layout: home
title: Home
permalink: /
nav: false
---

My primary research agenda is to develop a mathematical characterization of machine learning (ML) models,
their learning/training behavior and the associated precision achieved by them.
Towards this end, I study the two broad facets of ML: theory; through the eyes of tools from systems theory, statistics and optimization;
and applied; by building AI/ML models to solve key problems in nuclear physics, material science, HPC and more recently climate.
I have a strong publication record in the field of ML, HPC and scientific applications with a total of 51 publications.
I also have a significant track record of grants and have been involved in 23 grant proposals, many of them multi-institutional.
I also have substantial experience in successfully soliciting and managing multi-million dollar multi-institutional proposals as an institutional PI.

## News

<ul class="news-list">
  <li>
    <span class="news-date">Jul 2025</span>
    <span class="news-content">Presentation at <span class="news-venue">International Conference on Continuous Optimization</span></span>
  </li>
  <li>
    <span class="news-date">May 2025</span>
    <span class="news-content">Presentation at <span class="news-venue">SIAM Dynamical Systems</span></span>
  </li>
  <li>
    <span class="news-date">Feb 2025</span>
    <span class="news-content">Presentation at <span class="news-venue">SIAM-Computational Science and Engineering</span></span>
  </li>
  <li>
    <span class="news-date">Oct 2024</span>
    <span class="news-content">Grant awarded: <span class="news-venue">SciDAC-5 Rapids3 Institute</span></span>
  </li>
  <li>
    <span class="news-date">Sep 2024</span>
    <span class="news-content">Grant awarded: <span class="news-venue">Privacy Preserving Federated Learning</span></span>
  </li>
</ul>

<p><a href="{{ '/news/' | relative_url }}">See all news &rarr;</a></p>

## Research Areas

<div class="research-grid">
  {% for topic in site.data.research_topics %}
  <a href="{{ topic.permalink | relative_url }}" class="research-card card-{{ topic.color }}">
    <span class="card-number"><i class="fas {{ topic.icon }}"></i></span>
    <h3>{{ topic.title }}</h3>
    <span class="card-count">{{ topic.paper_count }} papers &rarr;</span>
  </a>
  {% endfor %}
</div>

## Quick Links

<div class="quick-links">
  <a href="{{ '/publications/' | relative_url }}">Publications (41+)</a>
  <a href="{{ '/team/' | relative_url }}">Team</a>
  <a href="{{ '/software/' | relative_url }}">Software</a>
  <a href="{{ '/assets/pdf/cv.pdf' | relative_url }}" target="_blank">CV (PDF)</a>
  <a href="https://scholar.google.com/citations?user=AQUdlTMAAAAJ" target="_blank">Google Scholar</a>
</div>
