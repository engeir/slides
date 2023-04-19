---
title: Insensitivity of global temperature response to the magnitude of volcanic eruptions
event: EGU General Assembly 2023
author: Eirik R. Enger
date: "2023-03-24"
lang: en-GB
revealOptions:
  transition: "none"
  allottedTime: 480_000
  showNotes: separate-page
  pdfSeparateFragments: false
---

<!--
Color is from https://uit.no/ressurs/uit/profil2019/examples/fargekart.png, but at a
darker luminosity.
-->

# Insensitivity of global temperature response to the magnitude of volcanic eruptions

<!-- .element: style="font-size:50pt" -->

_In EGU session __"Understanding volcano-climate impacts and the stratospheric aerosol
layer"___

<!-- .element: style="font-size:18pt" -->

<img src="./attachments/egu2023/UiT_Logo_Eng_2l_Hvit.png" width="auto" height="110px" />
<img src="https://egu23.eu/EGU22-sharing-is-encouraged.png" width="auto" height="110px" />
<a href="https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html" target="_blank">
<img src="./attachments/egu2023/egu23-3331-qr.png" width="auto" height="110px" /> </a>

Notes:

My name is Eirik Enger, and I'm a PhD candidate at UiT the Arctic University of Norway.
My work focus on how volcanoes affect climate, and today we will look at "Insensitivity
of global temperature response to the magnitude of volcanic eruptions".

---

## Motivation

<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-visibility="hidden" -->

--

<!-- .slide: data-background-color="#001928" -->

