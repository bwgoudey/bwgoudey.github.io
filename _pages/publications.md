---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
sidebar:
  nav: publications_nav
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Journal articles
{% for post in site.publications reversed %}
    {% if post.path contains '/journal' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}

## Conference proceedings
{% for post in site.publications reversed %}
    {% if post.path contains '/conference' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}

## Submissions and Pre-prints 
{% for post in site.publications reversed %}
    {% if post.path contains '/preprints' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}

## Patents 
{% for post in site.publications reversed %}
    {% if post.path contains '/patents' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}
