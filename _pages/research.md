---
layout: page
title: Research
permalink: /research/
description: A brief summary of my research. Feel free to click on the thumbnails below to read more...
nav: true
display_categories: [work, fun]
horizontal: false
order: 1
---
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

<div class="row justify-content-md-center" style="margin-top: 50px;">
   <img class="img-fluid" width="80%" src="{{ '/assets/img/paper_wordcloud.svg' | relative_url }}" alt="" title="Word cloud"/>
</div>
<div class="caption">
    A word cloud from my recent papers generated using the python package 
   <a href="https://github.com/amueller/word_cloud" style="font-family: monospace; background-color: #171F24; border-radius: 3px; padding: 3px 3px;">wordcloud</a>
</div>

