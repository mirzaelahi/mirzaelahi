---
layout: page
title: Research
permalink: /research/
---

## Carrier Transport in Graphene  <img class="Picture" src="{{ site.baseurl }}/images/src.png" alt="uva" width="60" align="right"><img class="Picture" src="{{ site.baseurl }}/images/uva.jpg" alt="uva" width="80" align="right" hspace="5">
<p align="right" vspace="-10"><br>[Aug 2014-Till Date]</p>

We explore both analytical and numerical methods to understand various aspects of graphene’s fundamental electronic structure, device and circuit level properties. I am involved in developing multiple simulation tools ([QUEST](https://github.com/masumhabib/quest)), consisting nonequilibrium Green's function formalism and semiclassical ray tracing with quantum tunneling model included, to explore electronic transport in 2D materials, to be specific Graphene.

In freshman optics, we learn about how light behaves at interfaces - Snell's law describes its bending, Fresnel's law describes its transmission, and Malus' law describes how to extinguish it with a polarizer-analyzer pair. We demonstrate that electrons in graphene can replicate all these photonic behaviors, except they are directly tunable with gate fields and can thus show highly unconventional analogs of Snell, Fresnel and Malus' law. Using a PN junction, we demonstrated that the refractive index can be turned negative, making electrons focus without a lens. The electrons at zero degree of incidence cannot back-scatter because of symmetry rules, so they transmit through arbitrarily high voltage barriers (Klein tunneling). Using two angled junctions, we can turn back these electrons like a polarizer analyzer, except we can control the degree of polarization precisely. All these attributes come together to help us design an electron based Klein tunnel switch in graphene. Such a switch can help us turn off graphene in the absence of a band-gap, thus making good use of its high transmission speed. The switch can also be used to build analog RF devices with high cut-off frequency.

***

## Application of Finite Element Method and High Performance Computation [Jun 2013 - Dec 2013]

-   2D Poisson Solver using FEM in MATLAB.
-   Tools: MATLAB, COMSOL.
-   Supervisor: Dr. [Khalid Ashraf](https://www.linkedin.com/in/khalid-ashraf-2b8a4a33){:target="_blank"}( Post Doctoral Researcher, ASPIRE Lab, EECS, UC Berkeley)

***

## AllShare Framework Development and Windows Mobile Application <img class="Picture" src="{{ site.baseurl }}/images/samsung.png" alt="uva" width="130" align="right">

<p align="right">[May 2012 - Jul 2014]</p>
-   AllShare Framework Development for Windows 8 and Windows Phone 8
-   Project Based on Networking Protocol (TCP/IP), Networking Standard (UPnP), and Technology Standard (DLNA)
-   Used Task Parallelism and WinRT API for building framework and Windows Store App.
-   Programming Language : C++ (Native, Managed), C#

***

## Undergraduate Research -Tunnel FET [Feb 2011 - Mar 2012]
<p align="justify">
My Undergraduate thesis is on “Analytical Modeling of On and Off current of Gate on Source Tunnel FET”. This work was supervised by Dr. Md. Shofiqul Islam. Here we proposed a complete  analytical model of the TFET and insight into the working principle of the device, a TFET structure is used that has its gate placed fully on  the source not covering the channel at all. Using Kane’s model and the line tunneling concept, an analytical model is developed for the TFET’s tunnel current that includes both the drain voltage and gate voltage dependence. Important quantum phenomenon  –  subband quantization  is considered due to the narrow potential well. Particularly,  the discreteness of the subband energy levels will drastically affect the BTBT transition probabilities and hence the tunneling current. Whereas in Kane’s model the energy spectra of both the valence and the conduction bands are considered continuous, transitions from a valence band with a continuous spectrum of a conduction band consisting of discrete subbands  is considered. Thus, this thesis paper has successfully introduced the subband quantization phenomenon in the  analytical modeling of the TFET structure considered.
</p>
<p align="center">
<img class="Picture" src="{{ site.baseurl }}/images/tfet.bmp" alt="Gate on source tunnel field effect transistor" width="400" align="center">
</p>
<!--Tell us about your blog. Hopefully it's cool.-->
<!---->
<!--<ul class="listing">-->
<!--{% for post in site.categories.research %}-->
<!--  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}-->
<!--  {% if year != y %}-->
<!--    {% assign year = y %}-->
<!--    <li class="listing-seperator">{{ y }}</li>-->
<!--  {% endif %}-->
<!--  <li class="listing-item">-->
<!--    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>-->
<!--    <a href="{{ site.baseurl }}{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>-->
<!--  </li>-->
<!--{% endfor %}-->
<!--</ul>-->
