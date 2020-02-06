---
layout: "post"
title: "abc"
---


## All in one


s


{% for post in site.tags.Primer Semestre %}

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


course: 'Primer Semestre'

{% for post in site.tags.Primer Semestre %}

<div>
  
    »
  <span class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">{{ post.title }}</a>
  </span>
</div>

{% endfor %}




sdsdsdsd
