---
layout: publication
date:   2025-08-14
title:  "Histogram Stratification for Spatio-Temporal Reservoir Sampling"
authors: [
    {name: "Corentin Salaün", affiliation: "MPI", url: "https://iribis.github.io/"},
    {name: "Martin Bálint", affiliation: "MPI", url: "https://people.mpi-inf.mpg.de/~mbalint/"},
    {name: "Laurent Belcour"},
    {name: "Eric Heitz"},
    {name: "Gurprit Singh", affiliation: "MPI"},
    {name: "Karol Myszkowski", affiliation: "MPI"},
]
conference: "ACM SIGGRAPH 2025"
categories: publication
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2025_stratified_restir.png"
materials: [
    { type: "document", name: "paper", url: "http://iribis.github.io/files/Stratified_Histogram_Resampling/paper.pdf" },
    { type: "url", name: "supp. mat.", url: "http://iribis.github.io/extra/Stratified_Histogram_Resampling/index.html"}
]
---

## Abstract

Monte Carlo (MC) rendering is a widely used approach for photorealistic image synthesis, yet real-time applications often limit sampling to one path per pixel, resulting in high noise levels. To mitigate this, resampled importance sampling (RIS) has shown promise by approximating ideal sample distributions through a discrete set of candidates, avoiding the complexity of neural models or data-intensive structures. However, current RIS techniques often rely on random sampling, which fails to maximize the potential of the candidate pool. We propose a two step approach that first organizes samples candidates into local histograms and then sample the histogram using Quasi Monte Carlo and antithetic patterns. This can be done with minimal overhead and allows to reduce error in rendering to increase visual quality. Additionally, we show how it can be combined with blue noise error distribution to perceptually reduce noise artifacts. Our approach yields a higher-quality resampling estimator with enhanced noise reduction, demonstrating significant improvements in real-time rendering tasks.