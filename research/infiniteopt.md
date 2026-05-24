---
layout: mdpage
title: Unifying Infinite-Dimensional Optimization
image: assets/images/infiniteopt_discoveries.png
description: 'Accerating Scientific Discovery through Abstraction'
nav-menu: false
show_tile: false
banner_color: style5
---

# Background
Infinite-dimensional optimization (InfiniteOpt) problems contain decision variables that are defined over continuous domains such as a space-time field or states under uncertainty. This classification of problems commonly embed <b>complex modeling elements</b> that include: measures (e.g., multi-dimensional integrals), differential algebraic equations (DAEs), and partial differential equations (PDEs). InfiniteOpt problems encompass a wide breadth of optimization fields that include stochastic optimization, dynamic optimization, PDE-constrained optimization, and combinations (e.g., stochastic PDEs). Applications pertaining to these optimization fields include model predictive control, process design, parameter estimation, reliability analysis, design of dynamic experiments, and more. Moreover, although problems in the aforementioned optimization fields are often identified as InfiniteOpt problems, there exists a <b>conceptual gap in abstracting these problems rigorously through a common lens</b>. Coherent abstractions play a key role in <b>accelerating discovery</b> and enabling general modeling languages.

# Unifying Abstraction
<img src="../assets/images/infiniteopt_discoveries.png" style="max-width:900px;width:100%">

To address the above gap, we developed  a <b>unifying abstraction for infinite-dimensional optimization</b> problems. This abstraction enables us to <b>navigate the complexity</b> in modeling/optimizing systems involving continuous domains (e.g., space-time, uncertainty). This integrates a number of distinct optimization fields to facilitate <b>theoretical crossover that has led to several scientific discoveries</b> such as highly accurate model identification for dynamic systems, new risk assessment metrics for decision-making, [characterizing uncertainty via random field theory](/research/rfo.html), the incorporation of [neural operator surrogates](/research/neuralops.html) into decision-making, and event-constrained optimization; all of which have inspired a <b>significant number of publications</b>. Moreover, I implemented the abstraction in the Julia software package [InfiniteOpt.jl](https://infiniteopt.github.io/InfiniteOpt.jl/stable/) which has amassed a large number of users across a wide breadth of application areas. This software package has also helped <b>accelerate scientific discoveries</b> and ensure these are <b>accessible</b> to individuals in diverse disciplines. For instance, InfiniteOpt.jl recently enabled evolutionary biologists to compare the paths chosen by mice against rigorous path planning determined by advanced decision-making techniques.

# GPU-Accelerated Nonlinear Optimization
<img src="../assets/images/gpu-transcription.jpg" style="max-width:1500px;width:100%">

InfiniteOpt problems are solved via direct transcription, producing large-scale finite-dimensional problems with highly recurrent algebraic structure. By exploiting this structure through a single instruction, multiple data (SIMD) abstraction, these problems can be parallelized on GPU architectures to significantly accelerate solution times. We implement this abstraction in the Julia package [InfiniteExaModels.jl](https://github.com/infiniteopt/InfiniteExaModels.jl), enabling scalable solution of nonlinear InfiniteOpt problems. This is especially impactful for applications such as nonlinear model predictive control, where such problems must be solved in real time.

# Infinite-Dimensional Generalized Disjunctive Programming
<img src="../assets/images/infinite_gdp_example.jpg" style="max-width:1500px;width:100%">

Many real-world systems combine <b>continuous dynamics</b> with <b>discrete logical decisions</b>, such as mode switching in chemical reactors, batch process scheduling, and control of hybrid dynamical systems. Generalized disjunctive programming (GDP) provides a natural language for such structure, but extending it to infinite-dimensional settings introduces new modeling and algorithmic challenges. We extend GDP to the infinite-dimensional setting, enabling descisions whose constraints depend on continuous parameters such as time, space, or uncertainty. This extentsion is available in the Julia package [DisjunctiveProgramming.jl](https://github.com/infiniteopt/DisjunctiveProgramming.jl). This is especially impactful for hybrid dynamic optimization, mode-switching control, and logic-based scheduling.

<ul class="actions">
    <li><a href="/research.html#infiniteopt" class="button icon fa-arrow-left">Go back to Research Summaries</a></li>
</ul>