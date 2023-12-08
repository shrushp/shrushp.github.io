---
layout: page
title: Quantification of quantum chaos using OTOCs 
description: Semester Project
img: assets/img/otoc.png
importance: 6
category: Minor 
---

The notion of chaos is central to understanding some of the fundamental aspects of statistical mechanics such as ergodicity and thermalization. Chaos in classical mechanics is well defined as the sensitivity of a system to arbitrarily small changes of its initial conditions, charecterized by Lyapunov exponent e.g. the growth rate of separation of two trajectories that are nearby at initial time. On the other side the definition and characterization of chaos in unitary quantum dynamics is a topical subject of investigation, in a recent developement chaos in quantum systems was charecterized as the spatio-temporal growth rate (“quantum Lyapunov exponent”) of an out of time order correlation(OTOC) of non compatiable local operators. In classical mechanics there is
no bound on the Lyapunov exponent but recently a bound on the “quantum Lyapunov exponent” was argued that depends on Temperature of the system and the Planck constant.


This bound can be understood by visualizing a semi-classical chaotic dynamics as a thermal wave packet of a single particle moving in a high dimensional phase space trajectory; where the bound appears as the impossibility to scatter the wave packet due to the curvature of the trajectory caused by a complex chaotic landscape over characteristic lengths smaller than the thermal
deBroglie wavelength. This semi-classical picture encourages one to think the quantum bound of chaos to be underpinned by the classical characteristics of a system and suggests the following property for a maximally chaotic system: the underlying classical system must have a spectra of chaotic length scales (trajectory curvatures) with no IR cut-off, such that even at the lowest possible energy the system has chaotic length scales below the deBroglie wavelength. Examples of such systems include various critical systems, specifically SYK model of quantum glasses , black holes are heavily investigated from this perspective. While this semiclassical picture gives some understanding based on quantum corrections on classical trajectories, it is still an open question how one can think about chaos in a purely quantum mechanical system where there is no
concept of trajectory.

In this work we attempt to work towards these questions by studying various quantum mechanical systems and trying to understand the interrelation of “quantum Lyapunov exponent” and the classical Lyapunov exponent. 

We calculated OTOC for various quantum mechanical systems (single particle) –Simple Harmonic Oscillator, particle in a box, stadium billiard, Inverse Simple Harmonic Oscillator, inverse square, coupled oscillator.



<div class="row">
    <div class="col-sm mt-1 mt-md-0">
        {% include figure.html path="assets/img/otoc_particle.png" title="otoc" class="img-fluid rounded z-depth-1" style="width: 20px; height: auto;" %}
    </div>
</div>
<div class="caption">
   Thermal OTOCs for particle in a box.
</div>

After that we calculate the OTOC for the inverse square potentials. A 

<div class="row">
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/n50.png" title="inv sq" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/n30.png" title="inv sq" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   Microcanonical OTOCs for inverse square potential.  
</div>

Here, you can see the polynomial growth of OTOC suggesting the presence of chaos!

Here is a overview of the chaos and scrambling: 
<table border="1">
    <tr>
        <th colspan="4">Comparison table</th>
    </tr>
    <tr>
        <th>Dynamical systems</th>
        <th>Scrambling</th>
        <th>Chaos</th>
        <th>Nature of OTOC</th>
    </tr>
    <tr>
        <td>Particle in a box</td>
        <td>not present</td>
        <td>not present</td>
        <td>Does not grow exponentially in time</td>
    </tr>
    <tr>
        <td>Stadium billiard</td>
        <td>not present</td>
        <td>present</td>
        <td>Does not grow exponentially in time</td>
    </tr>
    <tr>
        <td>Harmonic oscillator</td>
        <td>not present</td>
        <td>not present</td>
        <td>Does not grow exponentially in time</td>
    </tr>
    <tr>
        <td>Inverted harmonic oscillator</td>
        <td>present</td>
        <td>not present</td>
        <td>Grows exponentially in time</td>
    </tr>
    <tr>
        <td>Coupled harmonic oscillator</td>
        <td>present</td>
        <td>present</td>
        <td>Grows exponentially in time</td>
    </tr>
</table>
