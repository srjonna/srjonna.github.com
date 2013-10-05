---
layout: page
title: Sample blog
tagline: Supporting tagline
---
{% include JB/setup %}
    
<ul class="posts unstyled">
  {% for post in site.posts %}
    <li>
      <h2>{{ post.title }}</h2>
      <section>
        {% assign post_author = post.author%}
        {% assign post_date = post.date%}
        Published {% include custom/post_info %}
      </section>
      <p>{{ post.excerpt | markdownify}} <span><a href="{{ BASE_PATH }}{{ post.url }}">&raquo; continue reading</a></span>
      </p>
    </li>
  {% endfor %}
</ul>



