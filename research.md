---
layout: default
---

This page includes a narrative overview of my research. You can also skip right to the [publications](publications.html).

# Research Overview

At the broadest level, what particularly fascinates me about the brain is the extreme flexibility we seem to have - despite a relatively fixed anatomy, we are able to quickly and flexibly react to an ever changing world. The brain is constantly receiving dizzying amounts of information. Despite this, it is (usually) able to select important inputs, figure out what is going on, and come up with appropriate responses. Doing all this requires powerful processes to parse, select, and organize incoming information, and flexibly choose and direct systematic outputs. How is it that the brain is able to organize all its seemingly chaotic activity in order to allow us to systematically respond in structured ways, ultimately allowing for allowing us to do everything that we do?

Alternately put, the brain must have some powerful organizational capacities that allow for coordinating activity. Investigating this topic can broadly be thought of as investigating the functional organization of brain activity. In my work, I focus on investigating patterns of electrical brain activity that arise from large groups of neurons. In particular, I'm involved in work focused on measuring, analyzing and interpreting both periodic activity, or neural oscillations, and aperiodic activity, sometimes described as '1/f activity', that we see in electrical recordings of the brain. From these signals we try and infer properties of physiological activity, and how this activity may relate to cognition and disease. This work includes methods development of software tools, analyzing data from open-access databases, and running novel experiments with human subjects while we record their brain activity.

In practice, my research falls into a few different components, including:
- 1) Methods Development: developing methods and software tools to analyze neural data
- 2) Descriptive Work: exploring properties and patterns of neural data at scale
- 3) Experimental Work: hypothesis-driven experiments of periodic & aperiodic neural activity
- 4) Text-Mining & Meta-Science: automated meta-analyses on the scientific literature

These projects were mostly done at the [Voytek Lab](http://voyteklab.com), with Professor Bradley Voytek and collaborators.

On the rest of this page, you can find descriptions of the following projects:
* Table of Contents
{:toc}

## Parameterizing Neural Power Spectra

![Methods]({{ site.url }}/assets/pics/methods_web.png)

Quick Version: Methods for measuring periodic and aperiodic neural activity.

Neuro-electrophysiological data contains periodic or rhythmic components, often referred to as 'neural oscillations', as well as an aperiodic or '1/f-like' activity. Each of these components has different physiological generators and interpretations. In this work, we argue that the periodic and aperiodic components of neural data should each be explicitly measured in order to ensure that analyses and interpretations appropriately describe which features of the data are changing. To do so, we have developed a method to parameterize these components from the neural power spectrum.

The method for parameterizing neural power spectra is available as an [open-source Python toolbox](https://github.com/fooof-tools/fooof), and is described in this [paper](https://doi.org/10.1038/s41593-020-00744-x). As part of this work, we have been evaluating and exploring related methods to analyze periodic and aperiodic neural activity. For example, in [this](https://doi.org/10.1523/ENEURO.0192-20.2020) paper, we examine how band-ratio measures systematically conflate periodic and aperiodic activity. We are also working on systematically compare methods for analyzing aperiodic activity, and early report of which is available in this [conference paper](https://ccneuro.org/2019/proceedings/0000783.pdf). All of this work is largely driven by simulated data, including with our [NeuroDSP](https://github.com/neurodsp-tools/neurodsp) toolbox, which is described in this [paper](https://joss.theoj.org/papers/10.21105/joss.01272).

## Electrophysiological Data Mapping & Data Integration

![MEG]({{ site.url }}/assets/pics/mapping_web.png)

Quick Version: The 'what, when, and where' of neuro-electrophysiological data.

This project investigates the 'where, when, and what' of periodic and aperiodic neural activity. Broadly, this includes characterizing both neural oscillations and aperiodic activity across the human cortex. To do so, we analyze large, open-access datasets, including a large dataset of magnetoencephalography (MEG) data, and apply our novel methods to separately measure periodic and aperiodic components. A report on this project is currently in preparation, but some initial analyses are available in the [parameterization](https://doi.org/10.1038/s41593-020-00744-x) paper, and in conference posters
([SfN2018](https://www.dropbox.com/s/alwwb6ahb1wjank/MdandaEtal-SfN2018.pdf?dl=0),
[Biomag2018](https://www.dropbox.com/s/k5koyibwuaclx5k/DonoghueEtal-Biomag2018.pdf?dl=0))

Another area of interest in this area is to integrate and analyze across different spatially-defined data modalities in neuroscience, for example, relating periodic and aperiodic activity to structural connectivity, gene expression and/or functional associations. This work is currently a work in progress, but some early results have been presented in a
[conference poster](https://www.dropbox.com/s/al0bggj4mgqffat/DonoghueEtal-Neuroinformatics2018.pdf?dl=0).

## Experimental Investigations of Oscillatory Phase

![Phase]({{ site.url }}/assets/pics/experiments_web.png)

Quick Version: How do momentary fluctuations in oscillations relate to cognition?

If I flash a very brief, dim light, for the exact same event that happens, sometimes you may see it, but sometimes you won't. Why does the brain react so differently to the same input? One finding is that oscillatory phase, that is, the precise part of the rhythmic brain activity at which the flash occurs, systematically relates to your perception. This is consistent with ideas that low-frequency oscillations serve as a way to parse incoming inputs - this selection process creating rhythmic fluctuations of better (and worse) processing.

We have been investigating these ideas, including by developing an online presentation system that can selectively present stimuli at particular phases of subject's ongoing oscillations. This system allows us to try new experiments, and further probe the behavioral relevance of oscillatory phase.

The online presentation brain-computer interface and task validation was presented at [SfN-2015](https://www.dropbox.com/s/1o5whrrrukd5oy3/GougeletDonoghueEtal_RealTimePhasePresentation_SfN2015.pdf?dl=0). A follow up (offline) experiment examining the role of oscillatory phase in perceptual and/or attentional processes was presented at [SfN-2016](https://www.dropbox.com/s/gvcsj2l2dzw3ler/TDonoghue_PhaseAttention_SfN2016.pdf?dl=0).

## Automated Meta-Analyses of the Scientific Literature

![ERP]({{ site.url }}/assets/pics/literature_web.png)

Quick Version: Computationally summarizing and investigating the scientific literature.

The scientific literature is vast and ever growing. While informatics offers tools and approaches to help parse, organize and summarize the literature, there has been relatively little adoption of these approaches in cognitive neuroscience. In this work, we develop tools and apply analyses to the scientific literature to summarize and investigate patterns in the literature.

This started with an automated meta-analysis of studies using event-related potentials (ERPs). Using the PubMed API allows us to scrape relevant literature, and use automated procedures to create data-driven summaries of ERPs. This project is hosted online [here](tomdonoghue.github.io/ERP_SCANR). To further enable this kind of approach, I created a Python module for performing collection and analysis of the scientific literature, which is available [here](https://github.com/lisc-tools/lisc), and described in this [paper](https://joss.theoj.org/papers/10.21105/joss.01674).

With Richard Gao, this work has been generalized to explore topics across cognition, resulting in a couple conference papers
([Cogsci2017](https://mindmodeling.org/cogsci2017/papers/0395/paper0395.pdf),
[CCN2019](https://ccneuro.org/2019/proceedings/0001130.pdf)).
In work led by Will Fox, we have extended this project to investigating aspects of scientific communication, in particular examining differences in conveyed confidence in the scientific literature, comparing between primary literature and press releases, which resulted in a [conference paper](http://mindmodeling.org/cogsci2018/papers/0323/index.html).
