---
title: Temperature response estimation from volcanic eruptions using CESM2 and WACCM6
event: Boulder Visit
date: "2022-09-30"
revealOptions:
  allottedTime: 900000
---

## Temperature response estimation from volcanic eruptions using _CESM2_ and _WACCM6_

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

<!-- .element class="r-fit-text" -->

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

$$
T\_K(t)=\sum_{k=1}^K A\_k \phi\left( \frac{t-t\_k}{\tau\_\mathrm{d}} \right)
$$

$$
\downarrow \\\\
T\_K(t)=[\phi\*f\_K]\left(\frac{t}{\tau_\mathrm{d}}\right)
$$

<!-- .element class="fragment" -->

--

### Deconvolution algorithm

$$
\phi^{(n+1)}=\phi^{(n)}\frac{(T\_K-\langle T\_K\rangle)\*\hat{f}\_K+b}{\phi^{(n)}\*f\_K\*\hat{f}\_K+b}
$$

--

### Model setup

1. Synthetic eruptions are given to WACCM6
2. Run using the **BWma1850** compset

Notes:

The middle atmosphere (MA) chemistry is capable of calculating the evolution of
stratospheric aerosol from SO2 emissions from large volcanic eruptions. WACCM with MA
can only run at nominal $2^\circ$ resolution, while the more expensive TSMLT1
(troposphere, stratosphere, mesosphere and lower thermosphere) can go down to nominal
$1^\circ$ resolution.

--

<a href="https://github.com/engeir/volcano-cooking#volcano-cooking" target="_blank"><img
data-src="https://opengraph.githubassets.com/0272a6274f1088fbd84c0a90f3d6d5abd7446f7e/engeir/volcano-cooking"></a>

---

## Results

<!-- .element class="r-fit-text" -->

--

<!-- .slide: data-transition="slide-in fade-out" -->

### Single-volcano events

<!-- .element class="r-fit-text" -->

--

<!-- .slide: data-transition="fade-in fade-out" -->

| <div class="fragment grow" data-fragment-index="0"><div class="fragment shrink" data-fragment-index="1"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/e9fbe3577899d750c61cb4478155ce0b48d48570/assets/pic/volcano-ensemble-waveforms/medium-waveform.png" ></div></div> | <div class="fragment grow" data-fragment-index="1"><div class="fragment shrink" data-fragment-index="2"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/e9fbe3577899d750c61cb4478155ce0b48d48570/assets/pic/volcano-ensemble-waveforms/medium-plus-waveform.png" ></div></div> | <div class="fragment grow" data-fragment-index="2"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/e9fbe3577899d750c61cb4478155ce0b48d48570/assets/pic/volcano-ensemble-waveforms/strong-waveform.png" ></div> |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

--

<!-- .slide: data-transition="fade-in slide-out" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/hack-md-notes/abf78e1fcd784f3c57c73c107dc193c5c34c25f8/assets/pic/volcano-ensemble-waveforms/compare-waveform-integrate.png" -->

--

<!-- .slide: data-transition="fade" -->

| <div class="fragment grow" data-fragment-index="0"><div class="fragment shrink" data-fragment-index="1"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/4987583ac7a9a34e08bca2eda1392ae45090e128/assets/pic/volcano-zonal-mean/zonal-mean1-trefht-strong.png" ></div></div> | <div class="fragment grow" data-fragment-index="1"><div class="fragment shrink" data-fragment-index="2"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/4987583ac7a9a34e08bca2eda1392ae45090e128/assets/pic/volcano-zonal-mean/zonal-mean3-trefht-strong.png" ></div></div> | <div class="fragment grow" data-fragment-index="2"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/4987583ac7a9a34e08bca2eda1392ae45090e128/assets/pic/volcano-zonal-mean/zonal-mean6-trefht-strong.png" ></div> |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

Notes:

The volcanoes influence the hemispheres differently depending on when within the year
they appear, but the effect does not last very long (about 3 years).

