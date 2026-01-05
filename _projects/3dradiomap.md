---
layout: page
title: 3D Radio Map Dataset
description: "Addressing the lack of vertical data in current research, this dataset offers high-resolution 3D maps with rich attributes (RSS, DoA, AoA, ToA), enabling precise environmental perception for drone operations."
img: assets/img/raytracing.png
importance: 2
category: work
selected: true
---

Current research on radio maps predominantly relies on 2D datasets. While some existing works integrate building environment data, they are often limited to 2D planes or simplified vertical slices. This lack of continuous spatial data prevents models from accurately capturing the physical principles of signal propagation in complex real-world environments. Furthermore, many existing datasets focus on non-urban scenarios, which offer limited value for emerging low-altitude economy applications such as drone operations in city centers.

To address these limitations, we propose a comprehensive 3D Radio Map Dataset that features continuous height information with a high spatial resolution of one meter. Unlike previous iterations that typically restrict data to signal strength, this dataset encompasses rich signal parameters, including direction and angle of arrival, time of arrival, and propagation path data. This detailed multi-dimensional structure makes the dataset highly versatile, supporting a wide range of tasks beyond simple map construction, such as precise localization and environmental perception.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/radiomapcompasion.jpg" title="Comparison of Radio Map Datasets" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Comparison of dataset structures. Left: Traditional 2D radio map. Middle: 3D building environment input. Right: The proposed continuous 3D radio map.
</div>
