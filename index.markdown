---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<div class="grid-container">
  {% for zine in site.data.zines %}
    <article class="grid-item zine-card">
      <div class="zine-image-box">
      	<div class="zine-image-box-item rounded box-bottom turquoise"></div>
      	<div class="zine-image-box-item rounded box-top fuchsia"></div>
      	<img src="assets/covers/{{zine.front_cover}}" alt="Front cover of {{zine.title}}" class="zine-image-box-item zine-image {{zine.cover_style}}">
      </div>
      <p class="zine-title">{{ zine.title }}</p>
      <p class="italic">{{ zine.genre }}</p>
      <p>by {{ zine.author }}</p>
      <p>{{ zine.blurb }}</p>
    </article>
  {% endfor %}
</div>
