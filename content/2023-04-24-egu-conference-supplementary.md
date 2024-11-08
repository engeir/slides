---
title: "Supplementary to: Insensitivity of global temperature response to the magnitude of volcanic eruptions"
event: EGU General Assembly 2023
author: Eirik R. Enger
date: "2023-04-24"
lang: en-GB
hidden: true
revealOptions:
  transition: "none"
  showNotes: separate-page
  pdfSeparateFragments: false
---

# Supplementary to: Insensitivity of global temperature response to the magnitude of volcanic eruptions

<!-- .element: style="font-size:50pt" -->

_In EGU session **"Understanding volcano-climate impacts and the stratospheric aerosol
layer"**_

<!-- .element: style="font-size:18pt" -->

<img src="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/UiT_Logo_Eng_2l_Hvit.png" width="auto" height="110px" />
<img src="https://egu23.eu/EGU22-sharing-is-encouraged.png" width="auto" height="110px" />
<a href="https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html" target="_blank">
<img src="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/egu23-3331-qr.png" width="auto" height="110px" /> </a>

---

## Motivation

<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-visibility="hidden" -->

--

<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/aod-all-strengths.webp" -->

--

<!-- .slide: data-background-color="#001928" -->
<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/toa-all-strengths.webp" -->

--

<!-- .slide: data-background-color="#001928" -->

Using a linear operator to describe temperature fluctuations:

<!-- dprint-ignore-start -->

$$
\Delta T(t)=\hat{L}[f_K(t)]
$$

$$
\Delta T(t)=\phi\ast f_K(t)=\phi\ast\sum_k A_k\delta(t-t_k)
$$

<!-- dprint-ignore-end -->

Notes:

The first equation show the linear relation between some forcing 𝑓(𝑡) and the
deterministic temperature fluctuation due to the forcing.

We wish to look further into the linearity assumption in relation to volcanoes over a
large range of eruption magnitudes (total injected SO2).

Can we write up the temperature response to volcanic eruptions as a convolution between
the forcing and some general shape function, here represented by the letter 𝜙?

The forcing is here consisting only of forcing due to episodic volcanoes, where 𝐴
represent the amplitude of a given volcanic event arriving at time 𝑡_𝑘.

--

<!-- .slide: data-background-color="#001928" -->

<!-- dprint-ignore-start -->

`$$
\Delta T(t)=\phi\ast f_K(t)=\phi\ast\sum_k A_k\delta(t-t_k)
$$`

`$$
A_k\left\{
\begin{aligned}
&\overset{?}{=}g(M_k^{\max})\\
&\overset{?}{=}M_k^{\max}
\end{aligned}
\right.,\,
M=\left\{
\begin{aligned}
&\mathrm{SO_2\,[Tg]}\\
&\mathrm{AOD\,[1]}\\
&\mathrm{TOA\,[W/m^2]}
\end{aligned}
\right.
$$`

<!-- dprint-ignore-end -->

where `$M_k^{\max}$` is the peak magnitude of event `$k$`.

<!-- .element: style="font-size:20pt" -->

Notes:

If so, what representation of the forcing should one use? Do we perhaps need a
non-linear transformation (𝑔(⋅)) of the forcing to be able to get temperature from
convolutions?

We consider three different sources to describe the forcing; total injected SO2 in Tg,
the aerosol optical depth and forcing as top-of-the-atmosphere radiative forcing.

(Injected SO2 is used as model input to simulate the volcanoes, while both AOD and
radiative forcing are output variables of the model.)

---

## Results

<!-- .slide: data-visibility="hidden" -->

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/injection_vs_temperature.webp" -->

Notes:

Temperature anomaly against injected SO2.

| Short Name | Long Name                    |
| :--------- | :--------------------------- |
| C2W        | CESM2(WACCM6)                |
| C2WN↑      | CESM2(WACCM6), high latitude |
| C2C↑       | CESM2(CAM6)                  |
| C1C        | CESM1(CAM5)                  |
| P          | Pinatubo                     |
| P100       | Pinatubo times 100           |
| T          | Tambora                      |

> C1C data from
> <a href="https://doi.org/10.1175/BAMS-D-14-00233.1" data-citation-key="@ottobliesner2016">Otto-Bliesner
> et al. (2016)</a>.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/injection_vs_temperature_logscale.webp" -->

Notes:

Temperature anomaly against injected SO2.

