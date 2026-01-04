---
layout: page
title: Project Title  # 项目标题
description: A short description # 简短描述（显示在卡片上）
img: assets/img/12.jpg # 项目封面图
importance: 1
category: work
---

<!-- 1. 文字介绍区域 -->
这里写你的项目介绍。支持 Markdown 语法。
比如：这是我关于深度学习的研究项目，我们提出了一个新的架构...

<!-- 2. 图片展示区域（一行放2张图） -->
<div class="row">
    <!-- 左边的图片 -->
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/1.jpg" title="图片说明1" class="img-fluid rounded z-depth-1" %}
    </div>
    
    <!-- 右边的图片 -->
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/3.jpg" title="图片说明2" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<!-- 图片下方的说明文字（可选） -->
<div class="caption">
    这里是上面两张图片的统一说明。
</div>

<!-- 3. 如果还有更多图片（比如再放一张大图） -->
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/5.jpg" title="图片说明3" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