This is interesting since it might point to that, even though volcanoes from different
hemispheres spread differently and cool differently, the effect lasts only for a few
years. Thus, the tail might be similar for NH and SH eruptions, which is also where the
information we are looking for lies.

--

<!-- .slide: data-transition="fade" -->

<img width="49%" src="https://raw.githubusercontent.com/engeir/hack-md-notes/15d48cd3fe9d0abbb49c20d41d6ade6f8e4e7e27/assets/pic/volcano-zonal-mean/zonal-mean-aerodv-may-medium.png">
<img width="49%" src="https://raw.githubusercontent.com/engeir/hack-md-notes/15d48cd3fe9d0abbb49c20d41d6ade6f8e4e7e27/assets/pic/volcano-zonal-mean/zonal-mean-aerodv-nov-medium.png">

_Total aerosol optical depth in visible band_
<!-- .element: style="font-size:20pt" -->

Notes:

Here we pick out the two most different simulation and look at their aerosol optical
depth. (_Total aerosol optical depth in visible band_.)

We see that aerosol tend to spread to the winter hemisphere, but that after a couple of
years it is mostly gone.

--

<!-- .slide: data-transition="slide-in fade-out" -->

### Double-volcano events

<!-- .element class="r-fit-text" -->

--

<!-- .slide: data-transition="fade-in slide-out" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/hack-md-notes/a19bdfc5ad051cd259bd9741e67e1bf3ebe1e718/assets/pic/double-overlap/double-overlap-superpose.png" -->

--

Problem: simulations are not long enough to have a periodic signal

--

<!-- .slide: data-transition="slide-in fade-out" -->

### Long simulations

<!-- .element class="r-fit-text" -->

--

<!-- .slide: class="data-auto-animate" -->
<!-- .slide: data-transition="fade" -->

<div class="r-stack">
  <p class="fragment animated move-to" data-animated-move-to-top="-250px" data-animated-move-to-left="0px" data-fragment-index="0" data-animated-duration="300" data-animated-iterations="1" data-animated-fill="forwards">
  Using the <a target="_blank" href="https://www.cesm.ucar.edu/projects/community-projects/LME/">CESM LME</a> data set
  </p>
  <span>
  <img class="fragment fade-in" data-fragment-index="0" src="https://raw.githubusercontent.com/engeir/hack-md-notes/6c20ab748912530c65e30e648c04b4e45a55b838/assets/pic/deconv-cesm-lme/cesm_lme_deconvolution_ensall_mean_forcing.png" width="49%" >
  <img class="fragment fade-in" data-fragment-index="0" src="https://raw.githubusercontent.com/engeir/hack-md-notes/6c20ab748912530c65e30e648c04b4e45a55b838/assets/pic/deconv-cesm-lme/cesm_lme_deconvolution_ensall_mean_temperature.png" width="49%" >
  </span>
</div>

Notes:

But this was run with CESM1, and more importantly with **CAM5**, hence with a low-top
atmosphere reaching only to about $40\\,\mathrm{km}$. They also use $2^\circ$ resolution
for the atmosphere and land components, which for now is the same as I do, but possibly
$1^\circ$ will be needed.

--

<!-- .slide: data-transition="fade" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/hack-md-notes/6c20ab748912530c65e30e648c04b4e45a55b838/assets/pic/deconv-cesm-lme/cesm_lme_deconvolution_ensall_mean-respnse.png" -->
<!-- .slide: data-background-size="contain" -->

---

## Issues

<!-- .element class="r-fit-text" -->

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
<!-- Generated by revealjs-make-reflist. Do not edit. -->

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

--

<div class="csl-entry" id="ref-gregory2016" role="doc-biblioentry">
Gregory, J. M., T. Andrews, P. Good, T. Mauritsen, and P. M. Forster. 2016. <span>“Small Global-Mean Cooling Due to Volcanic Radiative Forcing.”</span> <em>Climate Dynamics</em> 47 (12): 3979–91. <a href="https://doi.org/10.1007/s00382-016-3055-1">https://doi.org/10.1007/s00382-016-3055-1</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<!-- End adding with revealjs-make-reflist -->
