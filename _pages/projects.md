<!--
---
layout: page
title: Projects
description: 
permalink: /projects/
nav: true
display_categories: [Application Characterization Methods, System Optimization Techniques, Infrastructure Reconfiguration Mechanisms]
horizontal: false
---


<!-- ### Background

Intelligent datacenters are indispensable infrastructures in the global digital transformation process. In constrast to traditional datacenters that primarily run model-based workloads such as Map-Reduce, etc., intelligent datacenters put an emphasis on deploying and implementing computing systems and infrastructures for emerging "data-centric" tasks such as neural networks. Therefore, intelligent datacenters often run more complex big data models and AI applications. Meanwhile, they incorporate a large number of dedicated and heterogeneous infrastructures for sensing and computing explosive data streams. 

### Motivation

However, the cumbersome data-centric workloads and infrastructures have led to increased power consumption in datacenters. Intelligent datacenters continue to face serious issues of low energy inefficiency and struggle to keep up with the stringent requirements of the global carbon neutrality mandates. In addition, high power consumption can lead to catastrophic losses such as power outages and even fires. Therefore, deploying and implementing highly energy-efficient intelligent datacenters is a major undertaking.

### Issues

In my research, I analyze the causes and challenges of energy inefficiency in intelligent datacenters at different levels of application, system and infrastructure. I conclude three challenges that jeopardize the energy efficiency of intelligent datacenters, including multi-modal workload challenges, disordered system challenges and heterogeneous infrastructure challenges. 

### Solutions

To tackle these challenges and deploy highly-efficient intelligent datacenters, we propose a group of multi-modal workload characterization methods, which include several efficient workload profile models and a workload analysis at the application level. At the system level, we implement a set of disorder-hidden system optimization techniques that enable multi-modal AI applications to run more efficiently on heterogeneous infrastructures. Besides, we also construct a series of architecture reconfiguration mechanisms for efficient collaboration of heterogeneous infrastructures. -->

<!-- Our project aims to deploy and implement highly energy-efficient intelligent datacenters through cross-layer optimization. Intelligent datacenters have become crucial infrastructures for the global digital transformation process. They are designed to handle complex big data models and AI applications, and incorporate a large number of dedicated and heterogeneous infrastructures for sensing and computing data streams. However, the increased power consumption of these datacenters poses a significant challenge to achieving global carbon neutrality and avoiding catastrophic losses. -->

Deploying and implementing highly energy-efficient intelligent datacenters  is a complex but critical undertaking. We propose several solutions to address the challenges of multi-modal workload, disordered system, and heterogeneous infrastructure, and aim to optimize the energy efficiency of intelligent datacenters at different levels. By this, we hope to contribute towards achieving global carbon neutrality and reducing catastrophic losses caused by high power consumption in intelligent datacenters.

### Background:
Traditional datacenters primarily run model-based workloads, such as Map-Reduce, while intelligent datacenters put an emphasis on deploying and implementing computing systems and infrastructures for emerging data-centric tasks, such as neural networks. The complex nature of data-centric workloads and infrastructures has led to low energy efficiency and an inability to meet stringent carbon neutrality mandates.

### Issues:
Our research analyzes the challenges of energy inefficiency in intelligent datacenters at different levels, including application, system, and infrastructure. We have identified three main challenges that contribute to the low energy efficiency of intelligent datacenters: multi-modal workload challenges, disordered system challenges, and heterogeneous infrastructure challenges.

### Solutions:
To tackle these challenges and deploy highly efficient intelligent datacenters, we propose a range of solutions. Firstly, we suggest a group of multi-modal workload characterization methods that include efficient workload profile models and an application level workload analysis. At the system level, we implement a set of disorder-hidden system optimization techniques to enable multi-modal AI applications to run more efficiently. Finally, we develop a heterogeneous infrastructure management framework that integrates various computing infrastructures and optimizes their energy usage.





<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
    {% for category in page.display_categories %}
      <h2 class="category">{{category}}</h2>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <!-- Generate cards for each project -->
      {% if page.horizontal %}
        <div class="container">
          <div class="row row-cols-2">
          {% for project in sorted_projects %}
            {% include projects_horizontal.html %}
          {% endfor %}
          </div>
        </div>
      {% else %}
        <div class="grid">
          {% for project in sorted_projects %}
            {% include projects.html %}
          {% endfor %}
        </div>
      {% endif %}
    {% endfor %}

  {% else %}
  <!-- Display projects without categories -->
    {% assign sorted_projects = site.projects | sort: "importance" %}
    <!-- Generate cards for each project -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-2">
        {% for project in sorted_projects %}
          {% include projects_horizontal.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for project in sorted_projects %}
          {% include projects.html %}
        {% endfor %}
      </div>
    {% endif %}

  {% endif %}

</div>
