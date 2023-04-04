---
title: Insensitivity of global temperature response to the magnitude of volcanic eruptions
event: EGU General Assembly 2023
author: Eirik R. Enger
date: "2023-03-24"
lang: en-GB
revealOptions:
  transition: 'none'
  allottedTime: 480_000
---

# Insensitivity of global temperature response to the magnitude of volcanic eruptions

<!-- .element: style="font-size:50pt" -->

Notes:

Hi, and thanks for showing up to my talk here today. My name is Eirik Enger, and I'm a
PhD candidate at UiT the Arctic University of Norway. My work there focus on how
volcanoes affect climate, and today we will look at "Insensitivity of global temperature
response to the magnitude of volcanic eruptions".

---

## Motivation

See to the abstract, pull out some of it to mention here.

Notes:

The reason we are visiting this topic is that there have been several attempts to do
[this], many of which focus on or assume [something about linearity maybe].

--

Previously a linear relation has been used, that is

$T^{\mathrm{det}}(t)=\hat{L}[F(t)]$

Notes:

Previous efforts have often been using a linear relation to describe temperature
fluctuations in response to a forcing. Some studies also assume the forcing from
different agents to be similar, although this have been disputed by several.

The equation is depicting the linear relation between some forcing F and the
deterministic temperature due to the forcing.

Here, we wish to look further into the linearity assumption in relation to volcanoes
over a large range of eruption magnitudes, where with magnitude it is meant the total
sulphur aerosol mass.

--

$$
\begin{aligned}
\Delta T
&=\int_{-\infty}^{t}\phi(t-s)\[f_K(s)\mathrm{d}s+\sigma \mathrm{d}B(s)\]\\\\
&=\int_{-\infty}^{t}\phi(t-s)f_K(s)\mathrm{d}s+\phi(t-s)\sigma \mathrm{d}B(s)
\end{aligned}
$$

Notes:

We wish to ask: is it reasonable to write up the temperature response to volcanic
eruptions as a convolution between the forcing and some general shape function, here
represented by the letter 𝜙.

--

$$
\Delta T=\phi\ast f_K=\phi\ast\sum_k A_k\delta(t-t_k)
$$

$$
A_k\left\\\{
\begin{aligned}
&\overset{?}{=}g(M_k^{\max})\\\\
&\overset{?}{=}M_k^{\max}
\end{aligned}
\right.,\\,
M_k^\max=\left\\\{
\begin{aligned}
&\mathrm{SO_2\\,[Tg]}\\\\
&\mathrm{AOD\\,[1]}\\\\
&\mathrm{TOA\\,[W/m^2]}
\end{aligned}
\right.
$$

where $M_k^{\max}$ is the magnitude of event $k$, given in $\mathrm{Tg}$
$\mathrm{SO_2}$, the $\mathrm{AOD}$ (aerosol optical depth), top-of-the-atmosphere
radiative imbalance in $\mathrm{W/m^2}$, or possibly something else entirely.

Notes:

The forcing is here consisting only of forcing due to episodic volcanoes, and we
consider three different sources to describe the forcing; total injected SO2 in
Tg, the aerosol optical depth and forcing as top-of-the-atmosphere radiative imbalance.
Injected SO2 is the input to the model that it reads from to simulate the volcanoes,
while both AOD and radiative imbalance are output variables of the model.

--

From Gregory et al. (2016):

> It would be useful for investigation of volcanic forcing and feedback in CMIP6 if
> ensemble experiments were conducted with historical volcanic aerosol as the only
> forcing agent in each AOGCM, to diagnose the climate response, and with the
> corresponding AGCMs with prescribed sea surface conditions, to diagnose the radiative
> forcing. This would reveal whether other models also exhibit a cloud adjustment and a
> lower climate sensitivity for volcanic forcing, and offer the opportunity for analysis
> of the processes involved.

<!-- .element: style="font-size:20pt" -->

We expect $M\_\{k,\\,\mathrm\{AOD\}\}^\max\propto
M\_\{k,\\,\mathrm\{TOA\}\}^\max,\\,\mathrm{AOD}\in (0,0.15)$

Notes:

One note to make about the AOD and radiative imbalance is that they are often assumed as
being proportional, with a proportionality constant of 25 estimated in the AR5.

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/gregory-toa-vs-aod-swap.png" -->

Notes:

This proportionality is shown here, but only for AOD values up to 0.15, roughly
equivalent to the peak of the 1991 Mt. Pinatubo eruption AOD levels. Whether this
property holds as one goes to much greater values, for example the Young Toba Tuff
eruption 74ky ago, is of interest to us. Such a super volcano would have roughly one
hundred times the AOD values as Mt. Pinatubo, but previous simulations indicate
radiative forcing values that are only about twenty times Mt. Pinatubo. Is this because
the relation does not hold for this large values or is it a shortcoming on the model's
side?

---

## Results

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/injection_vs_temperature.webp" -->

Notes:

**Figure:** Temperature anomaly against injected SO2 on linear-linear axis (left) and
semilog-x axis (right)

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/injection_vs_temperature_logscale.webp" -->

Notes:

**Figure:** Temperature anomaly against injected SO2 on linear-linear axis (left) and
semilog-x axis (right)

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/injection_vs_aod.webp" -->

Notes:

Injection versus aerosol optical depth

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/injection_vs_aod_logscale.webp" -->

Notes:

Injection versus aerosol optical depth on log-log axis

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/aod_vs_temperature.webp" -->

Notes:

Aerosol optical depth versus temperature

--

<!-- .slide: data-background-size="contain" -->
<!-- .slide: data-background="./attachments/aod_vs_temperature_logscale.webp" -->

Notes:

Aerosol optical depth versus temperature on semilog-x axis
<!-- Start adding with revealjs-make-reflist -->
<!-- Generated by revealjs-make-reflist. Do not edit. -->

---

## References

<!-- End adding with revealjs-make-reflist -->
