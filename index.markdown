---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<h1>Zines</h1>
<div class="grid-container">
  {% for zine in site.data.zines %}
    <article class="grid-item">
      <h2><a href="{{ post.url }}">{{ zine.title }}</a></h2>
      <!-- <p>{{ zine.excerpt }}</p> -->
    </article>
  {% endfor %}
</div>

<h1>About</h1>

<h1>Contact</h1>
