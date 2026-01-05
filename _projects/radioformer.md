---
layout: page
title: RadioFormer
description: "RadioFormer: One Physics-Guided Transformer to Unify 2D and 3D Radio Map Construction. 
A unified, physics-guided framework for 2D/3D radio map construction that achieves SOTA accuracy and operates 2500× faster than diffusion models."
importance: 1
img: assets/img/radioformer.png
category: work

selected: true
---

Radio maps, which model wireless signal quality across different locations, are essential for efficient network planning and positioning. This project aims to generate high-quality 2D and 3D radio maps based on environmental layouts. However, traditional deep learning approaches often fail to understand the underlying physical principles of signal propagation, making them ineffective in unknown environments. Additionally, existing 3D generation models are typically too slow for real-time application.

To address these challenges, we propose **RadioFormer**, a unified framework for both 2D and 3D radio map construction. Our solution uses an efficient compression technique to treat complex 3D data as stacked 2D layers, avoiding high computational costs. Unlike standard models that generate images based on simple pixel statistics, RadioFormer predicts signals by following the actual propagation path of radio waves. This physics-guided approach ensures the results align with physical laws and maintain vertical consistency. Consequently, RadioFormer achieves state-of-the-art accuracy and operates **2500 times faster** than comparable diffusion models, enabling real-time deployment in new environments.

<div class="row">
    <!-- 图1: Framework (Left) -->
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/radioformer.png" title="RadioFormer framework" class="img-fluid rounded z-depth-1" %}
    </div>

    <!-- 图2: Mechanism (Middle) -->
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/wavefront.png" title="Wavefront propagation" class="img-fluid rounded z-depth-1" %}
    </div>

    <!-- 图3: Visualization (Right) -->
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/propagation_visualization.png" title="Propagation order" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<!-- 统一的图注 -->
<div class="caption">
    Left: The RadioFormer framework. Middle: Wavefront propagation mechanism. Right: Visualization of the propagation order.
</div>
