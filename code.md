---
layout: default
---

# Code & Resources

This page contains links to code projects I work on, as well as resources I create and curate.

* Table of Contents
{:toc}

## Overview

My work includes a lot of code development, mostly in the
[Python](https://www.python.org/) programming language,
including developing
[open-source](https://opensource.com/resources/what-open-source)
software tools, releasing code for my research projects (see the [research page](research.html)),
and well as developing code-related teaching materials (see the [teaching page](teaching.html)).

My code is on Github, including on my
[personal page](https://github.com/TomDonoghue), the
[VoytekLab page](https://github.com/voytekresearch), and is indexed
[here](https://github.com/TomDonoghue/TomDonoghue/blob/main/codemap.md).

## Open-Source Packages

Below are a list of open-source Python packages that I work on.

### SpecParam: spectral parameterization

I am the lead developer of
[specparam](https://github.com/fooof-tools/fooof)
(formerly called `fooof`), a tool for parameterizing neural power spectra.

`specparam` is a method for spectral parameterization, which takes in frequency representations of data,
and parameterizes them into periodic and aperiodic components.

[Github](https://github.com/fooof-tools/) -
[Documentation](https://fooof-tools.github.io/fooof/) -
[Pypi](https://pypi.org/project/fooof/)

### NeuroDSP: neuro digital signal processing

I am a co-developer of
[neurodsp](https://github.com/neurodsp-tools/neurodsp),
a tool for analyzing and simulating neural time series.

`neurodsp` is a set of digital signal processing (DSP) tools, designed to be used for neural time series,
including filtering, spectral analysis, time-frequency analysis, burst detection and more.

[Github](https://github.com/neurodsp-tools/neurodsp) -
[Documentation](https://neurodsp-tools.github.io/) -
[Pypi](https://pypi.org/project/neurodsp/)

### LISC: literature scanner

I am the lead developer of
[lisc](https://github.com/lisc-tools/lisc),
a tool for collecting and analyzing scientific literature.

`lisc` connects to available APIs, such as for the Pubmed database, and offers functionality to collect
scientific literature articles from them, with tools to analyze the collected results.

[Github](https://github.com/lisc-tools/lisc) -
[Documentation](https://lisc-tools.github.io/) -
[Pypi](https://pypi.org/project/lisc/)

### SpikeTools: single-neuron analysis toolbox

I am the lead developer of
[spiketools](https://github.com/spiketools/spiketools),
a tool for analyzing single-unit neural data.

`spiketools` is a collections of tools for processing and analyzing single-unit neural data.

[Github](https://github.com/spiketools/spiketools) -
[Documentation](https://spiketools.github.io/)

## Project Code

I also strive to make the code underlying individual projects openly available.

The following project have openly available analysis code:
- [Parameterizing neural power spectra](https://github.com/fooof-tools/Paper)
- [Oscillation-Methods](https://github.com/OscillationMethods/OscillationMethods)
- [ERPscanr](https://github.com/ERPscanr/ERPscanr)
- [Band Ratios](https://github.com/voytekresearch/bandratios)

## Visualizations

I also sometimes create visualizations for projects and methods, including the following projects.

You might see these visualizers show up on my
[blog](blog.html) or on my
[twitter](https://twitter.com/TomDonoghue).

### Oscillation Methods Visualizers

A collection of animated gifs for the
[Oscillation Methods](https://github.com/OscillationMethods/OscillationMethods) project,
describing methodological considerations
for measuring and interpreting periodic neural activity.

[Site](https://oscillationmethods.github.io/docs/viz.html) -
[Source](https://github.com/OscillationMethods/Visualizers)

### Digital Signal Processing Visualizers

A collection of animated plots and gifs for topics related to  digital signal processing (DSP),
especially as it relates to neural data.

[Source](https://github.com/TomDonoghue/SigViz)

### Interactive Oscillation Visualization

A small set of interactive visualizations about some common ideas in electrophysiology
and time series analysis.

[Site](http://icogsci1.ucsd.edu/~tdonoghu/) -
[Source](https://github.com/TomDonoghue/osc_viz)

## Resources

The following are resources that may be useful for organized, robust, open science,
including resources I have created, and curated links to external sources.

### Open Lists

I keep a public collection of available resources on
[OpenLists](https://github.com/OpenLists), which are listed
[here](https://github.com/openlists/Overview).

The open lists include:
- [Electrophysiology Data](https://github.com/openlists/ElectrophysiologyData),
a list of openly available electrophysiological datasets
- [Electrophysiology Software](https://github.com/openlists/ElectrophysiologySoftware),
a list of software packages for working with electrophysiology data
- [Spike Resources](https://github.com/openlists/SpikeResources),
a list of tooling and resources for single-unit neural data analysis
- [Python Resources](https://github.com/openlists/PythonResources),
a list of resources for learning Python
- [DSP Resources](https://github.com/openlists/DSPResources),
a list of resources for learning digital signal processing
- [Git Resources](https://github.com/openlists/GitResources),
a list of resources for learning git & Github

### Structured Science

I also collect and develop
[resources and templates](https://github.com/structuredscience/)
for doing organized research projects.

Mostly, this includes templates, including:

- [A general project template](https://github.com/structuredscience/ProjectTemplate)
for organizing a repository
- [An EEG project template](https://github.com/structuredscience/EEGTemplate)
for organizing and preprocessing projects with EEG data
- [A task template](https://github.com/structuredscience/TaskTemplate)
for designing and organizing code for behavioral tasks
- [A paper template](https://github.com/structuredscience/PaperTemplate)
for writing up a project
