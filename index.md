---
layout: default
title: Welcome
excerpt_separator: <!--more-->
---

{{site.description}}

[New][docli]

[docli]: https://github.com/alex-esc/notes/new/master/_posts

{% for post in site.posts %}

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

See my [future posts list](up-next.md).

All my blog posts are licensed under <a href="{{ site.other.licenselink }}">{{ site.licensename }}</a>.


[l]: https://creativecommons.org/licenses/by-sa/4.0/
