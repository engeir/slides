---
title: Running CESM2 with synthetic volcanic forcing
event: UiT Climate Meeting
date: "2022-02-09"
---

# Running CESM2 with synthetic volcanic forcing

--

<!-- .slide: data-background="#891919" -->

## Plan

- Run CESM2 (community Earth system model) with volcanic forcing <!-- .element: class="fragment" data-fragment-index="1" -->
- Volcanoes are the only external forcing <!-- .element: class="fragment" data-fragment-index="2" -->
- Obtain estimate of the temperature response <!-- .element: class="fragment" data-fragment-index="3" -->

---

# Example

--

<!-- .slide: data-background="https://github.com/engeir/presentations-files/raw/9a4f6b9150206f27120130b18d8ac09f68469465/2021/fysikermotet/noresm/noresm_raw_dark.png" -->
<!-- .slide: data-background-size="95vw" -->

--

<!-- .slide: data-background="https://github.com/engeir/presentations-files/raw/9a4f6b9150206f27120130b18d8ac09f68469465/2021/fysikermotet/noresm/response_func_noresm1_choose_dark.png" -->
<!-- .slide: data-background-size="95vw" -->

--
<!-- .slide: data-background="https://github.com/engeir/presentations-files/raw/9a4f6b9150206f27120130b18d8ac09f68469465/2021/fysikermotet/noresm/noresm_raw_with_est_dark.png" -->
<!-- .slide: data-background-size="95vw" -->

--

<!-- .slide: data-background-color="#002f4b" -->
<!-- .slide: data-background-video-loop="true" -->
<!-- .slide: data-background-video="https://github.com/engeir/presentations-files/raw/9a4f6b9150206f27120130b18d8ac09f68469465/2021/fysikermotet/animation.mp4" -->
<!-- .slide: data-background-size="contain" -->

---

# Current affairs

--

Creating synthetic volcanic forcing data

--

<!-- .slide: data-transition="slide-in fade-out" -->
<!-- .slide: data-background="https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/synthetic_volcanoes_historic.png" -->
<!-- .slide: data-background-size="95vw" -->
<!-- .slide: data-background-transition="slide-in fade-out" -->
<!-- .slide: data-background-color="#000" -->

### Post industrial volcanoes
<!-- .element: style="margin-top: -20vh;" -->

--

<!-- .slide: data-transition="fade" -->
<!-- .slide: data-background="https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/synthetic_volcanoes_FPP.png" -->
<!-- .slide: data-background-size="95vw" -->
<!-- .slide: data-background-color="#000" -->

### FPP generated volcanoes
<!-- .element: style="margin-top: -20vh;" -->

--

<!-- .slide: data-transition="fade-in slide-out" -->
<!-- .slide: data-background="https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/synthetic_volcanoes_single.png" -->
<!-- .slide: data-background-size="95vw" -->
<!-- .slide: data-background-color="#000" -->

### Large single volcano
<!-- .element: style="margin-top: -20vh;" -->

--
<!-- .slide: data-transition="slide-in fade-out" -->

| ![Aerosol forcing](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/AEROD_v_simple_vanilla.png) | ![Temperature](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/TREFHT_simple_vanilla.png) |
| -: | :- |

Historical run, unchanged

Note:
How do I do this? Two images side-by-side should not be hard!?

--

<!-- .slide: data-transition="fade" -->

| ![Aerosol forcing](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/AEROD_v20220221_simple-ens1.png) | ![Temperature](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/TREFHT20220221_simple-ens1.png) |
| -: | :- |

Historical run, eruption in 1850-02-15

--

<!-- .slide: data-transition="fade" -->

| ![Aerosol forcing](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/AEROD_v20220221_simple-ens2.png) | ![Temperature](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/TREFHT20220221_simple-ens2.png) |
| -: | :- |

Historical run, eruption in 1850-05-15

--

<!-- .slide: data-transition="fade" -->

| ![Aerosol forcing](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/AEROD_v20220221_simple-ens3.png) | ![Temperature](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/TREFHT20220221_simple-ens3.png) |
| -: | :- |

Historical run, eruption in 1850-08-15

--

<!-- .slide: data-transition="fade" -->

| ![Aerosol forcing](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/AEROD_v20220221_simple-ens4.png) | ![Temperature](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/TREFHT20220221_simple-ens4.png) |
| -: | :- |

Historical run, eruption in 1850-11-15

--

<!-- .slide: data-transition="fade" -->

| ![Aerosol forcing](https://github.com/engeir/presentations/raw/main/2022/uit-climate-meeting/assets/AEROD_v20220218_simple-ens5.png) | ![Temperature](https://github.com/engeir/presentations/raw/a97344826c48c9210641d7eeae867d3cab1db520/2022/uit-climate-meeting/assets/TREFHT20220218_simple-ens5.png) |
| -: | :- |

Historical run, eruption in 1851-02-15

Note:
[Reset](#/2/5)
<!-- .element: style="position:relative;font-size:12pt;text-align:left" -->

---

# Experiments

--

<!-- .slide: data-transition="fade" -->

1. Small ensemble over 5 to 10 years &#8594; Look at internal variability
2. Longer run with volcanoes generated from a Poisson process <!-- .element: class="fragment" data-fragment-index="1" -->
3. Volcanoes that cluster together <!-- .element: class="fragment" data-fragment-index="2" -->

---

# Questions

--

What is an appropriate frequency of volcanoes?

--

Is the response the same as that you get from, say CO<sub>2</sub>?

What about solar?

--

<!-- .slide: data-transition="slide-in fade-out" -->

Is the response dependent on altitude?

Magnitude/total emitted aerosols?

Or maybe what hemisphere the aerosols are mainly in?

--

<!-- .slide: data-transition="fade" -->

- What is an appropriate frequency of volcanoes?
- Is the response the same as that you get from, say CO<sub>2</sub>? What about solar?
- Is the response dependent on altitude? Magnitude/total emitted aerosols? Or maybe what
  hemisphere the aerosols are mainly in?
