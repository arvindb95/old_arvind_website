---
layout: page
title: Masters Thesis
description: Transient localization with CZTI
img: /assets/img/Astrosat.png
thumbnail_credit: "Transient localization with CZTI"
importance: 3
category: work
---

Astrophysical transients are short timescale events, usually lasting from a few seconds to a few hundred seconds, and are sometimes associated with cataclysmic events like death of a star or merger of compact objects. This thesis focuses on the search for and study of astrophysical transients with the Cadmium Zinc Telluride Imager ([CZTI](http://astrosat.iucaa.in/czti/?q=home)), on-board [AstroSat](https://www.isro.gov.in/astrosat-0). At energies higher than 100 keV, CZTI functions as an open detector and is sensitive to transients from all over the sky. This makes it a very sensitive detector for various classes of astrophysical transients: Gamma Ray Bursts (GRBs), and even X-ray counterparts to gravitational wave events. As an all-sky detector, CZTI can detect transients shining through the satellite body. The analysis, localisation, and interpretation of this data requires a complete understanding of the absorption, scattering, and reprocessing of the incident photons by various elements of the satellite.

<div class="row justify-content-md-center" style="margin-top: 50px;">
   <img class="img-fluid" style="width: 50%; border-radius: 5px; float: right;" src="{{ '/assets/img/energy_redistributed.png' | relative_url }}" alt="" title="Energy redistribution"/>
</div>
<div class="caption">
   Photons of different energies incident on the CZTI detector get redistributed to lower energies due to interactions with satellite body.
</div>

Such interactions are impossible to compute analytically in a photon starved regime, since many of them are non-deterministic. This warrants the need for a simulation. A simulated “mass model” of the satellite has been developed using the [GEANT4 simulation package](https://geant4.web.cern.ch/). The thesis involved devising a method to compare the simulated transients to real ones to obtain an independent localisation to assist multimessenger observations. You can access the thesis document [here](/assets/pdf/Arvind_MS_Thesis_Final_Draft.pdf){:target="_blank"}.
