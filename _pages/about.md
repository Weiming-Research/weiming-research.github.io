---
layout: about
title: about
permalink: /
subtitle: "<a href='http://chenjunting.org'>WISELab</a>."

profile:
  align: right
  image: my_avatar.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <a href="/assets/pdf/Resume_weiming.pdf" target="_blank">Résumé/CV</a>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---
Welcome! I am a research assistant at WISELab, Chinese University of Hong Kong, Shenzhen.

<h2>
  <a href="{{ '/projects/' | relative_url }}" style="color: inherit;">selected projects</a>
</h2>
<div class="projects">
  {% include selected_projects.liquid %}
</div>
