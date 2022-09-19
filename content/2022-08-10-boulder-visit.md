---
title: Using CESM2 and WACCM for synthetic volcanic eruption simulations
event: Boulder Visit
date: "2022-08-10"
revealOptions:
  allottedTime: 900000
---

## Using _CESM2_ and _WACCM_ for synthetic volcanic eruption simulations

--

### Eirik Rolland Enger

PhD candidate in the _complex systems modelling_ group at UiT The Arctic University of
Norway

---

## Outline

- Intro
  - Background / motivation <!-- .element class="fragment" -->
  - Method and model setup <!-- .element class="fragment" -->
- Results
  - Single-volcano events <!-- .element class="fragment" -->
  - Double-volcano events <!-- .element class="fragment" -->
  - Long simulations <!-- .element class="fragment" -->
- Issues
  - Seasonality <!-- .element class="fragment" -->
  - Expensive computations <!-- .element class="fragment" -->

---

## Intro

--

### Background and motivation

The FPP and deconvolution

--

<!-- .slide: data-background-color="#002f4b" -->
<!-- .slide: data-background-video-loop="true" -->
<!-- .slide: data-background-video="https://github.com/engeir/presentations-files/raw/9a4f6b9150206f27120130b18d8ac09f68469465/2021/fysikermotet/animation.mp4" -->
<!-- .slide: data-background-size="contain" -->

--

### Filtered Poisson Process

`
$$
T_K(t)=\sum_{k=1}^K A_k \phi\left( \frac{t-t_k}{\tau_\mathrm{d}} \right)
$$
`
`
$$
\downarrow \\
T_K(t)=[\phi*f_k]\left(\frac{t}{\tau_\mathrm{d}}\right)
$$
` <!-- .element class="fragment" -->

--

### Model setup

--

<a href="https://github.com/engeir/volcano-cooking#volcano-cooking" target="_blank"><img
data-src="https://opengraph.githubassets.com/0272a6274f1088fbd84c0a90f3d6d5abd7446f7e/engeir/volcano-cooking"></a>

---

## Results

--

### Single-volcano events

Text

--

### Double-volcano events

Text

--

### Long simulations

Text

---

## Issues

--

### Seasonality

- Strong seasonal variability
- Weaker effect at different temperature

--

### Expensive computations

> Model runs take a long time, thus one per season is not reasonable

---

<a href="https://www.glossa-journal.org/article/10.5334/gjgl.362/"
data-citation-key="@aikio2002">Moskal (2018)</a> shows that suppletion for the
exclusive happens only when the inclusive pronoun is also suppletive. This follows in
work on \*ABA patterns in suppletion in <a
href="https://mitpress.mit.edu/books/universals-comparative-morphology"
data-citation-key="@benvenuto2009">Bobaljik (2012)</a> and <a
href="https://link.springer.com/article/10.1007%2Fs11049-018-9425-0"
data-citation-key="@danabasoglu2020">Smith et al (2019)</a>

I also want to include @dong2019, but don't think that will work. Probably need <a
href="https://link.springer.com/article/10.1007%2Fs11049-018-9425-0"
data-citation-key="@gregory2016">Smith et al (2019)</a>
<!-- Start adding with revealjs-make-reflist -->
---
## References
<div class="csl-entry" id="ref-aikio2002" role="doc-biblioentry">
Aikio, A. T., T. Lakkala, A. Kozlovsky, and P. J. S. Williams. 2002. <span>“Electric Fields and Currents of Stable Drifting Auroral Arcs in the Evening Sector.”</span> <em>Journal of Geophysical Research: Space Physics</em> 107 (A12): SIA 3-1-SIA 3-14. <a href="https://doi.org/10.1029/2001ja009172">https://doi.org/10.1029/2001ja009172</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-benvenuto2009" role="doc-biblioentry">
Benvenuto, F, R Zanella, L Zanni, and M Bertero. 2009. <span>“Nonnegative Least-Squares Image Deblurring: Improved Gradient Projection Approaches.”</span> <em>Inverse Problems</em> 26 (2): 025004. <a href="https://doi.org/10.1088/0266-5611/26/2/025004">https://doi.org/10.1088/0266-5611/26/2/025004</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-danabasoglu2020" role="doc-biblioentry">
Danabasoglu, G., J.-F. Lamarque, J. Bacmeister, D. A. Bailey, A. K. DuVivier, J. Edwards, L. K. Emmons, et al. 2020. <span>“The Community Earth System Model Version 2 (<span>Cesm2</span>).”</span> <em>Journal of Advances in Modeling Earth Systems</em> 12 (2): e2019MS001916. https://doi.org/<a href="https://doi.org/10.1029/2019MS001916">https://doi.org/10.1029/2019MS001916</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-gregory2016" role="doc-biblioentry">
Gregory, J. M., T. Andrews, P. Good, T. Mauritsen, and P. M. Forster. 2016. <span>“Small Global-Mean Cooling Due to Volcanic Radiative Forcing.”</span> <em>Climate Dynamics</em> 47 (12): 3979–91. <a href="https://doi.org/10.1007/s00382-016-3055-1">https://doi.org/10.1007/s00382-016-3055-1</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<!-- End adding with revealjs-make-reflist -->
