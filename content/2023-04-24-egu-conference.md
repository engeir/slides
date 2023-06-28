---
title: Insensitivity of global temperature response to the magnitude of volcanic eruptions
event: EGU General Assembly 2023
author: Eirik R. Enger
date: "2023-04-24"
lang: en-GB
revealOptions:
  transition: "none"
  allottedTime: 480_000
  pdfSeparateFragments: false
---

<!--
Color is from https://uit.no/ressurs/uit/profil2019/examples/fargekart.png, but at a
darker luminosity.
-->

# Insensitivity of global temperature response to the magnitude of volcanic eruptions

<!-- .element: style="font-size:50pt" -->

_In EGU session **"Understanding volcano-climate impacts and the stratospheric aerosol
layer"**_

<!-- .element: style="font-size:18pt" -->

<img
src="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/UiT_Logo_Eng_2l_Hvit.png"
width="auto" height="110px" />
<img src="https://egu23.eu/EGU22-sharing-is-encouraged.png" width="auto" height="110px" />
<a href="https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html" target="_blank">
<img
src="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/egu23-3331-qr.png"
width="auto" height="110px" />
</a>

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

_Figure from
<a href="https://doi.org/10.1007/s00382-016-3055-1" data-citation-key="@gregory2016">Gregory
et al. (2016)</a>_

<!-- .element: style="font-size:13pt" -->

![Gregory AOD vs forcing](https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/gregory-aod-toa-swap-trans.png)

<!-- .element: class="r-stretch" -->

Notes:

