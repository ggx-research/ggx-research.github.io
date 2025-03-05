---
layout: publication
date:   2025-03-04
title:  "Compression of Spectral Images using Spectral JPEG XL"
authors: [
    {name: "Alban Fichet"},
    {name: "Christoph Peters", affiliation: "Intel Corporation", url: "https://momentsingraphics.de"},
]
conference: "JCGT"
categories: publication
# Add a tag to display in the website
# Valid tags are: 'published', 'to_appear', 'techreport'
tags: 'published'
# Thumbnails should be 128x128 max
thumbnail: "/images/thumbnails/publication_spectral_jxl.png"
materials: [
    { type: "document", name: "paper", url: "https://jcgt.org/published/0014/01/04/paper.pdf" },
    { type: "document", name: "supp. pdf", url: "https://jcgt.org/published/0014/01/04/supplemental.pdf" },
    { type: "code", name: "code", url: "https://github.com/afichet/spectral-compress" }
]
---

<div style="display:flex; justify-content: space-evenly;">
    <div style="position:relative; width:100%;">
        <img style="width:100%;" src="/images/posts/2025-publication-spectral-jxl/teaser.png">
    </div>
</div>
<br />

## Abstract

We propose a method to accurately handle fluorescence in a non-spectral (*e.g.*, tristimulus) rendering engine, showcasing color-shifting and increased luminance effects. Core to our method is a principled reduction technique that encodes the re-radiation into a low-dimensional matrix working in the space of the renderer's Color Matching Functions (CMFs). Our process is independent of a specific CMF set and allows for the addition of a non-visible ultraviolet band during light transport. Our representation visually matches full spectral light transport for measured fluorescent materials even for challenging illuminants.
The advantages of spectral rendering are increasingly well known, and corresponding rendering algorithms have matured. In this context, spectral images are used as input (e.g., reflectance and emission textures) and output of a renderer. Their large memory footprint is one of the big remaining issues with spectral rendering. Our method applies a cosine transform in the wavelength domain. We then reduce the dynamic range of higher-frequency Fourier coefficients by dividing them by the mean brightness, i.e., the Fourier coefficient for frequency zero. Then we store all coefficient images using JPEG XL. The mean brightness is perceptually most important and we store it with high quality. At higher frequencies, we use higher compression ratios and optionally lower resolutions. Our format supports the full feature set of spectral OpenEXR, but compared to this lossless compression, we achieve file sizes that are 10 to 60 times smaller than their ZIP compressed counterparts.