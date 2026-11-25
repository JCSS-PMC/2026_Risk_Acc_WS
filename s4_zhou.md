# Probabilistic Tornado Wind Hazard Maps for Canada

**Wenxing Zhou, Department of Civil and Environmental Engineering, Western University, London, ON, Canada**

Session 4 · Thursday 22 October 2026, 12.11–12.38 (presentation and discussion)

[Presentation slides (PDF)](slides/Zhou_Probabilistic_Tornado_Wind_Hazard_Maps_Canada.pdf)

Based on: Y. Liu et al. (2026), Journal of Wind Engineering & Industrial Aerodynamics 278, 106619. Collaborators: Yongxu Liu, Hanping Hong, Dave Sills and Greg Kopp (PI); the work was largely carried out by the postdoctoral fellow Yongxu Liu.

## Summary

The presentation dealt with hazard quantification – not with risk or risk acceptance criteria – as the basis for proposed tornado design provisions in the 2030 edition of the National Building Code of Canada.

**Background.** Canada ranks second in the world, albeit a distant second, in the annual number of reported tornadoes (about 70 per year against about 1 200 in the US). Tornado damage to buildings can be catastrophic – an EF4 tornado north of Calgary in 2023, two F2 tornadoes in Vaughan near Toronto in 2009, an F3 tornado in Goderich on Lake Huron in 2011 – yet the current NBCC 2025 has no tornado design provisions (the US introduced them only in 2022). The study builds on thirty to forty years of tornado research at Applied Research Associates (ARA) and at Western, and on the Northern Tornadoes Project (NTP) at Western, which detects, surveys and rates tornadoes in Canada.

**Framework.** Tornado catalogue → correction for unreported tornadoes → occurrence rate → intensity and path geometry → striking rate for a given structure → tornado wind-field model → wind speed distribution given a strike → hazard map of wind speed for a given return period.

**Steps.** The NTP database holds 3 066 reported tornadoes from 1980 to 2023; southern Ontario is the hotspot, followed by Alberta, Saskatchewan and Manitoba, with few in British Columbia and the Maritimes. Since not all tornadoes are reported, the probability of reporting is modelled as a function of population density (2021 census), and the actual occurrence is modelled with Poisson, zero-inflated Poisson or negative binomial models with annual thunderstorm days and cloud-to-ground lightning flashes as explanatory variables, estimated by Bayesian updating or maximum likelihood on a grid. The negative binomial model, slightly more conservative, gives smoothed occurrence rates of 4–9·10<sup>−4</sup> per km² per year in southern Ontario. The intensity distribution over the (E)F scale and the path length (tens to hundreds of kilometres) and width (hundreds of metres) distributions – truncated Weibull, conditional on intensity, mostly from US data – feed the strike-rate calculation, which accounts for the variation of the actual intensity along the path (only about 15 % of the path of an F5 tornado is at F5 intensity; Twisdale et al. 1981). Strike rates are computed for point-like structures, areal structures (e.g. 100 000 ft²) and linear structures of different length. The three-dimensional synthetic wind-field model (Twisdale et al.) with tangential, radial and vertical components and probabilistic parameters gives the conditional distribution of the 3-s gust horizontal wind speed at 10 m given a strike of a given actual intensity.

**Maps.** For point-like structures the 10 000-year return period 3-s gust wind speed reaches about 130 km/h in southern Ontario and about 230 km/h for 100 000 years; for a 100 000 ft² areal structure the values rise to about 190 and 270 km/h.

## Discussion

*Summary of the discussion following the presentation (edited from the recording).*

Jochen Köhler, working on comparable snow maps for Norway, asked what probability is assigned to regions without observed tornadoes, since no observation does not mean zero probability; the model for the probability of reporting and the explanatory variables provide the background rate, and where no tornadoes have been observed the assumption makes little difference. Arnold Yuan asked about spatial correlation between grid cells, which had not been tested explicitly.

Raphaël Steenbergen noted that the strike rate for a building is of the order of 10<sup>−5</sup> per year, below the target failure probabilities of most buildings, and asked whether tornadoes therefore need not be considered in building design – which may indeed be why Canada has had no tornado provisions so far; for larger footprints and at community level the picture changes. The Netherlands, with even smaller values, has drawn the same conclusion, but continuous monitoring is required because of the increasing trend. Colin Caprani asked why the maps for F3 and F4 appear lower than those for F2 and F5 (the occurrence rates). A participant asked about the correlation between path length and width (assumed independent, under investigation) and about the meteorological reason for the concentration of the hazard along the US border; the catalogue includes tornadoes crossing from the US, and Jochen Köhler suggested combining the statistics with a meteorological model of the conditions favouring tornado formation, given the short observation period and the low probabilities. The session, and with it the workshop, closed here; see [Conclusions and Outlook](./s5_discussion.md).
