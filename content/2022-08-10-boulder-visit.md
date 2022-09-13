---
title: Using CESM2 and WACCM for synthetic volcanic eruption simulations
event: Boulder Visit
date: "2022-08-10"
revealOptions:
  allottedTime: 900000
---

## Using CESM2 and WACCM for synthetic volcanic eruption simulations

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

The FPP and the deconvolution

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
