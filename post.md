---
layout: main
---

## Post

I started reading regularly in Dec'2019 and have not stopped since. I enjoy fiction the most
but occasionally also try books around personal-development, biographies, etc.

I use this page to get myself into the habit of writing more. Below you can find
a list of my recommended books; books that I have read recently; and, some
random ramblings around the same.

I am quite active on [Goodreads](https://www.goodreads.com/user/show/33989424-ankit-sultana)
as well.

---

###  Posts

<ul class="related-posts">

{% assign blog_posts = site.posts | where: 'post', true %}
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

