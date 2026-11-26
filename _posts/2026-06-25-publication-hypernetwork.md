---
layout: publication
date:   2026-06-25
title:  "Neural Texture Compression using Hypernetworks"
authors: [
    {name: "Laurent Belcour"},
]
conference: "EGSR 2026"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2026_hypernetwork.png"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/abs/2606.26913" },
    { type: "code",     name: "code",  url: "https://github.com/belcour/egsr2026_hypernetwork" },
    { type: "document", name: "model", url: "https://huggingface.co/belcour/egsr2026_hypernetwork" },
    { type: "url",      name: "demo",  url: "https://huggingface.co/spaces/belcour/hypernetwork" },
    { type: "video",    name: "slides",url: "https://www.youtube.com/watch?v=jXAhFuz9E9w" },
]
---

<div style="display:flex; justify-content: space-evenly;">
    <div style="position:relative; width:100%;">
        <img style="width:100%;" src="/images/posts/2026-publication-hypernetwork/teaser.jpg">
    </div>
</div>
<br />

## Abstract

Recent work on neural texture compression has demonstrated that it is possible to learn small, per-material texture representations (composed of latent textures and a small Multi-Layer Perceptron decoder) that can be decoded in real-time during shading to reproduce the input to a physically based shading model. However, existing methods require performing gradient-descent optimization per material for a given MLP and latent configuration. In this work, we train a single hypernetwork that outputs both the latent features and the MLP's weights and biases. Though the solution space is high-dimensional, this approach produces results comparable in quality to the current reference neural texture compressors. We further extend this approach to infer multiple decoders at once or even produce decoders that learn super-resolution.
