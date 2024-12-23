---
layout: page
title: HSED
description: HSED is implemented by using hierarchical search to detect the maximum error of floating-point arithmetic expressions.
img: assets/img/hsed.jpg
importance: 2
category: work
# category: fun
giscus_comments: false
---

HSED is implemented by using hierarchical search to detect the maximum error of floating-point arithmetic expressions. The core idea of HSED is to use the lower precision below the original input precision to guide the search, quickly locate the error hotspots, and use the high precision layer to increase the sampling of the extremely samll intervals that cause the error hotpots to obtain more accurate error results.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/hsed.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The architecture decipts how HSED works, and the open-source repository is available at <a href="https://github.com/zuoyanzhang/HSED">GitHub</a>. The related paper was published and presented at <a href="https://dl.acm.org/doi/10.1007/s11227-023-05523-6">TJSC</a>
</div>
