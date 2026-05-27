---
layout: mdpage
title: PDE-Constrained Optimization of Conditioned Spaces
image: assets/images/hvac.jpg
description: 'Scalable High-Fidelity Modeling for Airflow Optimization'
nav-menu: false
show_tile: false
banner_color: style5
---

# Idea
<img src="../assets/images/hvac.jpg" style="max-width:900px;width:100%">

The standard tool for simulating airflow in ventilated spaces is computational fluid dynamics (CFD), which is notoriously time-consuming and computationally expensive, making it impractical to embed directly into an optimization framework. This has motivated the development of faster surrogate and reduced-order models. We focus on modeling techniques suited specifically to large conditioned spaces, and leverage tools developed within our group, [InfiniteOpt.jl](https://infiniteopt.github.io/InfiniteOpt.jl/stable/) and [InfiniteExaModels.jl](https://github.com/infiniteopt/InfiniteExaModels.jl), to further accelerate the solution of these optimization problems on GPUs.

<ul class="actions">
    <li><a href="/research.html#infiniteopt" class="button icon fa-arrow-left">Go back to Research Summaries</a></li>
</ul>