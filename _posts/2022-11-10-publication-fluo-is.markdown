---
layout: publication
date:   2022-11-10
title:  " Efficient Storage and Importance Sampling for Fluorescent Reflectance"
authors: [
    {
        name: "Qingqin Hua",
        url: "https://qingqin-hua.com/",
        affiliation: "Saarland University"
    },
    {
        name: "Vojtěch Tázlar",
        url: "https://cgg.mff.cuni.cz/members/tazlarv/",
        affiliation: "Charles University"
    },
    {name: "Alban Fichet"},
    {
        name: "Alexander Wilkie",
        url: "https://cgg.mff.cuni.cz/~wilkie/Website/Home.html",
        affiliation: "Charles University"
    }
]
conference: "Computer Graphics Forum"
categories: publication
tags: published
thumbnail: "/images/thumbnails/publication_fluo_is.png"
materials: [
    { type: "document", name: "paper",     url: "https://hal.science/hal-03909700v1/document" },
    { type: "document", name: "supp. pdf", url: "https://hal.science/hal-03909700v1/file/Efficient-Storage-and-Importance-Sampling-for-Fluorescent-Reflectance-Supplemental.pdf" }
]
---

## Abstract
We propose a technique for efficient storage and importance sampling of fluorescent spectral data. Fluorescence is fully described by a re-radiation matrix, which for a given input wavelength indicates how much energy is re-emitted at other wavelengths. However, such representation has a considerable memory footprint. To significantly reduce memory requirements, we propose the use of Gaussian mixture models for the representation of re-radiation matrices. Instead of the full-resolution matrix, we work with a set of Gaussian parameters that also allow direct importance sampling. Furthermore, if accuracy is of concern, a re-radiation matrix can be used jointly with efficient importance sampling provided by the Gaussian mixture. In this paper, we present our pipeline for efficient storage of bispectral data and provide its extensive evaluation on a large set of bispectral measurements. We show that our method is robust and colour accurate even with its comparably minor memory requirements and that it can be seamlessly integrated into a standard Monte Carlo path tracer.