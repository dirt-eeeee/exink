---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<div class="grid-container">
  {% for zine in site.data.zines %}
    <article class="grid-item zine-card">
      <div class="zine-image-box">
      	<div class="angled-box box-bottom turquoise"></div>
      	<div class="angled-box box-top fuchsia"></div>
      </div>
      <p class="zine-title">{{ zine.title }}</p>
      <p class="italic">{{ zine.genre }}</p>
      <p>by {{ zine.author }}</p>
      <p>{{ zine.blurb }}</p>
    </article>
  {% endfor %}
</div>
