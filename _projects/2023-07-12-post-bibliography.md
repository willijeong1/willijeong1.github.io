---
layout: page
title: 
description: 
img: 
importance:
category:
related_publications: false
---

This post shows how to add bibliography to simple blog posts. We support every citation style that [jekyll-scholar](https://github.com/inukshuk/jekyll-scholar) does. That means simple citation like {% cite einstein1950meaning %}, multiple citations like {% cite einstein1950meaning einstein1905movement %}, long references like {% reference einstein1905movement %} or also quotes:

{% quote einstein1905electrodynamics %}
Lorem ipsum dolor sit amet, consectetur adipisicing elit,
sed do eiusmod tempor.

Lorem ipsum dolor sit amet, consectetur adipisicing.
{% endquote %}

If you would like something more academic, check the [distill style post]({% post_url 2018-12-22-distill %}).
