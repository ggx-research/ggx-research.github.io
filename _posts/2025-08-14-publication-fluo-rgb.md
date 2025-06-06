---
layout: publication
date:   2025-08-14
title:  "A Fluorescent Material Model for Non-Spectral Editing & Rendering"
authors: [
    {name: "Laurent Belcour"},
    {name: "Alban Fichet"},
    {name: "Pascal Barla", affiliation: "INRIA", url: "https://www.labri.fr/perso/barla"},
]
conference: "ACM SIGGRAPH 2025"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'to_appear'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2025_fluo_rgb.png"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/pdf/2505.19672" },
]
---

<!-- <div style="display:flex; justify-content: space-evenly;">
    <div style="position:relative; width:80%;">
        <img style="width:100%; border:solid 1px black;" src="/images/posts/2024-publication-fluo-rgb/unity-blue.jpg">
        <span style="width:50%; text-align:left;  font-weight:600; font-size:2em; position:absolute; top:2%; left:2%; color:#FF0000;">Fluo OFF</span>
        <span style="width:50%; text-align:right; font-weight:600; font-size:2em; position:absolute; top:2%; right:2%; color:#00FF00;">Fluo ON</span>
    </div>
</div>
<div style="width:80%; padding-left:10%; padding-right:10%; font-style:italic; font-size:0.9em;">
We introduce a method to render fluorescent materials in a non-spectral rendererer, exhibiting typical increased luminance and hue-shifting effects when the same materials are placed under a different lighting. Our method is based on a new reduction technique that accurately matches the spectral reference, significantly improving on previous work where a naive formulation of the fluorescence reradiation matrix reduction was used.</div>
<br /> -->

## Abstract

Fluorescent materials are characterized by a spectral reradiation toward longer wavelengths.
Recent work <a href="https://ggx-research.github.io/publication/2024/06/03/publication-fluo-rgb.html">[Fichet2024]</a> has shown that the rendering of fluorescence in a non-spectral engine is possible through the use of appropriate reduced reradiation matrices. But the approach has limited expressivity, as it requires the storage of one reduced matrix per fluorescent material, and only works with measured fluorescent assets.

In this work, we introduce an analytical approach to the editing and rendering of fluorescence in a non-spectral engine. It is based on a decomposition of the reduced reradiation matrix, and an analytically-integrable Gaussian-based model of the fluorescent component. The model reproduces the appearance of fluorescent materials accurately, especially with the addition of a UV basis. Most importantly, it grants variations of fluorescent material parameters in real-time, either for the editing of fluorescent materials, or for the dynamic spatial variation of fluorescence properties across object surfaces. A simplified one-Gaussian fluorescence model even allows for the artist-friendly creation of plausible fluorescent materials from scratch, requiring only a few reflectance colors as input.