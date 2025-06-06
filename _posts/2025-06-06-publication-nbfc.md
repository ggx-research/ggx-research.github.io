---
layout: publication
date:   2025-06-06
title:  "Hardware Accelerated Neural Block Texture Compression with Cooperative Vectors"
authors: [
    {name: "Laurent Belcour"},
    {name: "Anis Benyoub"},
]
conference: "HPG 2025"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'to_appear'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2025_nbfc.png"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/pdf/2505.19672" },
    { type: "video",    name: "video", url: "https://www.youtube.com/watch?v=8sy3QP1R-p8" },
]
---

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/8sy3QP1R-p8?si=BhK39NAj1_eKIfr_&amp;controls=1" title="YouTube video player" frameborder="0" style="border:solid black 1px;" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</center>

## Abstract

In this work, we present an extension to the neural texture compression method of <a href="https://arxiv.org/abs/2311.16121">Weinreich and colleagues [2024]</a>. Like them, we leverage existing block compression methods which permit to use hardware texture filtering to store a neural representation of physically-based rendering (PBR) texture sets (including albedo, normal maps, roughness, etc.). However, we show that low dynamic range block compression formats still make the solution viable. Thanks to this, we show that we can achieve higher compression ratio or higher quality at fixed compression ratio. We improve performance at runtime using a tile based rendering architecture that leverage hardware matrix multiplication engine. Thanks to all this, we render 4k textures sets (9 channels per asset) with anisotropic filtering at 1080p using only 28MB of VRAM per texture set at 0.55ms on an Intel B580.