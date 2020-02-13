---
layout: "post"
title: "Psicología general: procesos y teorías"
---


## All in one




{% for post in site.tags.Psicologia general %}

<article class='post'>
  <h1 class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">
      {{ post.title }}
    </a>
  </h1>
  <div class="post-date">{{ post.date | date: "%b %-d, %Y" }}</div>
  {{ post.content }}
</article>

{% endfor %}




{% for item in collection reversed %}
{% for post in site.tags.Psicologia general %}

<div>
  
    »
  <span class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">{{ post.title }}</a>
  </span>
</div>

{% endfor %}
{% endfor %}

