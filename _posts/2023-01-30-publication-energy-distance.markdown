---
layout: publication
date:   2023-01-30
title:  "The Energy Distance as a Replacement for the Reconstruction Loss in Conditional GANs"
authors: [
    {name: "Eric Heitz", affiliation: "Unity Technologies", url: ""},
    {name: "Thomas Chambon", affiliation: "Unity Technologies", url: ""}
]
conference: "JCGT 2023"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_2023_energy.png"
materials: [
    { type: "document", name: "paper", url: "https://jcgt.org/published/0012/01/02/" },
]
---

## Abstract
Conditional adversarial generative networks (cGANs) are often trained with a reconstruction loss in addition to the adversarial loss to compensate for its instability. However, reconstruction losses are known to conflict with the adversarial objective and prevent generating diverse outputs (mode collapse). 
This problem is acknowledged by the community but is either ignored or addressed with sophisticated approaches. 
We promote a surprisingly simple and yet unconsidered alternative: replacing the reconstruction loss by the energy distance. 
With a minor implementation modification, it solves the conflict problem with the adversarial objective, prevents mode collapse, and produces high-quality results in several image-processing tasks.