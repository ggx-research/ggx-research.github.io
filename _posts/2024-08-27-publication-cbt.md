---
layout: publication
date:   2024-07-27
title:  "Concurrent Binary Trees for Large-Scale Game Components"
authors: [
    {name: "Anis Benyoub"},
    {name: "Jonathan Dupuy" },
]
conference: "HPG 2024"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'to_appear'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2024_cbt.jpg"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/abs/2407.02215" },
    { type: "code", name: "code", url: "https://github.com/AnisB/large_cbt" }
]
---
## Abstract

A concurrent binary tree (CBT) is a GPU-friendly data-structure suitable for the generation of bisection based terrain tessellations, i.e., adaptive triangulations over square domains. In this paper, we expand the benefits of this data-structure in two respects. First, we show how to bring bisection based tessellations to arbitrary polygon meshes rather than just squares. Our approach consists of mapping a triangular subdivision primitive, which we refer to as a bisector, to each halfedge of the input mesh. These bisectors can then be subdivided adaptively to produce conforming triangulations solely based on halfedge operators. Second, we alleviate a limitation that restricted the triangulations to low subdivision levels. We do so by using the CBT as a memory pool manager rather than an implicit encoding of the triangulation as done originally. By using a CBT in this way, we concurrently allocate and/or release bisectors during adaptive subdivision using shared GPU memory. We demonstrate the benefits of our improvements by rendering planetary scale geometry out of very coarse meshes. Performance-wise, our triangulation method evaluates in less than 0.2ms on console-level hardware. 
