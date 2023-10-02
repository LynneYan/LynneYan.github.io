---
layout: page
title: Research
permalink: /research/
description: Data visualization provides intuitive and practical tools for information exploration and scientific discovery. However, with the increased availability of computing resources and sensing devices, data’s ever-increasing size and complexity pose fundamental challenges to existing visualization techniques. The first challenge is data understanding, requiring new methodologies to extract key features and insights from large-scale data. Second, the development of data transmission and storage systems is outpaced by unprecedented data growth. This disparity challenges in situ data processing since data needs to be transferred to a commodity workstation to conduct interactive inspections. Third, visualization tools and methodologies for understanding the sensitivities and uncertainties of scientific simulations are lacking. My research aims to address these challenges by significantly enriching methodologies and tools of topology-based visualization for scientific data exploration. 
nav: true
nav_order: 2
display_categories: 
horizontal: false
---

<!-- pages/research.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
