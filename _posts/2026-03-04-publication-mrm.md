---
layout: publication
date:   2026-03-04
title:  "The Minimal Retroreflective Microfacet Model"
authors: [
    {name: "Jamie Portsmouth", affiliation: "Autodesk"},
    {name: "Matthias Raab", affiliation: "NVIDIA"},
    {name: "Laurent Belcour"},
    {name: "Francis Liu", affiliation: "NVIDIA"},
]
conference: "JCGT"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2026_mrm.png"
materials: [
    { type: "document", name: "paper", url: "https://jcgt.org/published/0015/01/04/paper.pdf" },
    { type: "document", name: "supp. pdf", url: "https://jcgt.org/published/0015/01/04/supplemental.pdf" },
    { type: "url", name: "shadertoy", url: "https://www.shadertoy.com/view/tX3Gz8" }
]
---

<div style="display:flex; flex-direction:column; width:100%;">
    <span style="font-weight:600; margin-bottom:2px;">GGX</span>
    <div style="display:flex; justify-content: space-evenly; width:100%;">
        <div style="position:relative; width:31%;"><img style="width:100%; border:solid 1px black;" src="/images/posts/2026-publication-mrm/ggx_cone.jpg"></div>
        <div style="position:relative; width:31%;"><img style="width:100%; border:solid 1px black;" src="/images/posts/2026-publication-mrm/ggx_jacket.jpg"></div>
        <div style="position:relative; width:31%;"><img style="width:100%; border:solid 1px black;" src="/images/posts/2026-publication-mrm/ggx_shoe.jpg"></div>
    </div>
    <span style="font-weight:600; margin:6px 0 2px 0;">MRM</span>
    <div style="display:flex; justify-content: space-evenly; width:100%;">
        <div style="position:relative; width:31%;"><img style="width:100%; border:solid 1px black;" src="/images/posts/2026-publication-mrm/mrm_cone.jpg"></div>
        <div style="position:relative; width:31%;"><img style="width:100%; border:solid 1px black;" src="/images/posts/2026-publication-mrm/mrm_jacket.jpg"></div>
        <div style="position:relative; width:31%;"><img style="width:100%; border:solid 1px black;" src="/images/posts/2026-publication-mrm/mrm_shoe.jpg"></div>
    </div>
</div>
<p style="font-style: italic; margin-top:4px;">
Renderings of our MRM model (bottom row) obtained by an almost trivial modification of the equivalent roughness GGX microfacet model (top row). The lighting in all cases is aligned with the view direction, exhibiting a strong retroreflective peak in the MRM model.
</p>
<br />

<div style="display:flex; flex-wrap: nowrap; justify-content:space-around; width:100%;">
    <div style="width:47%;">
        <video loop controls style="width:100%; border:solid 1px black;">
            <source src="/videos/publication_2026_mrm_jacket_ggx.mp4" type="video/mp4">
        </video>
        <center><strong>GGX</strong></center>
    </div>
    <div style="width:47%;">
        <video loop controls style="width:100%; border:solid 1px black;">
            <source src="/videos/publication_2026_mrm_jacket_mrm.mp4" type="video/mp4">
        </video>
        <center><strong>MRM</strong></center>
    </div>
</div>
<br />

## Abstract

We describe the Minimal Retroreflective Microfacet (MRM) model, which provides a simple scheme for modifying a pre-existing microfacet BSDF implementation to produce a physically plausible retroreflective result. Based on the previously published back-vector formulation, MRM can be implemented with minimal changes to existing microfacet code, making it easy to integrate into existing rendering systems. We provide verification of reciprocity (under the assumption of a reflection-symmetric normal distribution function (NDF), which holds for all commonly used distributions) energy conservation, implementation details, and a comparison to measured data.
