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
  <a href="{{ '/projects/' | relative_url }}" style="color: inherit;">Selected projects</a>
</h2>

<!-- Selected Projects 内容区域 -->
<div class="projects">
  <!-- 创建一个 Grid 容器，强制让卡片竖向排列 -->
  <div class="row row-cols-1"> 
    
    <!-- 获取所有 selected=true 的项目，并按 importance 排序 -->
    {% assign selected_projects = site.projects | where: "selected", "true" | sort: "importance" %}
    
    <!-- 循环输出每一个项目 -->
    {% for project in selected_projects %}
      <!-- 
         调用 projects_horizontal.liquid 
         它会自动读取 project.img 显示图片
         读取 project.description 显示描述
         并自动排版成“图片+文字”的横向卡片
      -->
      {% include projects_horizontal.liquid %}
    {% endfor %}
    
  </div>
</div>
