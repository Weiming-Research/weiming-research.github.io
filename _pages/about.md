---
layout: about
title: about
permalink: /
subtitle: "Research Assistant @ <a href='https://www.cuhk.edu.cn/en'>Chinese University of Hong Kong, Shenzhen</a>."

profile:
  align: right
  image: my_avatar.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <a href="/assets/pdf/Resume_weiming.pdf" target="_blank">Résumé/CV</a>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---
Welcome! I am a Research Assistant at <a href="http://chenjunting.org" target="_blank">WISELab</a>, <a href="https://www.cuhk.edu.cn/en" target="_blank">CUHK-Shenzhen</a>. I am fortunate to be advised by <a href="https://sse.cuhk.edu.cn/en/faculty/chenjunting" target="_blank">Prof. Junting Chen</a>. Previously, I had the opportunity to intern at <a href="https://www.kaust.edu.sa/en/" target="_blank">KAUST</a>, working under <a href="https://cemse.kaust.edu.sa/profiles/tareq-al-naffouri" target="_blank">Prof. Tareq Al-Naffouri</a> in the <a href="https://isl.kaust.edu.sa" target="_blank">Information Science Lab</a>.

Before that, I earned B.Eng. in Intelligence Science and Technology from <a href="https://en.shu.edu.cn" target="_blank">Shanghai University</a>. During my undergraduate studies, I was mentored by <a href="https://liyanma-shu.github.io" target="_blank">Prof. Liyan Ma</a> and <a href="https://scie-ce.shu.edu.cn/info/1091/1075.htm" target="_blank">Prof. Qinghua Huang</a>.

My research aims to push the frontiers of AI through **Physics-inspired Large Language Models**. Currently, I focus on applying these techniques to wireless communications and acoustic sensing, with specific interests in:
<ul>
    <li>LLM-based Radio Map Learning and Applications</li>
    <li>Dynamic 3D Communications</li>
    <li>Sound Event Localization and Detection</li>
</ul>

<div class="intro-quote">
    "Curiosity evokes 'care'; it evokes the care one takes of what exists and what might exist." &mdash; Michel Foucault
</div>

<h2>
  <a href="{{ '/projects/' | relative_url }}" style="color: inherit;">selected projects</a>
</h2>

<!-- selected Projects 内容区域 -->
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

<style>
  /* 1. 隐藏自动生成的论文列表左侧的缩略图/徽章列 */
  .publications .row .abbr,
  .publications .row .preview {
    display: none !important;
  }
  
  /* 2. 将论文文字内容区域强制拉宽到 100% */
  .publications .row .col-sm-8 {
    flex: 0 0 100% !important;
    max-width: 100% !important;
    
    /* 关键修改：删除了 padding: 0 的设置 */
    /* 让它保留 Bootstrap 默认的 15px padding，从而与上方的 Projects 对齐 */
  }

  /* 3. (可选) 如果看起来还是有一点点不对齐，可以强制重置 Row 的 margin */
  /* 通常不需要这步，但如果上面改了还不行，请把下面这行注释解开 */
  /* .publications .row { margin-left: 0 !important; margin-right: 0 !important; } */
</style>