_Figure from [Gregory et al. (2016)](https://doi.org/10.1007/s00382-016-3055-1)_

<!-- .element: style="font-size:13pt" -->

![Gregory AOD vs forcing](./attachments/egu2023/gregory-aod-toa-swap-trans.png)

<!-- .element: class="r-stretch" -->

Notes:

This plot is from Gregory et al. (2016), and it's showing radiative forcing against
aerosol optical depth. Two simulations were done by the authors using the HadCM3 climate
model, one simulation by [Andrews (2014)](http://dx.doi.org/10.1175/JCLI-D-13-00336.1)
used the HadGEM2 climate model while the AR5 data points are from a time series from the
Fifth Assessment report of the IPCC (intergovernmental panel on climate change).

This show a proportionality between annual mean values of AOD and radiative forcing, but
only for AOD values up to 0.15, roughly equivalent to the peak of the 1991 Mt. Pinatubo
eruption. Whether this property holds as one goes to much greater values, for example
comparable to the Young Toba Tuff eruption 74ky ago, is of interest to us. Such a super
volcano would have roughly one hundred times the AOD values as Mt. Pinatubo, but
previous simulations indicate radiative forcing values that are only about twenty times
that of Mt. Pinatubo. Is this because the linearity does not hold for this large values,
or is it a shortcoming on the model's side?

Can we make a similar comparison of the peak values, for example in daily resolution (as
opposed to averaging over the whole year before comparing)?

> Plot from [Gregory et al. (2016)](https://doi.org/10.1007/s00382-016-3055-1), figure
> 4.

--

<!-- .slide: data-state="blur" -->
<!-- .slide: data-background-color="#001928" -->

### Simulations

- CESM2 (Community Earth System Model, version 2.1.3) <!-- .element: class="fragment"
  -->
- WACCM6 atmosphere <!-- .element: class="fragment" -->
- <!-- .element: class="fragment" --> Dynamic ocean and constant sea-surface conditions
  (AOGCM & AGCM)

Notes:

Simulations are carried out with the Community Earth System Model, version 2.1.3, and
using the WACCM6 high-top atmosphere component, specifically in a nominal two degree
resolution and the "middle atmosphere" component setting. Both simulations with a
dynamic ocean (i.e., running the model as an AOGCM) and constant sea-surface conditions
(i.e., a AGCM) have been done.

--

<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/egu2023/ens-plts/temperature-all-strengths.webp" -->

Notes:

We here see the three main simulations that have been run, of individual volcanic
eruptions at the equator with three different magnitudes defined by inputting different
amounts of SO2 into the atmosphere.

We are specifically looking at the temperature response from the three different
eruption magnitudes, where the notation of a downward arrow, horizontal line and upward
arrow will be used to indicate the different magnitudes of a weak, medium and strong
eruption, respectively.

> For similar plots of aerosol optical depth and radiative forcing, see the
> supplementary.

--

<!-- .slide: data-state="blur" -->
<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/egu2023/ens-plts/temperature-all-strengths.webp" -->
<!-- .slide: data-background-opacity="0.15" -->

- <!-- .element: style="font-size=25pt" --> At the equator, at $18$–$20$
  `$\mathrm{km}$` altitude
- <!-- .element: class="fragment" style="font-size:25pt" --> $\mathrm{SO_2}$ amounts:
  `$26\,\mathrm{Tg}$`(↓), `$400\,\mathrm{Tg}$`(—) and `$1629\,\mathrm{Tg}$`(↑)

Notes:

The volcanoes were created from an equatorial eruption, with the SO2 injected between 18
and 20 km altitude. The amounts of injected SO2 were 26 Tg (similar to Mt. Pinatubo),
400 Tg and 1629 Tg (same order of magnitude as young Toba Tuff ~74 ky ago) of SO2 into
the atmosphere between 18 and 20 km height.

> Tg = tera gram = Mt = mega tons = 1e12 grams

--

<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/egu2023/double-overlap-superpose.webp" -->

Notes:

Results from running with a 400 Tg volcanic event occurring once (Single event, orange)
and occurring twice four years apart (Double event, blue). "Superposed" in green is two
copies of the single event superposed. The single event is copied and shifted in time,
where the shadings mark the two regions of the single events.

The volcano erupted on 15. February 1853 and on the same day in 1857.

From this initial simulation of overlapping pulses, the superposing of temperature
response is relatively good, motivating further analysis of the linearity (or lack
thereof) of the temperature response.

---

## Results

<!-- .slide: data-visibility="hidden" -->

--

_Legend description for the forthcoming figures._

<!-- .element: style="font-size:20pt" -->

| Short Name | Long Name                             |
| :--------- | :------------------------------------ |
| C2W        | CESM2(WACCM6)                         |
| C2WN↑      | CESM2(WACCM6), high latitude, north   |
| C2WDO—     | CESM2(WACCM6), double and overlapping |
| P          | Pinatubo                              |
| P100       | Pinatubo times 100                    |
| T          | Tambora                               |

<!-- .element: class_="fragment animated move-to scale-down" data-animated-move-to-left="-15vw" data-animated-move-to-top="10vh" -->
<!-- .element: style="font-size:15pt" -->

Notes:

We have run the CESM2 as an AOGCM and AGCM with constant SST conditions with made up
volcanic eruptions of three different sizes:

- the smallest volcano is comparable to the Mt. Pinatubo eruption
- the largest volcano is comparable to the Young Toba Tuff eruption (i.e., roughly 100
  times Mt. Pinatubo)
- the third sits in the middle between the two extremes.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/egu2023/ens-plts/aod_vs_temperature_logscale.webp" -->

Notes:

Aerosol optical depth versus temperature on semilog-x axis.

This plot is showing the peak values of the three individual CESM2(WACCM6) runs, the
CESM2(WACCM6) run that is the same as the largest individual, but placed at 56 degree
north, as well as data from the Mount Pinatubo eruption, Pinatubo times 100 simulation
and Mount Tambora Eruption.

The C2W temperature data show close to logarithmic dependence on AOD, while data from
other sources than CESM2 fall slightly off this, with especially the Pinatubo times 100
simulation having a large temperature response.

| Short Name | Long Name                             |
| :--------- | :------------------------------------ |
| C2W        | CESM2(WACCM6)                         |
| C2WN↑      | CESM2(WACCM6), high latitude, north   |
| P          | Pinatubo                              |
| P100       | Pinatubo times 100                    |
| T          | Tambora                               |

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/egu2023/ens-plts/aod_vs_temperature.webp" -->

Notes:

Plotting this on linear axis makes it more clear that the biggest outlier is the
Pinatubo times 100 simulation, while the Pinatubo and Tambora data lie close to the
weakest CESM2 simulation.

A similar plot can be made with temperature anomaly against injected SO2 (input field to
the CESM2 simulations), but this is not shown here since it is close to a simple scaling
of the x-axis.

| Short Name | Long Name                             |
| :--------- | :------------------------------------ |
| C2W        | CESM2(WACCM6)                         |
| C2WN↑      | CESM2(WACCM6), high latitude, north   |
| P          | Pinatubo                              |
| P100       | Pinatubo times 100                    |
| T          | Tambora                               |

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/egu2023/ens-plts/aod_vs_toa_avg_inset.webp" -->

Notes:

Similar plot to the one shown from Gregory et al. (2016), of annual mean radiative
forcing against aerosol optical depth.

All C2W-labels are simulations with the CESM2 climate model and dynamic ocean using
WACCM6 in the middle atmosphere configuration. Blue, downward pointing triangles
indicate annual means from the simulation with the weakest eruption (similar to Mt.
Pinatubo); orange diamond indicate the medium-sized eruption simulation and green upward
pointing arrow indicate means from the strongest eruption simulation. The peak values
from the three simulations are shown as the red circles.

The two largest (green and orange) line up quite well, the medium with a steeper
gradient than the strong, but where the strong have some points among the medium
eruption (along the -4 gradient line) stemming from the initial rise/descent of the
eruption. The decaying part last longer, thus more points come from the decay, and they
line up close to on a gradient of -1.

Also shown is the double and overlapping simulation where two medium-sized eruptions
were used. The points from this simulation, shown by the red thin diamonds, places
themselves among the points coming from the medium-sized individual simulation, as
expected.

The brown triplet shows an individual eruption simulation using the strongest eruption,
but placed at 56 degrees north. The response is not as strong as for the equatorial
eruption, but still the annual means fall in line with the path draw by the green
triangles.

The peak values from the Pinatubo times 100 simulation is shown with a pink square. This
simulation incidently falls on the same gradient line as the medium-sized eruption.

For comparison, the HadCM3 data points from the figure by Gregory et al. (2016) is also
shown in grey "x"-es.

| Short Name            | Long Name                                                |
| :-------------------- | :------------------------------------------------------- |
| C2W↓                  | CESM2(WACCM6), weak eruption                             |
| C2W—                  | CESM2(WACCM6), medium eruption                           |
| C2W↑                  | CESM2(WACCM6), strong eruption                           |
| C2W Peaks\*           | CESM2(WACCM6), peak values                               |
| C2WDO—                | CESM2(WACCM6), double and overlapping, medium eruption   |
| C2WN↑                 | CESM2(WACCM6), high latitude, north, strong eruption     |
| P100 Peak\*           | Pinatubo times 100, peak value                           |
| Gregory et al. (2016) | Values from HadCM3 sstPiHistvol by Gregory et al. (2016) |

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/egu2023/ens-plts/aod_vs_toa_avg_full.webp" -->

---

<!-- .slide: data-background-color="#001928" -->

### Links

<!-- FIXME: for now, I'm using an old slide as an example. Update the links! -->

_FIXME: for now, I'm using an old slide as an example. Update the links!_

<!-- .element: style="color:red" -->

The slides can be viewed both with
([html](https://slides.eirikenger.xyz/2023-01-24-midterm-evaluation-presentation),
[pdf](https://raw.githubusercontent.com/engeir/presentations-files/main/2022/chess-am/poster.pdf))
and without
([html](https://slides.eirikenger.xyz/2023-01-24-midterm-evaluation-presentation?showNotes=true),
[pdf](https://raw.githubusercontent.com/engeir/presentations-files/main/2022/chess-am/poster.pdf))
speaker notes.

[Link](https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html) and QR code to the
conference abstract information:

<a href="https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html" target="_blank">
<img src="./attachments/egu2023/egu23-3331-qr.png" width="auto" height="110px" /> </a>

<!-- Start adding with revealjs-make-reflist -->
<!-- Generated by revealjs-make-reflist. Do not edit. -->

---

## References

- <!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-gregory2016" role="doc-biblioentry">
Gregory, J. M., T. Andrews, P. Good, T. Mauritsen, and P. M. Forster. 2016. <span>“Small Global-Mean Cooling Due to Volcanic Radiative Forcing.”</span> <em>Climate Dynamics</em> 47 (12): 3979–91. <a href="https://doi.org/10.1007/s00382-016-3055-1">https://doi.org/10.1007/s00382-016-3055-1</a>.
</div>
<!-- End adding with revealjs-make-reflist -->
