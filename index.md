---
layout: page
title: Sample blog
tagline: Supporting tagline
---
{% include JB/setup %}
    
<ul class="posts list-unstyled">
  {% for post in site.posts %}
    <li>
      <h2><a class="post-title" href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
      <section class="post-info">
        {% assign info_post = post%}
        Published {% include custom/post_info %}
      </section>
      <p>{{ post.excerpt | markdownify}} <span><a href="{{ BASE_PATH }}{{ post.url }}">&raquo; continue reading</a></span>
      </p>
    </li>
  {% endfor %}
</ul>



