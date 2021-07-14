---
layout: main
---

### Home

## Blog

<ul class="related-posts">

{% assign blog_posts = site.posts | where: 'blog_post', true %}
{% for post in blog_posts limit:3 %}
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

---

## Post 张贴

<ul class="related-posts">

{% assign blog_posts = site.posts | where: 'post', true %}
{% for post in blog_posts limit:3 %}
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

## Show 秀

<ul class="related-posts">

{% assign blog_posts = site.posts | where: 'show', true %}
{% for post in blog_posts limit:3 %}
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

## Projects 项目

<ul class="related-posts">

{% assign blog_posts = site.posts | where: 'projects', true %}
{% for post in blog_posts limit:3 %}
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
