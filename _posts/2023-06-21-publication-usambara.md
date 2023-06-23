---
layout: publication
date:   2023-06-21
title:  "One-to-Many Spectral Upsampling of Reflectances and Transmittances"
authors: [
    {name: "Laurent Belcour"},
    {name: "Pascal Barla", affiliation: "INRIA", url: "https://www.labri.fr/perso/barla"},
    {name: "Gael Guennebaud", affiliation: "INRIA", url: "http://www.labri.fr/perso/guenneba/"},
]
conference: "EGSR 2023"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2023_usambara.png"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/abs/2306.11464" },
]
---

<div style="display:flex; justify-content: space-evenly;">
<div style="position:relative; width:40%;">
    <img width="512px" style="width:100%; border:solid 1px black;" src="/images/posts/2023-publication-usambara/usambara.png">
    <span style="width:50%; text-align:center; font-family:linux-libertine; font-weight:600; font-size:0.8em; position:absolute; top:5%; left:0%; color:#ff7f0eff;">Usambara effect</span>
    <span style="width:50%; text-align:center; font-family:linux-libertine; font-weight:600; font-size:0.8em; position:absolute; top:5%; left:50%; color:#2ca02cff;">Saturation effect</span>
    <img width="512px" style="width:91%; position:absolute; top:58%; left:7%;" src="/images/posts/2023-publication-usambara/spectrum.svg">
</div>
    <img width="512px" style="width:44%;" src="/images/posts/2023-publication-usambara/chroma.svg">
</div>
<div style="width:90%; padding-left:5%; padding-right:5%; font-style:italic; font-size:0.9em;">
We introduce a method to generate many spectra with the same chromaticity under a given illuminant. We show how to apply this technique to either reproduce spectra mimicking the Usambara effect, a form of vathochromism (change of chrominance with respect to optical depth, on the left) or a simple saturating spectra (on the right).
</div>
<br />

## Abstract

Spectral rendering is essential for the production of physically-plausible synthetic images, but requires to introduce several changes in the content generation pipeline. In particular, the authoring of spectral material properties (e.g., albedo maps, indices of refraction, transmittance coefficients) raises new problems.While a large panel of computer graphics methods exists to upsample a RGB color to a spectrum, they all provide a one-to-one mapping. This limits the ability to control interesting color changes such as the Usambara effect or metameric spectra. In this work, we introduce a one-to-many mapping in which we show how we can explore the set of all spectra reproducing a given input color. We apply this method to different colour changing effects such as vathochromism -- the change of color with depth, and metamerism. 