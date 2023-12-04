---
title: "The Martian Dichotomy"
excerpt: "<img src='/images/mars_crust.jpg'><br/>_Image credit: MOLA Science Team_"
collection: science
---
<style>
* {
  box-sizing: border-box;
}

.column {
  float: left;
  width: 33.33%;
  padding: 5px;
}

/* Clearfix (clear floats) */
.row::after {
  content: "";
  clear: both;
  display: table;
}
</style>

The main focus (and the motivation for the funding) of my PhD project was to investigate the potential impact origin of the Martian Dichotomy.

The Martian Dichotomy refers to the most ancient and distinctive feature of Mars: a dramatic 4--8 km contrast in elevation between the two hemispheres (e.g. Andrews-Hanna et al., 2008) that correlates closely with a ~25 km crustal thickness disparity (Zuber, 2000; Neumann et al., 2004). The northern hemisphere is the thinner (and lower) of the two, and exhibits this as an apparent basin that covers ~42% of its surface.

<img src='/images/Crust_Altitude.png'>
_Elevation (top) and crustal thickness (bottom) maps of Mars, adapted from Zuber et al. (2000). The red line on the bottom figure shows the Dichotomy boundary, solid where it is known to a high degree of confidence and dashed where it is estimated._

Many authors have proposed that this basin is the result of a giant impact from some large planetary body, leaving behind what would be the largest impact crater in the Solar System (the "Borealis Basin") (e.g. Marinova et al., 2008}. However, giant impacts introduce giant shockwaves, which lead to extreme internal heating. So much heat, in fact, that almost the entire hemisphere may be melted down to the surface of the planet's iron core. More recent studies have therefore supported an alternative hypothesis, whereby the body impacts and subsequently melts the southern hemisphere, which then solidifies and re-crystallises to form a thicker crust than that of the unmodified, primordial northern hemisphere (Golabek et al., 2011, 2018).

In collaboration with my co-authors, I investigated the feasibility of this southern impact scenario for the Martian Dichotomy. Accurately studying such an event requires the combination of two entirely different perspectives: the immediate effects of the giant impact that occur within the first ~24 hours, and the subsequent internal evolution (i.e. the movement of the rocky mantle and production of crust) that transpire over the following 4.5 billion years. I focussed on the former component, simulating the impact using an advanced smoothed-particle hydrodynamics (SPH) code, SPHLATCH. The investigation into long-term internal evolution was led by Dr Kar Wai Cheng of ETH Zurich using the 3D geodynamics code StagYY.

Several publications are in the works for this project. In the first, already [published in Icarus](https://www.sciencedirect.com/science/article/pii/S0019103522004870), the impact models take the lead; I ran over a hundred simulations and developed a simplified geophysical model (in C++ and Python) to estimate the crustal distribution one can expect from a given impact. This allowed me to highlight the most likely impact parameters. The second publication, currently in review in Geophysical Research Letters, instead focusses on the long-term evolution. The final publication, currently in review in Icarus, combines the two approaches to provide the most comprehensive study on the topic to date.

<div class="row">
  <div class="column">
    <img src="/images/head_on.gif" alt="head_on" style="width:100%">
  </div>
  <div class="column">
    <img src="/images/90.gif" alt="90" style="width:100%">
  </div>
  <div class="column">
    <img src="/images/2000km_50core_1p0.gif" alt="2000km" style="width:100%">
  </div>
</div>
_Example simulation results from Ballantyne et al. (2023). The colours indicate composition and parent body, with purple and yellow material being the rocky mantle and iron core of the impacting body, respectively, and blue and red being the mantle and core of Mars._

__References:__
<br>
Andrews-Hanna, J.C., Zuber, M.T., Banerdt, W.B., 2008. The Borealis basin and the origin of the martian crustal dichotomy. Nature 453 (7199), 1212–1215. [http://dx.doi.org/10.1038/nature07011](http://dx.doi.org/10.1038/nature07011)

Golabek, G.J., Emsenhuber, A., Jutzi, M., Asphaug, E.I., Gerya, T.V., 2018. Coupling SPH and thermochemical models of planets: Methodology and example of a Mars- sized body. Icarus 301, 235–246. [http://dx.doi.org/10.1016/j.icarus.2017.10.003](http://dx.doi.org/10.1016/j.icarus.2017.10.003)

Golabek, G.J., Keller, T., Gerya, T.V., Zhu, G., Tackley, P.J., Connolly, J.A., 2011. Origin of the martian dichotomy and Tharsis from a giant impact causing massive magmatism. Icarus 215 (1), 346–357. [http://dx.doi.org/10.1016/J.ICARUS.2011.06.012](http://dx.doi.org/10.1016/J.ICARUS.2011.06.012)

Marinova, M.M., Aharonson, O., Asphaug, E., 2008. Mega-impact formation of the Mars hemispheric dichotomy. Nature 453 (7199), 1216–1219. [http://dx.doi.org/10.1038/nature07070](http://dx.doi.org/10.1038/nature07070)

Neumann, G.A., Zuber, M.T., Wieczorek, M.A., McGovern, P.J., Lemoine, F.G., Smith, D.E., 2004. Crustal structure of Mars from gravity and topography. J. Geophys. Res. E 109 (8), E08002. [http://dx.doi.org/10.1029/2004JE002262](http://dx.doi.org/10.1029/2004JE002262)

Zuber, M.T., 2000. Internal structure and early thermal evolution of Mars from Mars global surveyor topography and gravity. Science 287 (5459), 1788–1793. [http://dx.doi.org/10.1126/science.287.5459.1788](http://dx.doi.org/10.1126/science.287.5459.1788)
