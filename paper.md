---
title: 'A database of the healthy human spinal cord morphometry in the PAM50 template space'
tags:
  - spinal cord
  - morphometric measures 
  - normative values
  - open-source
authors:
  - name: Jan Valošek
    orcid: 0000-0002-7398-4990
    affiliation: "1, 2, 3, 4"
  - name: Sandrine Bédard
    orcid: 0000-0001-9859-1133
    affiliation: "1"
  - name: Miloš Keřkovský
    orcid: 0000-0003-0587-9897
    affiliation: "5"
  - name: Tomáš Rohan
    orcid: 0000-0002-7105-583X
    affiliation: "5"
  - name: Julien Cohen-Adad
    orcid: 0000-0003-3662-9532
    affiliation: "1, 2, 6, 7"
affiliations:
  - name: NeuroPoly Lab, Institute of Biomedical Engineering, Polytechnique Montreal, Montreal, QC, Canada
    index: 1
  - name: Mila - Quebec AI Institute, Montreal, QC, Canada
    index: 2
  - name: Department of Neurosurgery, Faculty of Medicine and Dentistry, Palacký University Olomouc, Olomouc, Czechia
    index: 3
  - name: Department of Neurology, Faculty of Medicine and Dentistry, Palacký University Olomouc, Olomouc, Czechia
    index: 4
  - name: Department of Radiology and Nuclear Medicine, University Hospital Brno and Masaryk University, Brno, Czechia
    index: 5
  - name: Functional Neuroimaging Unit, CRIUGM, Université de Montréal, Montreal, QC, Canada
    index: 6
  - name: Centre de recherche du CHU Sainte-Justine, Université de Montréal, Montreal, QC, Canada
    index: 7
date: 16 August 2023
bibliography: paper.bib
---

# Summary

Spinal cord morphometry measures derived from magnetic resonance imaging (MRI) scans serve as valuable prognostic biomarkers 
for various spinal cord pathologies. Despite their significance, interpreting these biomarkers is challenging due to substantial 
variability between subjects. The lack of a standardized normalization method to mitigate this variability and the need for a 
better understanding of morphometric distribution contribute to the current knowledge gap.

In this work, we present a database of healthy normative values for six commonly used measures of spinal cord morphometry built 
using a new fully-automatic normalization approach. Morphometric measures were computed from a large open-access dataset of 
healthy adult volunteers (N = 203) and brought to the common space of the PAM50 spinal cord template using a newly proposed 
normalization method based on linear interpolation \autoref{fig:figure1}.

The database is interactive, available online (TODO: add a link to interactive preprint) and allows filtering for sex, age, 
and MRI vendors. The proposed method is open-source and easily accessible through the Spinal Cord Toolbox (SCT) v6.0 and higher. 

This new morphometric database allows researchers to normalize morphometrics based on sex and age, thereby minimizing inter-subject 
variability associated with demographic and biological factors.

# Figures

![Schematic representation of the normalization approach. (A) T2-weighted images of 203 participants from the Spine Generic 
Public Database (multi-subject) were used. The spinal cord was segmented, and vertebral levels were identified automatically 
using the Spinal Cord Toolbox (SCT). (B) Six morphometric measures were computed for each axial slice from the single-subject 
segmentation masks. (C) For each level, the number of slices in the subject native space and the corresponding level in the PAM50 
template (D) were identified. Then, the morphometric measures were linearly interpolated to the PAM50 space using the number of 
slices in the PAM50 template and the subject native space for each vertebral level.\label{fig:figure1}](normalization_diagram.png){ width=80% }

# Acknowledgements

Thanks to Nick Guenther and Mathieu Guay-Paquet for their assistance with dataset management. We would like to thank Joshua Newton for his contributions in helping us implement the algorithm to SCT. We express our gratitude to Allan R. Martin for his insightful discussions on the clinical aspects of the work. We would also like to thank Nathan Molinier for providing valuable feedback on the manuscript figures. We acknowledge all participants as well as collaborators of the _spine-generic_ study.

Funded by the Canada Research Chair in Quantitative Magnetic Resonance Imaging [CRC-2020-00179], the Canadian Institute of Health Research [PJT-190258], the Canada Foundation for Innovation [32454, 34824], the Fonds de Recherche du Québec - Santé [322736], the Natural Sciences and Engineering Research Council of Canada [RGPIN-2019-07244], the Canada First Research Excellence Fund (IVADO and TransMedTech), the Courtois NeuroMod project, the Quebec BioImaging Network [5886, 35450], INSPIRED (Spinal Research, UK; Wings for Life, Austria; Craig H. Neilsen Foundation, USA), Mila - Tech Transfer Funding Program. Supported by the Ministry of Health of the Czech Republic, grant nr. NU22-04-00024. All rights reserved. JV has received funding from the European Union's Horizon Europe research and innovation programme under the Marie Sktodowska-Curie grant agreement No 101107932.

# References
