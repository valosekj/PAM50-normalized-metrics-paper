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

This document is intended to provide: 

* Author list & affiliations
* A brief overview of the submission

Given that the actual preprint content will be generated in the `Jupyter Book` format by combining `Jupyter Notebooks` and `Markdown` files found at the `content` folder, we suggest keeping this document as brief as possible (about 1-2 pages). Nevertheles, it is at author's discretion to provide a longer `preprint.md` for creating the PDF that'll accompany the NeuroLibre Book.

# Mathematics

Single dollars ($) are required for inline mathematics e.g. $f(x) = e^{\pi/x}$

Double dollars make self-standing equations:

$$\Theta(x) = \left\{\begin{array}{l}
0\textrm{ if } x < 0\cr
1\textrm{ else}
\end{array}\right.$$

You can also use plain \LaTeX for equations
\begin{equation}\label{eq:fourier}
\hat f(\omega) = \int_{-\infty}^{\infty} f(x) e^{i\omega x} dx
\end{equation}
and refer to \autoref{eq:fourier} from text.

# Citations

Citations to entries in `preprint.bib` should be in
[rMarkdown](http://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html)
format.

For a quick reference, the following citation commands can be used:
* `@author:2021`  ->  "Author et al. (2021)"
* `[@author:2021]` -> "(Author et al., 2021)"
* `[@author1:2021; @author2:2001]` -> "(Author1 et al., 2021; Author2 et al., 2021)"

This is an example citation [@neurolibre:2021].

# Figures

Figures can be included like this:

![Caption for example figure.\label{fig:example}](images/example_figure.png)

You can reference figure from text using \autoref{fig:example}.

Figure sizes can be customized by adding an optional second parameter:

![Caption for example figure.](images/example_figure.png){ width=20% }

# Acknowledgements

NeuroLibre is sponsored by Canadian Open Neuroscience Platform (CONP), Brain Canada, Quebec Bioimaging Network, Cancer Computing and Healthy Brains & Healthy Life. 

# References
