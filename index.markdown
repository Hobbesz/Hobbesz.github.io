---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<h2>Recent Posts</h2>

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

    	<div class="date">
    		{{ post.date | date: "%B %e, %Y" }}
  		</div>

      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
    </article>
  {% endfor %}
</div>
