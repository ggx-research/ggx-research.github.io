---
layout: publication
date:   2023-06-09
title:  "Real-Time Rendering of Glinty Appearances using Distributed Binomial Laws on Anisotropic Grids"
authors: [
    {name: "Thomas Deliot" },
    {name: "Laurent Belcour"},
]
conference: "HPG 2023"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2023_glints.jpg"
materials: [
    { type: "document", name: "paper", url: "https://arxiv.org/abs/2306.05051" },
    { type: "video", name: "video", url: "https://www.youtube.com/watch?v=hsBacmXO08I" },
    { type: "code",  name: "code",  url: "https://drive.google.com/file/d/1YQDxlkZFEwV6ZeaXCUYMhB4P-3ODS32e/view?usp=drive_link"},
    { type: "code",  name: "demo",  url: "https://drive.google.com/file/d/1QonFDpE8FNaX7wk_CPniq4JPR0r4syON/view?usp=drive_link"},
    { type: "code",  name: "demo (teaser)",  url: "https://drive.google.com/file/d/1lfxNI7o7mqbJLDQnc3LBVPIjnIBU92PD/view?usp=drive_link"},
]
---


## Abstract

In this work, we render in real-time glittery materials caused by  discrete flakes on the surface. To achieve this, one has to count the  number of flakes reflecting the light towards the camera within every  texel covered by a given pixel footprint. To do so, we derive a counting  method for arbitrary footprints that, unlike previous work, outputs the  correct statistics. We combine this counting method with an anisotropic  parameterization of the texture space that reduces the number of texels  falling under a pixel footprint. This allows our method to run with  both stable performance and 1.5× to 5× faster than the state-of-the-art.

<center style="width:100%;">
    <embed
        src="https://www.youtube.com/embed/hsBacmXO08I"
        type="video/mp4"
        allow="autoplay; encrypted-media; picture-in-picture"
        allowfullscreen
        style="width:100%; height:calc(26cqw); overflow:auto; resize:horizontal;"
    >
</center>
<br />