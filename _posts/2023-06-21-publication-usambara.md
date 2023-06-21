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


## Abstract

Spectral rendering is essential for the production of physically-plausible synthetic images, but requires to introduce several changes in the content generation pipeline. In particular, the authoring of spectral material properties (e.g., albedo maps, indices of refraction, transmittance coefficients) raises new problems.While a large panel of computer graphics methods exists to upsample a RGB color to a spectrum, they all provide a one-to-one mapping. This limits the ability to control interesting color changes such as the Usambara effect or metameric spectra. In this work, we introduce a one-to-many mapping in which we show how we can explore the set of all spectra reproducing a given input color. We apply this method to different colour changing effects such as vathochromism -- the change of color with depth, and metamerism. 