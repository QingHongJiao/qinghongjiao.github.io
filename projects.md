---
layout: main
---

## Projects

项目……稍等片刻😂😂😂
---


### 项目 projects

<ul class="related-posts">

{% assign blog_posts = site.posts | where: 'projects', true %}
{% for post in blog_posts %}
        <li class="main-page-list">
        <h4>
            <div style="display: inline-block; width: 90px">
                <small>{{ post.date | date: "%Y-%m-%d" }}</small>
            </div>
        <a href="{{ site.baseurl }}{{ post.url }}">
            <span>{{ post.title }}</span>
        </a>
        </h4>
        </li>
        {% if forloop.last %}</ul>{% endif %}
{% endfor %}
