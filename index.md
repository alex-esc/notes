---
layout: default
title: Welcome
excerpt_separator: <!--more-->
---

{{site.description}}


## Latest note



{% for post in site.posts limit:1 %}


<article class='post'>
  <h1 class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">
      {{ post.title }}
    </a>
  </h1>

  <div class="post-date">{{ post.date | date: "%b %-d, %Y" }}</div>
  <div class="post-date">
    <a href="https://github.com/alex-esc/notes/blob/master/ {{page.relative_path}} ">
      [edit]
    </a>
  </div>
  
  {{ post.content }}
</article>

{% endfor %}


## Previous notes


{% for post in site.posts limit:5 offset:1 %}


<article class='post'>
  <h3>
    <a href="{{ site.path }}{{ post.url }}">
      {{ post.title }}
    </a>
  </h3>
  <div class="post-date">{{ post.date | date: "%b %-d, %Y" }}</div>
  {{ post.excerpt | strip_html | truncatewords:20 }}
</article>

{% endfor %}



All my notes are licensed under <a href="{{ site.other.licenselink }}">{{ site.licensename }}</a>.


[l]: https://creativecommons.org/licenses/by-sa/4.0/
