---
layout: default
title: Archive
---

# Navigating the archive

* [Latest blog post](index.md)
* [All content in one page](all.md)
* [Download for offline view][dl]

# Search

Press `f3` on desktop or tap `find in page` on mobile to search for keywords on any page listed above.

# About the content

The content on this archive is written by Alex Esc. (<a href="{{ site.about }}">about me</a>) and its licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License][l].


[l]: https://creativecommons.org/licenses/by-sa/4.0/
[me]: {{ site.about }}



<a href="{{ site.about }}">about me</a>

# Posts in reverse chronological oder

{% for post in site.posts %}

<div>
  {{ post.date | date: "%b %-d, %Y" }}
    »
  <span class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">{{ post.title }}</a>
  </span>
</div>

{% endfor %}

[dl]: https://github.com/alex-esc/posts/archive/master.zip