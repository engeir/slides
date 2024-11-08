---
title: Temperature response estimation from volcanic eruptions using CESM2 and WACCM6
event: Boulder Visit
date: "2022-09-30"
revealOptions:
  allottedTime: 2_400_000
---

## Temperature response estimation from volcanic eruptions using _CESM2_ and _WACCM6_

--

### Eirik Rolland Enger

PhD candidate in the _complex systems modelling_ group at UiT The Arctic University of
Norway

---

## Outline

- Intro
  - Background / motivation <!-- .element class="fragment" data-fragment-index="0" -->
  - Method and model setup <!-- .element class="fragment" data-fragment-index="0" -->
- Results
  - Single-volcano events <!-- .element class="fragment" data-fragment-index="1" -->
  - Double-volcano events <!-- .element class="fragment" data-fragment-index="1" -->
- Outlook
  - Long simulations <!-- .element class="fragment" data-fragment-index="2" -->

---

## Intro

<!-- .element class="r-fit-text" -->

--

<!-- .slide: data-transition="slide-in fade-out" -->

### Background and motivation

The FPP and deconvolution

--

<!-- .slide: data-background-color="#002f4b" -->
<!-- .slide: data-background-video-loop="true" -->
<!-- .slide: data-background-video="https://github.com/engeir/presentations-files/raw/9a4f6b9150206f27120130b18d8ac09f68469465/2021/fysikermotet/animation.mp4" -->
<!-- .slide: data-background-size="contain" -->

--

<!-- .slide: data-transition="fade" -->

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

<!-- .slide: data-transition="fade" -->

### Deconvolution algorithm

$$
\phi^{(n+1)}=\phi^{(n)}\frac{(T\_K-\langle T\_K\rangle)\*\hat{f}\_K+b}{\phi^{(n)}\*f\_K\*\hat{f}\_K+b}
$$

<a href="https://doi.org/" data-citation-key="@richardson1972">Richardson (1972)</a>,
<a href="https://doi.org/10.1086/111605" data-citation-key="@lucy1974">Lucy (1974)</a>,
<a href="https://doi.org/10.1088/0266-5611/26/2/025004" data-citation-key="@benvenuto2009">Benvenuto
et al. (2009)</a>

<!-- .element: style="font-size:13pt" -->

--

<!-- .slide: data-transition="fade-in slide-out" -->

### Phenomenological model for intermittent processes

1. Stationarity <!-- .element class="fragment" -->
2. Linearity <!-- .element class="fragment" -->

--

<!-- .slide: data-transition="slide-in fade-out" -->

### Model setup

1. Synthetic eruptions are given to CESM2
2. Run using the BWma1850 compset
   <!-- .element: class="fragment" data-fragment-index="1" -->

<a href="https://github.com/engeir/volcano-cooking#volcano-cooking" target="_blank"><img
width="80%"
data-src="https://opengraph.githubassets.com/0272a6274f1088fbd84c0a90f3d6d5abd7446f7e/engeir/volcano-cooking"></a>

<!-- .element: class="fragment" data-fragment-index="0" -->

Notes:

What we want is to run CESM2 with custom synthetic volcanoes while the rest of the
climate system stay unforced by external factors.

