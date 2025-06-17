---
layout: publication
date:   2025-06-06
title:  "Adaptive Tetrahedral Grids for Volumetric Path-Tracing
"
authors: [
    {name: "Anis Benyoub"},
    {name: "Jonathan Dupuy"},
]
conference: "SIGGRAPH Talks 2025"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'to_appear'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2025_leb3d.png"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/abs/2506.11510" }
]
---

## Abstract

We advertise the use of tetrahedral grids constructed via the longest edge bisection algorithm for rendering volumetric data with path tracing. The key benefits of such grids is two-fold. First, they provide a highly adaptive space-partitioning representation that limits the memory footprint of volumetric assets. Second, each (tetrahedral) cell has exactly 4 neighbors within the volume (one per face of each tetrahedron) or less at boundaries. We leverage these properties to devise optimized algorithms and data-structures to compute and path-trace adaptive tetrahedral grids on the GPU. In practice, our GPU implementation outperforms regular grids by up to x30 and renders production assets in real time at 32 samples per pixel.

