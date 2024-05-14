---
layout: publication
date:   2024-04-17
title:  "Transforming a Non-Differentiable Rasterizer into a Differentiable One with Stochastic Gradient Estimation"
authors: [
    {name: "Thomas Deliot"},
    {name: "Eric Heitz"},
    {name: "Laurent Belcour"},
]
conference: "I3D 2024"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2024_intel_diffrast.png"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/abs/2404.09758" },
    { type: "video", name: "video", url: "https://www.youtube.com/watch?v=hoFL0QGrqDg" },
    { type: "code", name: "code", url: "https://drive.google.com/file/d/1FUVUyctYzZVHij6f8lS7scMbQzg1CeN6/view?usp=sharing"},
]
award: [
    "Best paper #2",
    "Best presentation"
]
---


<div style="display:flex; flex-wrap: nowrap; justify-content:space-around; width:100%;;">
    <video loop controls style="width:30%; border:solid 1px black;">
        <source src="/videos/publication_2024_intel_diffrast_video_0.mp4" type="video/mp4">
    </video>
    <video loop controls style="width:30%; border:solid 1px black;">
        <source src="/videos/publication_2024_intel_diffrast_video_1.mp4" type="video/mp4">
    </video>
    <video loop controls style="width:30%; border:solid 1px black;">
        <source src="/videos/publication_2024_intel_diffrast_video_2.mp4" type="video/mp4">
    </video>
</div>
<br />

## Abstract

We show how to transform a non-differentiable rasterizer into a differentiable one with minimal engineering efforts and no external dependencies (no Pytorch/Tensorflow). We rely on Stochastic Gradient Estimation, a technique that consists of rasterizing after randomly perturbing the scene’s parameters such that their gradient can be stochastically estimated and descended. This method is simple and robust but does not scale in dimensionality (number of scene parameters). Our insight is that the number of parameters contributing to a given rasterized pixel is bounded. Estimating and averaging gradients on a per-pixel basis hence bounds the dimensionality of the underlying optimization problem and makes the method scalable. Furthermore, it is simple to track per-pixel contributing parameters by rasterizing ID- and UV-buffers, which are trivial additions to a rasterization engine if not already available. With these minor modifications, we obtain an in-engine optimizer for 3D assets with millions of geometry and texture parameters.

<center style="width:100%; border: solid 1px black;">
    <embed
        src="https://www.youtube.com/embed/hoFL0QGrqDg?si=GzYuKYBLSX3-EgVY"
        type="video/mp4"
        allow="autoplay; encrypted-media; picture-in-picture"
        allowfullscreen
        style="width:100%; height:calc(26cqw); overflow:auto; resize:horizontal;"
    >
</center>