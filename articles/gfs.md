---
title: GFS
subtitle: "Last content update: jun, 2019"
layout: page
hero_height: is-medium
menubar: gfs-menu
content_width: is-8
show_sidebar: true
---

<div class="title is-4" id="vertical-coordinate-system">Vertical Coordinate System</div>

<p>The FV3 - Global Forecast Model (FV3 - GFS) uses a hybrid sigma-pressure (σ-p) coordinate in the vertical direction, with a gradual transition from full sigma at the surface to full pressure at about 70 hPa. Operationally, the FV3 - GFS has 64 unevenly spaced vertical layers, concentrated in the planetary boundary layer and near the tropopause. The top layer is centered at about 0.3 hPa and the bottom layer at about 997.3 hPa. for surface pressure of 1000 hPa.</p>

<p>The vertical levels are not used directly for computations of vertical motions, since the 3-dimensional finite volume is advected following the volume (i.e. Lagrangian/ “follow the parcel” computations). Every several timesteps, the volume is re-interpolated to the hybrid sigma-pressure (σ-p) levels.</p>

<div class="title is-5 mt-5">Operational Impacts of the Hybrid Sigma-Pressure Coordinate</div>

<p>The main benefits of the hybrid coordinate in areas of rugged terrain are more accurate:</p>

<ul>
<li>pressure gradient force calculations</li>
<li>vertical advection of forecast quantities</li>
<li>jet stream level and stratospheric wind and height forecasts</li>
<li>assimilation of satellite radiances because of better stratospheric forecasts</li>
</ul>

<p>The spacing of the vertical levels and their flattening with decreasing pressure can be seen the graphic below.</p>

<figure class="is-flex is-justify-content-center">
    <img alt="GFS Hybrid Sigma Pressure Levels Over North America" src="/img/articles/gfs/gfs-hybrid-sigma-pressure-levels-over-north-america.jpg">
</figure>

<p>For more information on the hybrid σ-p coordinate system, see the <a href="https://www.meted.ucar.edu/nwp/model_structure/print.htm#page_2.5.2">Vertical Coordinate section</a> of NWP Training Series Course 1: Impact of model structure and dynamics.</p>

