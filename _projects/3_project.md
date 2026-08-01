---
layout: page
title: Chorus
description: Chorus is a compiler-runtime framework that globally schedules transient parameter materialization for memory-constrained sharded LLM training.
img: assets/img/chorus-cover.png
card_img_offset: true
importance: 0
category: work
giscus_comments: false
---

Chorus is a compiler-runtime framework for transient parameter materialization in memory-constrained sharded large language model training. It treats a complete training iteration as a coupled scheduling problem, coordinating communication, full-parameter buffer lifetimes, and computation under time-varying GPU memory headroom.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/chorus-overview.png" title="Overview of the primary Chorus implementation on ZeRO-3" alt="Chorus workflow from PyTorch graph capture through global scheduling and runtime persistent retention" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

As the overview shows, the compiler builds a whole-iteration graph, derives a profile-guided block-level model, selects all-gather launch positions and retention decisions, and realizes the result through graph rewriting and fused prefetching. Runtime warmup then finalizes a persistent retention set using measured memory behavior.

The public implementation supports two distributed training backends: DeepSpeed ZeRO-3 through DeepCompile and PyTorch SimpleFSDP through compiled autograd. The source code and usage guide are available in the <a href="https://github.com/zuoyanzhang/Chorus">Chorus GitHub repository</a>.
