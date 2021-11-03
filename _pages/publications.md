---
layout: page
permalink: /publications/
title: Research Interests & Publications
# description: List of my publications in reversed chronological order. 
years: [2021, 2020, 2019]
---
My research interests span a wide array of topics around graph neural networks. Rather than focusing on a particular niche, I like to constantly look for new interesting and impactful problems. Some of the problems in graph neural networks that have caught my interest so far are:
- **Scalability**: How do we scale GNNs to billion nodes graphs?
- **Dynamic Graphs**: How do we learn on graphs that change over time? 
- **Missing Node Features**: How do apply GNNs to graphs where we only observe only a subset of features for each node (which is almost always the case in practice)?
- **Low Homophily Graphs**: How do we design GNNs that work on graphs with low label homophily (where neighbors tend to have different labels)

### Publications
Below is a list of my publications in reversed chronological order. 


{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
