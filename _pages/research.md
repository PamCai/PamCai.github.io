---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
header:
  og_image: "research/2SFRAP.png"
---

My academic research leverages **theoretical polymer physics** and **experimental rheological characterization** tools to applications in novel materials and biological fluids. I am interested in the connection between molecular level design of polymeric materials and their macroscopic physical behavior. Polymeric materials of interest include polymers with dynamic associations (sometimes known as "self-healing" materials) and polymers that interact via ionic bonds. These materials of the utmost interest because of their prevalence in biological tissues and fluids. For example, extracellular matrices are composed of polymers that can form dynamic bonds such as collagen, laminin, and hyaluronic acid. On the other hand, biopolymers are also charged, and their charged nature can influence the overall physical behavior of these biological fluids, such as mucus. Thus, I have derived polymer dynamics theories that leverage experimentally relevant molecular level parameters of polymers to predict the macrorheological behavior of these bulk materials.

Theory, however, is not useful in a vacuum. Knowledge of molecular details would help the design of biomaterials used for creating disease models. Additionally, biophysical understanding of biological fluids like mucus could inspire more target-specific treatments for mucus-related diseases. So, another focus of my work is on characterization techniques that allow better probing of complex biological materials, helping us gain insight into the physical interactions between components within. I have characterized COVID-19 patient-derived respiratory secretions using dynamic light scattering (DLS) microrheology to recommend better treatments to improve breathing in patients. Lastly, I have used biophysical modeling to gain insight into the mechanism behind antibiotic tolerance in <i>Pseudomonas aeruginosa</i>, an opportunistic pathogen that is highly prevalent in hospital infections.

In a new avenue of research, I am leveraging polyelectrolyte complexation to design more sustainable plastics.

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}