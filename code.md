---
layout: default
---

# Code

This page contains links to code projects that I work on.

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
Note that code specifically related to
[teaching](teaching.html)
and/or
[resources](resources.html)
(such as visualizations) are listed on those pages.

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
[PyPI](https://pypi.org/project/fooof/)

### NeuroDSP: neuro digital signal processing

I am a co-developer of
[neurodsp](https://github.com/neurodsp-tools/neurodsp),
a tool for analyzing and simulating neural time series.

`neurodsp` is a set of digital signal processing (DSP) tools, designed to be used for neural time series,
including filtering, spectral analysis, time-frequency analysis, burst detection and more.

[Github](https://github.com/neurodsp-tools/neurodsp) -
[Documentation](https://neurodsp-tools.github.io/) -
[PyPI](https://pypi.org/project/neurodsp/)

### LISC: literature scanner

I am the lead developer of
[lisc](https://github.com/lisc-tools/lisc),
a tool for collecting and analyzing scientific literature.

`lisc` connects to available APIs, such as for the Pubmed database, and offers functionality to collect
scientific literature articles from them, with tools to analyze the collected results.

[Github](https://github.com/lisc-tools/lisc) -
[Documentation](https://lisc-tools.github.io/) -
[PyPI](https://pypi.org/project/lisc/)

### SpikeTools: single-neuron analysis toolbox

I am the lead developer of
[spiketools](https://github.com/spiketools/spiketools),
a tool for analyzing single-unit neural data.

`spiketools` is a collections of tools for processing and analyzing single-unit neural data.

[Github](https://github.com/spiketools/spiketools) -
[Documentation](https://spiketools.github.io/) -
[PyPI](https://pypi.org/project/spiketools/)

## Pipelines

Pipelines for processing particular datatypes.

### Human Single-Unit Pipeline

`HSUPipeline` is a pipeline for processing and analyzing single-unit neural data from human subjects.
It includes templates for pre-processing, organizing, and analyzing human single-unit data.

[Github](https://github.com/HSUpipeline/) -
[Website](https://hsupipeline.github.io/)

## Project Code

I also strive to make the code underlying individual projects openly available.

The following project have openly available analysis code:
- [Single neurons in the human medial temporal lobe flexibly shift representations across spatial and memory tasks](https://github.com/HSUpipeline/analyzeTH)
- [Frequency band ratio measures conflate periodic and aperiodic neural activity](https://github.com/voytekresearch/bandratios)
- [Parameterizing neural power spectra into periodic and aperiodic components](https://github.com/fooof-tools/Paper)
- [Methodological considerations for studying neural oscillations](https://github.com/OscillationMethods/OscillationMethods)
- [Automated meta-analysis of the event-related potential (ERP) literature](https://github.com/ERPscanr/ERPscanr)
