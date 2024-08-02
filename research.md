# Research

My research focuses primarily on the inference of cosmological parameters using gravitational wave (GW) signals from compact binary coalesences (CBCs) (merging black holes or neutron stars). In particular I specialise in incorporating information from galaxy catalogues into this analysis.

I'm also the lead developer for GW cosmological inference software [gwcosmo](https://lscsoft.docs.ligo.org/gwcosmo/), which can perform bright and dark siren cosmological and population inference.

A list of ongoing and previous projects can be found below, in (approximately) reverse chronological order.


## Ongoing projects

### Analysing GWTC-4 with gwcosmo for the O4a LVK Cosmology paper
Ongoing LVK collaborative project. Look out for the paper release and data release in 2025!

### Cosmological inference combining different populations of CBCs
Ongoing project with PhD student Alex Papadopoulos, aiming to correctly combine populations of binary black holes, binary neutron stars, and neutron star-black hole mergers (and those awkward ones which fall somewhere in between...) into a single comprehensive cosmological analysis.

### Inferring the properties of host galaxies using CBC detections
Ongoing project with PhD student Zhuotao Li, investigating the prospect of distinguishing between different host galaxy weighting models using future LVK(I) detections, thus shedding light on the kinds of galaxies which host binary black hole mergers.

### Preparing gwcosmo for the era of big data
The current gwcosmo analysis is stretched with the current LVK detections and GLADE+ catalogue. With GW detections increasing (and set to expand rapidly in O5 and beyond), plus many big upcoming galaxy surveys, now is the time to power up this analysis...


## Previous projects

### Constraining modified gravity parameters using gwcosmo and GWTC-3
Project with Anson Chen and Tessa Baker while at QMUL. Anson implemented a range of modified gravity models into gwcosmo (ones which include a friction term, thus causing measured GW luminosity distance to differ from EM luminosity distance). We tested these on mock data, and then ran the analysis on GWTC-3. Spoiler: no signs of deviations from GR just yet. [Read about it here.](https://iopscience.iop.org/article/10.1088/1475-7516/2024/02/035)

### Joint population and cosmological inference
Following the third observing run, it was increasingly obvious that the dark siren + galaxy catalogue method of cosmological inference will be dominated by population assumptions, so I developed a vastly improved method for cosmological inference. This method improved the speed of gwcosmo by 3 orders of magnitude, with no loss of accuracy. The key revolves around pre-computing a line-of-sight redshift prior which contains the galaxy catalogue information as well as the completeness correction. MCMC or nested sampling can then be used to jointly estimate population parameters (such as those which describe the mass distribution and rate evolution with redshift of CBCs) alongside H0. This was implemented in gwcosmo and tested on GWTC-3 with the help of the gwcosmo development team. [Read about it here.](https://iopscience.iop.org/article/10.1088/1475-7516/2023/12/023)

### Analysing GWTC-3 with gwcosmo for the O3 LVK Cosmology paper
LVK collaborative project, applying gwcosmo to the GWTC-3 events, using the GLADE+ galaxy catalogue. This paper highlighted the impact of assuming a fixed population when doing a cosmological analysis, resulting in an easily-biased analysis. However it also highlighted the potential constraining power of gravitational wave detections on their own. [Read about it here.](https://iopscience.iop.org/article/10.3847/1538-4357/ac74bb)

### A pixelated approach to galaxy catalogue incompleteness for dark siren cosmology
Realising that galaxy catalogue completeness is highly non-uniform, both due to obscuration by the Milky Way band, and for composite catalogues which are made up of multiple surveys, I developed a pixelated method for correcting for galaxy catalogue incompleteness in a GW cosmological analysis. [Read about it here.](https://academic.oup.com/mnras/article/512/1/1127/6526882)

### Analysing GWTC-1 with gwcosmo for the O2 LVC Cosmology paper
LVC collaborative project, applying gwcosmo to the GWTC-1 GW events, using the GLADE 2.4 catalogue and the DES Y1 galaxy catalogue, to produce a measurement on H0. The fact that galaxy catalogue completeness was non-uniform across the sky led me to implement an improved analysis which assumed that the catalogue was only uniformly complete within the sky area of each GW event. [Read about it here.](https://iopscience.iop.org/article/10.3847/1538-4357/abdcb7)

### Dark siren cosmology with incomplete galaxy catalogues
Project with many LVC collaborators in the early days of my PhD. We developed the mathematical framework for incorporating incomplete galaxy catalogues into a GW cosmology analysis by modelling the incompleteness with an apparent magnitude threshold. This was implemented in an early version of gwcosmo, and tested on mock data. [Read about it here.](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.101.122001)