Made a Python project to create the volcanic forcing files. Uses the
**createVolcEruptV3.ncl** script from
[svn.code.sf.net](http://svn.code.sf.net/p/codescripts/code/trunk/ncl/emission/) to
convert from the source files.

The middle atmosphere (MA) chemistry is capable of calculating the evolution of
stratospheric aerosol from SO2 emissions from large volcanic eruptions. WACCM with MA
can only run at nominal 2° resolution, while the more expensive TSMLT1 (troposphere,
stratosphere, mesosphere and lower thermosphere) can go down to nominal 1° resolution.

---

## Results

<!-- .element class="r-fit-text" -->

--

<!-- .slide: data-transition="slide-in fade-out" -->

### Single-volcano events

<!-- .element class="r-fit-text" -->

--

<!-- .slide: data-transition="fade-in fade-out" -->

<!-- dprint-ignore-start -->
| <div class="fragment grow" data-fragment-index="0"><div class="fragment shrink" data-fragment-index="1"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/e9fbe3577899d750c61cb4478155ce0b48d48570/assets/pic/volcano-ensemble-waveforms/medium-waveform.png" ></div></div> | <div class="fragment grow" data-fragment-index="1"><div class="fragment shrink" data-fragment-index="2"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/e9fbe3577899d750c61cb4478155ce0b48d48570/assets/pic/volcano-ensemble-waveforms/medium-plus-waveform.png" ></div></div> | <div class="fragment grow" data-fragment-index="2"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/e9fbe3577899d750c61cb4478155ce0b48d48570/assets/pic/volcano-ensemble-waveforms/strong-waveform.png" ></div> |
| :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| $26\\,\mathrm{Tg}$ <!-- .element: style="font-size:20pt" --> | $400\\,\mathrm{Tg}$ <!-- .element: style="font-size:20pt" --> | $1629\\,\mathrm{Tg}$ <!-- .element: style="font-size:20pt" --> |
<!-- dprint-ignore-end -->

Notes:

The smallest eruption is comparable in size to the Mt. Pinatubo eruption. The Young(est)
Toba Tuff eruption (∼74000 years ago) has an estimated sulphur dioxide amount of 5400
Tg, more than the strongest simulated here.

Ensemble medians of four simulations with eruptions spaced with three months, one in
each season.

--

<!-- .slide: data-transition="fade-in slide-out" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/hack-md-notes/abf78e1fcd784f3c57c73c107dc193c5c34c25f8/assets/pic/volcano-ensemble-waveforms/compare-waveform-integrate.png" -->

Notes:

We here look at the waveform of the temperature, to see if a clear difference between
the shapes, and in particular the tails, can be found. The two strongest eruptions
produce temperature responses that are similar in shape, while the weakest has a sharper
peak. However, this difference is not conclusive, and the tail is also close to the two
stronger eruptions.

--

<!-- .slide: data-transition="fade" -->

<!-- dprint-ignore-start -->
| <div class="fragment grow" data-fragment-index="0"><div class="fragment shrink" data-fragment-index="1"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/4987583ac7a9a34e08bca2eda1392ae45090e128/assets/pic/volcano-zonal-mean/zonal-mean1-trefht-strong.png" ></div></div> | <div class="fragment grow" data-fragment-index="1"><div class="fragment shrink" data-fragment-index="2"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/4987583ac7a9a34e08bca2eda1392ae45090e128/assets/pic/volcano-zonal-mean/zonal-mean3-trefht-strong.png" ></div></div> | <div class="fragment grow" data-fragment-index="2"><img src="https://raw.githubusercontent.com/engeir/hack-md-notes/4987583ac7a9a34e08bca2eda1392ae45090e128/assets/pic/volcano-zonal-mean/zonal-mean6-trefht-strong.png" ></div> |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| $1\\,\mathrm{yr}$ <!-- .element: style="font-size:20pt" --> | $3\\,\mathrm{yr}$ <!-- .element: style="font-size:20pt" --> | $6\\,\mathrm{yr}$ <!-- .element: style="font-size:20pt" --> |
<!-- dprint-ignore-end -->

Notes:

This show longitude and time averages from the time of the eruption until 1, 3 and 6
years have passed, respectively.

The volcanoes influence the hemispheres differently depending on when within the year
they appear, but the effect does not last very long (about 3 years).

This is interesting since it might point to that, even though volcanoes from different
hemispheres spread differently and cool differently, the effect lasts only for a few
years. Thus, the tail might be similar for NH and SH eruptions, which is also where the
information we are looking for lies.

--

<!-- .slide: data-transition="fade-in slide-out" -->

<img
  width="49%"
  src="https://raw.githubusercontent.com/engeir/hack-md-notes/15d48cd3fe9d0abbb49c20d41d6ade6f8e4e7e27/assets/pic/volcano-zonal-mean/zonal-mean-aerodv-may-medium.png"
/>
<img
  width="49%"
  src="https://raw.githubusercontent.com/engeir/hack-md-notes/15d48cd3fe9d0abbb49c20d41d6ade6f8e4e7e27/assets/pic/volcano-zonal-mean/zonal-mean-aerodv-nov-medium.png"
/> _Total aerosol optical depth in visible band_

<!-- .element: style="font-size:20pt" -->

Notes:

Here we pick out the two most different simulation and look at their aerosol optical
depth. (_Total aerosol optical depth in visible band_.)

We see that aerosol tend to spread to the winter hemisphere, but that after a couple of
years it is mostly gone.

Why do we care? Volcanoes in different hemispheres warm differently, but the temperature
may still revert to equilibrium in similar ways, i.e., they have similar tails.

--

<!-- .slide: data-transition="slide-in fade-out" -->

### Double-volcano events

<!-- .element class="r-fit-text" -->

--

<!-- .slide: data-transition="fade" -->

_How linear is the temperature response?_

--

<!-- .slide: data-transition="fade" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/hack-md-notes/1e3d1dca42484fc10c418dd1ede027301c9a532d/assets/pic/double-overlap/double-overlap-temp-smoothing-simple.png" -->

--

<!-- .slide: data-transition="fade-in slide-out" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/hack-md-notes/1e3d1dca42484fc10c418dd1ede027301c9a532d/assets/pic/double-overlap/double-overlap-superpose.png" -->

Notes:

We see that when we superpose the single-events using the control run mean temperature
as the baseline, we largely are able to explain the shape of the double-event. Could not
have expected any better match, but this is clearly not enough to conclude.

Works well as a test to check if it is worthwhile doing.

Problem: simulations are not long enough to have a periodic signal

---

## Outlook

<!-- .element class="r-fit-text" -->

--

<!-- .slide: data-transition="slide-in fade-out" -->

### Long simulations

<!-- .element class="r-fit-text" -->

--

<!-- .slide: class="data-auto-animate" -->
<!-- .slide: data-transition="fade" -->

<div class="r-stack">
  <p
    class="fragment animated move-to"
    data-animated-move-to-top="-200px"
    data-animated-move-to-left="0px"
    data-fragment-index="0"
    data-animated-duration="300"
    data-animated-iterations="1"
    data-animated-fill="forwards"
  >
    Using the
    <a
      style="color: #80ff80"
      target="_blank"
      href="https://www.cesm.ucar.edu/projects/community-projects/LME/"
      >CESM LME</a
    >
    data set
  </p>
  <span>
    <img
      class="fragment fade-in"
      data-fragment-index="0"
      src="https://raw.githubusercontent.com/engeir/hack-md-notes/6c20ab748912530c65e30e648c04b4e45a55b838/assets/pic/deconv-cesm-lme/cesm_lme_deconvolution_ensall_mean_forcing.png"
      width="49%"
    />
    <img
      class="fragment fade-in"
      data-fragment-index="0"
      src="https://raw.githubusercontent.com/engeir/hack-md-notes/6c20ab748912530c65e30e648c04b4e45a55b838/assets/pic/deconv-cesm-lme/cesm_lme_deconvolution_ensall_mean_temperature.png"
      width="49%"
    />
  </span>
</div>
<a
  href="https://doi.org/10.1175/BAMS-D-14-00233.1"
  data-citation-key="@ottobliesner2016"
  >Otto-Bliesner et al. (2016)</a
>

<!-- .element: style="font-size:13pt" -->

Notes:

Use datasets from CESM LME (Last Millennium Ensemble).

But this was run with CESM1, and more importantly with **CAM5** (as opposed to WACCM),
hence with a low-top atmosphere reaching only to about 40 km. They also use 2°
resolution for the atmosphere and land components, which for now is the same as I do,
but possibly 1° will be needed.

--

<!-- .slide: data-transition="fade" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/hack-md-notes/6c20ab748912530c65e30e648c04b4e45a55b838/assets/pic/deconv-cesm-lme/cesm_lme_deconvolution_ensall_mean-respnse.png" -->
<!-- .slide: data-background-size="contain" -->

--

<!-- .slide: data-transition="fade" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/hack-md-notes/4cfe0e39fca9474b5dcdbf9ab59eae968a32ecd4/assets/pic/gcm-temperature-decay/temperature-decay-avg.png" -->
<!-- .slide: data-background-size="contain" -->

Notes:

Even with the single- and double-event simulations we may be able to run the
deconvolution, but still need to reach equilibrium so the time series are periodic.

--

Plan: run CESM2 with **deep ocean** and **high-top atmosphere** over several decades

Notes:

**Problem 1**: Model runs take a long time, thus one per season is not reasonable.
**Problem 2**: Due to strong seasonal variability, at least two is preferable.

<!-- Start adding with revealjs-make-reflist -->
<!-- Generated by revealjs-make-reflist. Do not edit. -->

---

## References

<div class="csl-entry" id="ref-benvenuto2009" role="doc-biblioentry">
Benvenuto, F, R Zanella, L Zanni, and M Bertero. 2009. <span>“Nonnegative Least-Squares Image Deblurring: Improved Gradient Projection Approaches.”</span> <em>Inverse Problems</em> 26 (2): 025004. <a href="https://doi.org/10.1088/0266-5611/26/2/025004">https://doi.org/10.1088/0266-5611/26/2/025004</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-lucy1974" role="doc-biblioentry">
Lucy, L. B. 1974. <span>“<span class="nocase">An iterative technique for the rectification of observed distributions</span>.”</span> <em>The Astronomical Journal</em> 79 (6): 745. <a href="https://doi.org/10.1086/111605">https://doi.org/10.1086/111605</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-ottobliesner2016" role="doc-biblioentry">
Otto-Bliesner, Bette L., Esther C. Brady, John Fasullo, Alexandra Jahn, Laura Landrum, Samantha Stevenson, Nan Rosenbloom, Andrew Mai, and Gary Strand. 2016. <span>“Climate Variability and Change Since 850 <span>CE</span>: An Ensemble Approach with the Community Earth System Model.”</span> <em>Bulletin of the American Meteorological Society</em> 97 (5): 735–54. <a href="https://doi.org/10.1175/BAMS-D-14-00233.1">https://doi.org/10.1175/BAMS-D-14-00233.1</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-richardson1972" role="doc-biblioentry">
Richardson, W. H. 1972. <span>“<span class="nocase">Bayesian-Based Iterative Method of Image Restoration*</span>.”</span> <em>J. Opt. Soc. Am.</em> 62 (1): 55–59. <a href="http://www.osapublishing.org/abstract.cfm?URI=josa-62-1-55">http://www.osapublishing.org/abstract.cfm?URI=josa-62-1-55</a>.
</div>
<!-- .element: style="font-size:20pt" -->
<!-- End adding with revealjs-make-reflist -->
