---
layout: post
title: "Some Things I've Made"
author: "Rahul Keerthi"
date: 2020-09-11 20:55:02 +0100
categories: intro portfolio
excerpt: Here are some projects I'm particularly proud of - you can see a description of them, the website (if available) and the source code on GitHub. You can also see my resume to learn more about my story, and discover what kind of spaghetti I like.
---

Here are some projects I'm particularly proud of - you can see a description of them, the website (if available) and the source code on GitHub.

You can also see my resume [here](/apartofme/assets/Rahul Keerthi Resume.pdf){:target="\_blank"} (opens in a new tab) to learn more about my story, and discover what kind of spaghetti I like.

## Solo Projects

{% for project in site.data.projects %}
{% if project.type == "solo" %}

  <div class="card-product">
    <div class="card-product-infos">
      <h1>{{project.title}}</h1>
      <h2>{{project.tagline}}</h2>
      <a href="https://github.com/rahulkeerthi/{{project.github}}" target="_blank">GH</a> {% if project.link %}| <a href="{{project.link}}" target="_blank">Website</a> {% endif %}
      <p><strong>Description:</strong> {{project.description}}</p>
      <p><strong>Stack:</strong> {{project.stack}}</p>
    </div>
  </div>
  {% endif %}
{% endfor %}

## Team Projects

{% for project in site.data.projects %}
{% if project.type == "group" %}

  <div class="card-product">
    <div class="card-product-infos">
      <h1>{{project.title}}</h1>
      <h2>{{project.tagline}}</h2>
      <a href="https://github.com/rahulkeerthi/{{project.github}}" target="_blank">GH</a> {% if project.link %}| <a href="{{project.link}}" target="_blank">Website</a> {% endif %}
      <p><strong>Description:</strong> {{project.description}}</p>
      <p><strong>Stack:</strong> {{project.stack}}</p>
    </div>
  </div>
  {% endif %}
{% endfor %}
