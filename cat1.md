---
layout: page
title: 
permalink: /cat1/
---

<div class="posts">



<div class="cat-nav">
  <ul>
    <li>
      <a  href="/essays">Show All</a>
    </li>
    <li>
    <a class="is-active" href="/cat1" >Category 1</a>
          </li>
    <li>
      <a href="/cat2" class="btn-nav">Category 2</a>
    </li>
    <li>
      <a href="/cat3" class="btn-nav">Category 3</a>
    </li>
        <li>
    <a href="/cat4" class="btn-nav">Category 4</a>
          </li>
    <li>
      <a href="/cat5" class="btn-nav">Category 5</a>
    </li>
  </ul>
</div>

  

  {% for post in site.categories.cat1 %}
  <!-- {% unless post.categories contains "notes" or post.categories contains "lists"%} -->
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  <!-- {% endunless %} -->
  {% endfor %}

  <article class="post">
</div>
