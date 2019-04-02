---
layout: default
title:  Welcome
---

{% for post in site.posts %}
<section>
<article class='post'>
  <div class="post-date">{{ post.date | date: "%m/%d/%Y" }}</div>
  <h2 class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">
      {{ post.title }}
    </a>
  </h2>
  <span class='book-author'>
  by {{ post.book-author }}
  </span>
  <div class='post-excerpt'>
    {{ post.excerpt }}
    <a href='{{ site.path }}{{ post.url }}' class='flourish' >
      &#8640;
    </a>
  </div>
</article>
</section>
{% endfor %}
