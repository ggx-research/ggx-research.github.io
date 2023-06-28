---
layout: publication
date:   2023-06-09
title:  "Sampling Visible GGX Normals with Spherical Caps"
authors: [
    {name: "Jonathan Dupuy" },
    {name: "Anis Benyoub"},
]
conference: "HPG 2023"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2023_ggx.jpg"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/abs/2306.05044" },
    { type: "url", name: "code", url: "https://gist.github.com/jdupuy/4c6e782b62c92b9cb3d13fbb0a5bd7a0" },
]
award: "Best paper #2"
---
## Abstract
Importance sampling the distribution of visible GGX normals requires sampling those of a hemisphere. In this work, we introduce a novel method for sampling such visible normals. Our method builds upon the insight that a hemispherical mirror reflects parallel light rays uniformly within a solid angle shaped as a spherical cap. This spherical cap has the same apex as the hemispherical mirror, and its aperture given by the angle formed by the orientation of that apex and the direction of incident light rays. Based on this insight, we sample GGX visible normals as halfway vectors between a given incident direction and directions drawn from its associated spherical cap. Our resulting implementation is even simpler than that of Heitz and leads to systematic speed-ups in our benchmarks. 
