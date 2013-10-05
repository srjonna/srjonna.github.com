---
layout: page
title: Sample blog
tagline: Supporting tagline
---
{% include JB/setup %}
    
<ul class="posts">
  {% for post in site.posts %}
    <li>
      <h2>{{ post.title }}</h2>
      <section>
        {% assign post_author = post.author%}
        {% assign post_date = post.date%}
        Published {% include custom/post_info %}
      </section>
    </li>
  {% endfor %}
</ul>



