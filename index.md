---
layout: default
title: Welcome
excerpt_separator: <!--more-->
---



## Latest Post



{% for post in site.posts limit:1 %}


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


## More posts

Find older blog posts on the _[archive](archive.md)_, or follow me via _[RSS](feed.xml)_.


{% for post in site.posts limit:5 offset:1 %}


<article class='post'>
  <h3>
    <a href="{{ site.path }}{{ post.url }}">
      {{ post.title }}
    </a>
  </h3>
  <div class="post-date">{{ post.date | date: "%b %-d, %Y" }}</div>
  {{ post.content | strip_html | truncatewords: 50 }}
</article>

{% endfor %}

All my blog posts are licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License][l].


[l]: https://creativecommons.org/licenses/by-sa/4.0/
 
