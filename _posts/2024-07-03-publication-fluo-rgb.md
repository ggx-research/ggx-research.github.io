---
layout: publication
date:   2024-06-03
title:  "Non-Orthogonal Reduction for Rendering Fluorescent Materials in Non-Spectral Engines"
authors: [
    {name: "Alban Fichet"},
    {name: "Laurent Belcour"},
    {name: "Pascal Barla", affiliation: "INRIA", url: "https://www.labri.fr/perso/barla"},
]
conference: "Computer Graphics Forum"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'to_appear'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2024_fluo_rgb.png"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/pdf/2406.17360" }
]
---

<div style="display:flex; justify-content: space-evenly;">
    <div style="position:relative; width:80%;">
        <img style="width:100%; border:solid 1px black;" src="/images/posts/2024-publication-fluo-rgb/unity-blue.jpg">
        <span style="width:50%; text-align:left;  font-weight:600; font-size:2em; position:absolute; top:2%; left:2%; color:#FF0000;">Fluo OFF</span>
        <span style="width:50%; text-align:right; font-weight:600; font-size:2em; position:absolute; top:2%; right:2%; color:#00FF00;">Fluo ON</span>
    </div>
</div>
<div style="width:80%; padding-left:10%; padding-right:10%; font-style:italic; font-size:0.9em;">
We introduce a method to render fluorescent materials in a non-spectral rendererer, exhibiting typical increased luminance and hue-shifting effects when the same materials are placed under a different lighting. Our method is based on a new reduction technique that accurately matches the spectral reference, significantly improving on previous work where a naive formulation of the fluorescence reradiation matrix reduction was used.</div>
<br />

## Abstract

We propose a method to accurately handle fluorescence in a non-spectral (*e.g.*, tristimulus) rendering engine, showcasing color-shifting and increased luminance effects. Core to our method is a principled reduction technique that encodes the re-radiation into a low-dimensional matrix working in the space of the renderer's Color Matching Functions (CMFs). Our process is independent of a specific CMF set and allows for the addition of a non-visible ultraviolet band during light transport. Our representation visually matches full spectral light transport for measured fluorescent materials even for challenging illuminants.