This plot is from Gregory et al. (2016), and it's showing radiative forcing against
aerosol optical depth. Two simulations were done by the authors using the HadCM3 climate
model, one simulation by [Andrews (2014)](http://dx.doi.org/10.1175/JCLI-D-13-00336.1)
used the HadGEM2 climate model while the AR5 data points are from the Fifth Assessment
report of the IPCC (intergovernmental panel on climate change).

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

> Plot from [Gregory et al. (2016)](https://doi.org/10.1007/s00382-016-3055-1),
> figure 4.

--

<!-- .slide: data-background-color="#001928" -->

### Simulations

- CESM2 (Community Earth System Model, version 2.1.3)
  <!-- .element: class="fragment" -->
- WACCM6 atmosphere <!-- .element: class="fragment" -->
- Dynamic ocean and prescribed sea-surface temperature conditions (AOGCM & AGCM)
  <!-- .element: class="fragment" -->

Notes:

Simulations are carried out with the Community Earth System Model, version 2.1.3, and
using the WACCM6 high-top atmosphere component, specifically in a nominal two degree
resolution and the "middle atmosphere" component setting. Both simulations with a
dynamic ocean (i.e., running the model as an AOGCM) and prescribed sea-surface
temperature conditions (i.e., a AGCM) have been done.

--

<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide:
data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/temperature-all-strengths.webp"
-->

Notes:

We here see the three main simulations that have been run, of individual volcanic
eruptions at the equator with three different magnitudes defined by inputting different
amounts of SO2 into the atmosphere.

We are specifically looking at the temperature response from the three different
eruption magnitudes, where the notation of a downward arrow, horizontal line and upward
arrow will be used to indicate the different magnitudes of a weak, medium and strong
eruption, respectively.

> For similar plots of aerosol optical depth and radiative forcing, see the
> [supplementary](https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html).

--

<!-- .slide: data-state="blur" -->
<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide:
data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/temperature-all-strengths.webp"
-->
<!-- .slide: data-background-opacity="0.15" -->

- At the equator
- <!-- .element: class="fragment" -size:29pt" --> $\mathrm{SO_2}$ injected at $18$–$20$
  `$\mathrm{km}$` altitude
- <!-- .element: class="fragment" -size:29pt" --> $\mathrm{SO_2}$ amounts:
  - `$26\,\mathrm{Tg}$`(↓)
  - `$400\,\mathrm{Tg}$`(—)
  - `$1629\,\mathrm{Tg}$`(↑)

Notes:

The volcanoes were created from an equatorial eruption, with the SO2 injected between 18
and 20 km altitude. The amounts of injected SO2 were 26 Tg (similar to Mt. Pinatubo),
400 Tg and 1629 Tg (same order of magnitude as Young Toba Tuff ~74 ky ago) of SO2 into
the atmosphere between 18 and 20 km height.

> Tg = tera gram = Mt = mega tons = 1e12 grams

--

<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide:
data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/double-overlap-superpose.webp"
-->

Notes:

Let us say we take the medium-sized volcano and let it erupt twice with four years
apart. This is what we see here in blue, with two copies of the medium-sized volcano
shown in orange, aligned so that the eruptions occur at the same time (the shadings mark
the two regions of the single events). Superposing the two orange individual eruption
time series gives the green time series.

The volcano erupted first on 15. February 1853 and then on the same day in 1857.

From this initial simulation of overlapping pulses, the superposing of temperature
response is relatively good, motivating further analysis of the linearity (or lack
thereof) of the temperature response. From this alone one might expect that temperature
does indeed respond linearly to _some representation_ of the radiative forcing.

---

## Results

<!-- .slide: data-visibility="hidden" -->

--

_Legend description for the forthcoming figures._

<!-- .element: style="font-size:20pt" -->
<!-- .slide: data-visibility="hidden" -->

| Short Name | Long Name                             |
| :--------- | :------------------------------------ |
| C2W        | CESM2(WACCM6)                         |
| C2WN↑      | CESM2(WACCM6), high latitude, north   |
| C2WDO—     | CESM2(WACCM6), double and overlapping |
| P          | Pinatubo                              |
| P100       | Pinatubo times 100                    |
| T          | Tambora                               |

<!-- .element: class_="fragment animated move-to scale-down"
data-animated-move-to-left="-15vw" data-animated-move-to-top="10vh" -->
<!-- .element: style="font-size:15pt" -->

Notes:

We have run the CESM2 as an AOGCM and AGCM with prescribed SST conditions with made up
volcanic eruptions of three different sizes:

- the smallest volcano is comparable to the Mt. Pinatubo eruption
- the largest volcano is comparable to the Young Toba Tuff eruption (i.e., roughly 100
  times Mt. Pinatubo)
- the third sits in the middle between the two extremes.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide:
data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/aod_vs_temperature_logscale.webp"
-->

Notes:

Aerosol optical depth versus temperature on semilog-x axis.

This plot is showing the peak values of the three individual CESM2(WACCM6) runs, as well
as data from the Mount Pinatubo eruption, Pinatubo times 100 simulation and Mount
Tambora eruption.

The C2W temperature data show close to logarithmic dependence on AOD, while data from
other sources than CESM2 fall slightly off this, with especially the Pinatubo times 100
simulation having a large temperature response.

| Short Name | Long Name          |
| :--------- | :----------------- |
| C2W        | CESM2(WACCM6)      |
| P          | Pinatubo           |
| P100       | Pinatubo times 100 |
| T          | Tambora            |

> **Pinatubo** AOD data from
> <a href="https://doi.org/10.5194/gmd-11-2633-2018" data-citation-key="@sukhodolov2018">Sukhodolov
> et al. (2018)</a>, temperature from
> <a href="https://doi.org/10.1029/1999JD900835" data-citation-key="@hansen1999">Hansen
> et al. (1999)</a>. **Pinatubo times 100** AOD and temperature data from
> <a href="https://doi.org/10.1007/s00382-005-0066-8" data-citation-key="@jones2005">Jones
> et al. (2005)</a>. **Tambora** AOD data from
> <a href="https://doi.org/10.5194/essd-9-809-2017" data-citation-key="@toohey2017">Toohey,
> M. and Sigl, M. (2017)</a>, temperature from
> <a href="https://doi.org/10.1002/wcc.407" data-citation-key="@raible2016">Raible et
> al. (2016)</a>.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide:
data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/aod_vs_temperature.webp"
-->

Notes:

Plotting this on linear axis makes it more clear that the biggest outlier is the
Pinatubo times 100 simulation, while the Pinatubo and Tambora data lie close to the
weakest CESM2 simulation.

A similar plot can be made with temperature anomaly against injected SO2 (input field to
the CESM2 simulations), but this is not shown here since it is close to a simple scaling
of the x-axis.

> The "temperature-versus-SO2"-plot and similar plots can be viewed in the
> [supplementary](https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html).

| Short Name | Long Name          |
| :--------- | :----------------- |
| C2W        | CESM2(WACCM6)      |
| P          | Pinatubo           |
| P100       | Pinatubo times 100 |
| T          | Tambora            |

> **Pinatubo** AOD data from
> <a href="https://doi.org/10.5194/gmd-11-2633-2018" data-citation-key="@sukhodolov2018">Sukhodolov
> et al. (2018)</a>, temperature from
> <a href="https://doi.org/10.1029/1999JD900835" data-citation-key="@hansen1999">Hansen
> et al. (1999)</a>. **Pinatubo times 100** AOD and temperature data from
> <a href="https://doi.org/10.1007/s00382-005-0066-8" data-citation-key="@jones2005">Jones
> et al. (2005)</a>. **Tambora** AOD data from
> <a href="https://doi.org/10.5194/essd-9-809-2017" data-citation-key="@toohey2017">Toohey,
> M. and Sigl, M. (2017)</a>, temperature from
> <a href="https://doi.org/10.1002/wcc.407" data-citation-key="@raible2016">Raible et
> al. (2016)</a>.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide:
data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/aod_vs_toa_avg_inset.webp"
-->

Notes:

Similar plot to the one shown from Gregory et al. (2016), of annual mean radiative
forcing against aerosol optical depth. This uses the same ratio on the axes, but
somewhat zoomed out.

All C2W-labels are simulations with the CESM2 climate model and WACCM6 in the middle
atmosphere configuration. Blue, downward pointing triangles indicate annual means from
the simulation with the weakest eruption (similar to Mt. Pinatubo); orange diamonds
indicate the medium-sized eruption simulation and green upward pointing triangles
indicate means from the strongest eruption simulation.

For comparison, the HadCM3 data points from the figure by Gregory et al. (2016) is also
shown in grey "x"-es, as well as annual means from the double and overlapping simulation
(red diamonds) and the peak values from both Pinatubo and Tambora.

There is still substantial noise in the C2W data, but ~~no years across the whole
ensemble~~ _only the weak eruption data points (as well as two individual data points
from the intermediate and strong)_ fall below the "-19" gradient line for AOD values of
only 0.02 and higher.

| Short Name            | Long Name                                                |
| :-------------------- | :------------------------------------------------------- |
| T Peak\*              | Tambora, peak value                                      |
| C2W↓                  | CESM2(WACCM6), weak eruption                             |
| C2W—                  | CESM2(WACCM6), medium eruption                           |
| C2W↑                  | CESM2(WACCM6), strong eruption                           |
| P Peak\*              | Pinatubo, peak value                                     |
| C2WDO—                | CESM2(WACCM6), double and overlapping, medium eruption   |
| Gregory et al. (2016) | Values from HadCM3 sstPiHistvol by Gregory et al. (2016) |

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide:
data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/aod_vs_toa_avg_full.webp"
-->

Notes:

If we zoom out to include all data points, it is evident that the two largest eruption
simulations follow a way less steep gradient than the HadCM3 data does.

The two largest (green and orange) ~~line up quite well, but on different slopes; the
medium with a steeper gradient than the strong, but where the strong have some points
among the medium eruption (along the -4 gradient line) stemming from the initial rise of
the eruption. The decaying part last longer, thus more points come from the decay, and
they line up close to on a gradient of -1.~~ _start off similarly, but on a loop
trajectory, where the intermediate data points loop cuts off short and thus get on
average a steeper graient than the strong eruption points._

The points from double and overlapping simulation, shown by the red thin diamonds,
places themselves among the points coming from the medium-sized individual simulation,
as expected.

The peak values from the three main equatorial simulations are shown as the red circles.
The peak value from the Pinatubo times 100 simulation (from Jones et al. (2005)) is
shown with a pink square. This simulation incidently falls on the same gradient line as
the medium-sized eruption. While the magnitude of the radiative forcing obtained from
this simulation of a super-eruption seems to be too small when compared to the "-19"
gradient line, compared to the simulations done here with CESM2, its radiative forcing
magnitude seems too big.

Filling out this radiative forcing-AOD space may give a clearer answer to whether there
is a linear relation to be found, and possibly its range of validity. And even if there
is no linear relationship, the loop that is drawn out by the strongest eruption may hint
to there being different dynamical processes at play during the initial rise and the
slow decay to equilibrium when comparing radiative forcing and aerosol optical depth.

| Short Name            | Long Name                                                |
| :-------------------- | :------------------------------------------------------- |
| C2W Peaks\*           | CESM2(WACCM6), peak values                               |
| T Peak\*              | Tambora, peak value                                      |
| C2W↓                  | CESM2(WACCM6), weak eruption                             |
| C2W—                  | CESM2(WACCM6), medium eruption                           |
| C2W↑                  | CESM2(WACCM6), strong eruption                           |
| P100 Peak\*           | Pinatubo times 100, peak value                           |
| P Peak\*              | Pinatubo, peak value                                     |
| C2WDO—                | CESM2(WACCM6), double and overlapping, medium eruption   |
| Gregory et al. (2016) | Values from HadCM3 sstPiHistvol by Gregory et al. (2016) |

> **Pinatubo times 100** AOD and temperature data from
> <a href="https://doi.org/10.1007/s00382-005-0066-8" data-citation-key="@jones2005">Jones
> et al. (2005)</a>.

---

<!-- .slide: data-background-color="#001928" -->

## Links

<!-- dprint-ignore-start -->

----

<!-- dprint-ignore-end -->

The slides can be viewed both with
([HTML](https://slides.eirikenger.xyz/2023-04-24-egu-conference?showNotes=separate-page),
[PDF](https://raw.githubusercontent.com/engeir/presentations-files/main/2023/egu23/2023-04-24-egu-conference-showNotes-separate-page.pdf))
and without
([HTML](https://slides.eirikenger.xyz/2023-04-24-egu-conference?showNotes=false),
[PDF](https://raw.githubusercontent.com/engeir/presentations-files/main/2023/egu23/2023-04-24-egu-conference-showNotes-false.pdf))
speaker notes.

[Link](https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html) and QR code to the
conference abstract information:

<a href="https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html" target="_blank">
<img src="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/egu23-3331-qr.png" width="auto" height="110px" /> </a>

<!-- dprint-ignore-start -->

----

<!-- dprint-ignore-end -->
<!-- dprint-ignore-start -->

<!-- Start adding with revealjs-make-reflist -->
<!-- Generated by revealjs-make-reflist. Do not edit. -->

---

## References

- <!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-gregory2016" role="doc-biblioentry">
Gregory, J. M., T. Andrews, P. Good, T. Mauritsen, and P. M. Forster. 2016. <span>“Small Global-Mean Cooling Due to Volcanic Radiative Forcing.”</span> <em>Climate Dynamics</em> 47 (December): 3979–91. <a href="https://doi.org/10.1007/s00382-016-3055-1">https://doi.org/10.1007/s00382-016-3055-1</a>.
</div>
- <!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-hansen1999" role="doc-biblioentry">
Hansen, James, Reto Ruedy, J. Glascoe, and Makiko Sato. 1999. <span>“<span>GISS</span> Analysis of Surface Temperature Change.”</span> <em>Journal of Geophysical Research: Atmospheres</em> 104 (D24): 30997–1022. <a href="https://doi.org/10.1029/1999JD900835">https://doi.org/10.1029/1999JD900835</a>.
</div>
- <!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-jones2005" role="doc-biblioentry">
Jones, Gareth S., Jonathan M. Gregory, Peter A. Stott, Simon F. B. Tett, and Robert B. Thorpe. 2005. <span>“<span class="nocase">An <span>AOGCM</span> simulation of the climate response to a volcanic super-eruption</span>.”</span> <em>Climate Dynamics</em> 25 (7): 725–38. <a href="https://doi.org/10.1007/s00382-005-0066-8">https://doi.org/10.1007/s00382-005-0066-8</a>.
</div>
- <!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-raible2016" role="doc-biblioentry">
Raible, Christoph C., Stefan Brönnimann, Renate Auchmann, Philip Brohan, Thomas L. Frölicher, Hans-F. Graf, Phil Jones, et al. 2016. <span>“Tambora 1815 as a Test Case for High Impact Volcanic Eruptions: Earth System Effects.”</span> <em>WIREs Climate Change</em> 7 (4): 569–89. <a href="https://doi.org/10.1002/wcc.407">https://doi.org/10.1002/wcc.407</a>.
</div>

--

- <!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-sukhodolov2018" role="doc-biblioentry">
Sukhodolov, T., J.-X. Sheng, A. Feinberg, B.-P. Luo, T. Peter, L. Revell, A. Stenke, D. K. Weisenstein, and E. Rozanov. 2018. <span>“Stratospheric Aerosol Evolution After Pinatubo Simulated with a Coupled Size-Resolved Aerosol–Chemistry–Climate Model, <span>SOCOL</span>-<span> AER</span>v1.0.”</span> <em>Geoscientific Model Development</em> 11 (7): 2633–47. <a href="https://doi.org/10.5194/gmd-11-2633-2018">https://doi.org/10.5194/gmd-11-2633-2018</a>.
</div>
- <!-- .element: style="font-size:20pt" -->
<div class="csl-entry" id="ref-toohey2017" role="doc-biblioentry">
Toohey, M., and M. Sigl. 2017. <span>“Volcanic Stratospheric Sulfur Injections and Aerosol Optical Depth from 500 <span>BCE</span> to 1900 <span>CE</span>.”</span> <em>Earth System Science Data</em> 9 (2): 809–31. <a href="https://doi.org/10.5194/essd-9-809-2017">https://doi.org/10.5194/essd-9-809-2017</a>.
</div>
<!-- End adding with revealjs-make-reflist -->