| Short Name | Long Name                    |
| :--------- | :--------------------------- |
| C2W        | CESM2(WACCM6)                |
| C2WN↑      | CESM2(WACCM6), high latitude |
| C2C↑       | CESM2(CAM6)                  |
| C1C        | CESM1(CAM5)                  |
| P          | Pinatubo                     |
| P100       | Pinatubo times 100           |
| T          | Tambora                      |

> C1C data from
> <a href="https://doi.org/10.1175/BAMS-D-14-00233.1" data-citation-key="@ottobliesner2016">Otto-Bliesner
> et al. (2016)</a>.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/injection_vs_aod.webp" -->

Notes:

Aerosol optical depth versus injected SO2.

| Short Name | Long Name                    |
| :--------- | :--------------------------- |
| C2W        | CESM2(WACCM6)                |
| C2WN↑      | CESM2(WACCM6), high latitude |
| C2C↑       | CESM2(CAM6)                  |
| P          | Pinatubo                     |
| P100       | Pinatubo times 100           |
| T          | Tambora                      |

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/injection_vs_aod_logscale.webp" -->

Notes:

Aerosol optical depth versus injected SO2.

| Short Name | Long Name                    |
| :--------- | :--------------------------- |
| C2W        | CESM2(WACCM6)                |
| C2WN↑      | CESM2(WACCM6), high latitude |
| C2C↑       | CESM2(CAM6)                  |
| P          | Pinatubo                     |
| P100       | Pinatubo times 100           |
| T          | Tambora                      |

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/aod_vs_temperature.webp" -->

Notes:

Temperature versus aerosol optical depth.

| Short Name | Long Name                    |
| :--------- | :--------------------------- |
| C2W        | CESM2(WACCM6)                |
| C2WN↑      | CESM2(WACCM6), high latitude |
| P          | Pinatubo                     |
| P100       | Pinatubo times 100           |
| T          | Tambora                      |

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/aod_vs_temperature_logscale.webp" -->

Notes:

Temperature versus aerosol optical depth.

| Short Name | Long Name                    |
| :--------- | :--------------------------- |
| C2W        | CESM2(WACCM6)                |
| C2WN↑      | CESM2(WACCM6), high latitude |
| P          | Pinatubo                     |
| P100       | Pinatubo times 100           |
| T          | Tambora                      |

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/injection_vs_toa.webp" -->

Notes:

Radiative forcing versus injected SO2.

| Short Name | Long Name          |
| :--------- | :----------------- |
| C2W        | CESM2(WACCM6)      |
| C1C        | CESM1(CAM5)        |
| P          | Pinatubo           |
| P100       | Pinatubo times 100 |

> C1C data from
> <a href="https://doi.org/10.1175/BAMS-D-14-00233.1" data-citation-key="@ottobliesner2016">Otto-Bliesner
> et al. (2016)</a>.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/toa_vs_temperature.webp" -->

Notes:

Temperature versus radiative forcing.

| Short Name | Long Name          |
| :--------- | :----------------- |
| C2W        | CESM2(WACCM6)      |
| C1C        | CESM1(CAM5)        |
| P          | Pinatubo           |
| P100       | Pinatubo times 100 |

> C1C data from
> <a href="https://doi.org/10.1175/BAMS-D-14-00233.1" data-citation-key="@ottobliesner2016">Otto-Bliesner
> et al. (2016)</a>.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide:
data-background="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/aod_vs_toa_avg_scaled.webp"
-->

Notes:

Scaled version of the two smaller eruption data points, such that the peak values
coincide.

| Short Name  | Long Name                      |
| :---------- | :----------------------------- |
| C2W Peaks\* | CESM2(WACCM6), Peak values     |
| C2W↓        | CESM2(WACCM6), weak eruption   |
| C2W—        | CESM2(WACCM6), medium eruption |
| C2W↑        | CESM2(WACCM6), strong eruption |

---

<!-- .slide: data-background-color="#001928" -->

### Links

<!-- dprint-ignore-start -->

----

<!-- dprint-ignore-end -->

Go to
[html version](https://slides.eirik.re/2023-04-24-egu-conference-supplementary?showNotes=separate-page).

[Link](https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html) and QR code to the
conference abstract information:

<a href="https://meetingorganizer.copernicus.org/EGU23/EGU23-3331.html" target="_blank">
<img src="https://raw.githubusercontent.com/engeir/presentations/dd0a662/2023/egu23/assets/egu23-3331-qr.png" width="auto" height="110px" /> </a>

<!-- dprint-ignore-start -->

----

<!-- dprint-ignore-end -->
