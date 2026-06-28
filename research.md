---
layout: default
---

This page includes a narrative overview of my research, organized into different 'themes'.

You can also skip right to my
[publications](publications.html).

# Research Overview

The human brain is constantly receiving dizzying amounts of information.
Despite this, it is (usually) able to select important inputs, process what they mean,
and come up with appropriate responses.
To do so, the brain must have some powerful organizational capacities for coordinating activity,
allowing for the functional organization of brain activity.
With this idea in mind, in my work I focus on investigating patterns of electrical brain activity
that arise from large groups of neurons. In particular, I'm involved in work focused on measuring,
analyzing and interpreting both periodic activity (neural oscillations), and aperiodic activity
(1/f-like activity), that we see in electrical recordings of the brain.
From these signals we try and infer properties of physiological activity,
and how this activity may relate to cognition and disease.
This work includes methods development of software tools,
analyzing data from open-access databases and across clinical disorders,
running novel experiments with human participants,
and broad literature analyzes to examine other work in the field.

In practice, my research falls into a few different components, including:
- 1) Methods Development: developing methods and software tools to analyze neural data
- 2) Descriptive Work: exploring patterns of neural data in healthy & clinical populations
- 3) Experimental Work: hypothesis-driven experiments of periodic & aperiodic neural activity
- 4) Physiological Work: examining the activity of individual neurons
- 5) Text-Mining & Meta-Science: automated meta-analyses on the scientific literature

On the rest of this page, you can find descriptions of the following projects:
* Table of Contents
{:toc}

## Methods Development: Measuring Periodic & Aperiodic Activity

![Methods]({{ site.url }}/assets/pics/methods_web.png)

Quick Version: Methods for measuring periodic and aperiodic neural activity.

Neuro-electrophysiological data contains periodic or rhythmic components, often referred to as
'neural oscillations', as well as an aperiodic or '1/f-like' activity. These different periodic
& aperiodic components have different physiological generators and interpretations,
such that we argue that they should each be explicitly measured in order to ensure that analyses
and interpretations appropriately describe which features of the data are changing.
To do so, we developed a method to
[parameterize neural power spectra](https://doi.org/10.1038/s41593-020-00744-x)
into periodic and aperiodic components which is available as an
[open-source Python toolbox](https://github.com/fooof-tools/fooof),
with extensive documentation on the corresponding
[website](https://specparam-tools.github.io/).
In addition, functionality of time-domain analyses and simulations which are used across projects
are available in the
[NeuroDSP](https://github.com/neurodsp-tools/neurodsp) toolbox, also with a
[documentation website](https://neurodsp-tools.github.io/neurodsp/) and associated
[software paper](https://joss.theoj.org/papers/10.21105/joss.01272).

In related work, we evaluate and compare other methods, including
[band-ratio measures](https://doi.org/10.1523/ENEURO.0192-20.2020),
such as theta/beta, which systematically conflate periodic and aperiodic activity
Further exploring measurements related topics of neuro-physiological activity, is the
"Oscillation Methods" project, a 'methodological review' for neural oscillations, which is described in this
[paper](https://doi.org/10.1111/ejn.15361) and also hosted on this
[project website](https://oscillationmethods.github.io/).
Similarly, the "Aperiodic Methods" project, explores and compares a large collection of methods
that relate to measuring aperiodic aspects of neural activity, as described in this
[preprint](https://doi.org/10.1101/2024.09.15.613114).

## Descriptive Work: Electrophysiological Data Mapping in Healthy & Clinical Populations

![MEG]({{ site.url }}/assets/pics/mapping_web.png)

Quick Version: The 'what, when, and where' of neuro-electrophysiological data.

Descriptively, I work on projects investigating the 'what, where, and when' of periodic and
aperiodic neural activity, examining how these features vary within across healthy and
clinical populations, as well as across different brain states. The aforementioned methods
projects include examinations of large open-access datasets, which is a theme of my research.
Examinations across brain states also include an investigation of
[time-resolved analyses of sleep](https://doi.org/10.1038/s44271-025-00334-2),
led by [Mohamed S. Ameen](https://orcid.org/0000-0003-4147-490X).

Beyond examining patterns of periodic & aperiodic activity in healthy adult populations,
I also collaborate with clinical researchers on differences in electrophysiological activity
in clinical disorders.
This includes a project led by
[Madeline Robertson](https://orcid.org/0000-0002-2761-0162), on
[children with ADHD](https://doi.org/10.1152/jn.00388.2019),
reporting a difference in aperiodic activity in this group,
and a project led by
[Martina Kopčanová](https://orcid.org/0009-0004-0300-3343),
examining data from patients with
[Alzheimer's dementia]((https://doi.org/10.1016/j.nbd.2023.106380).)
which found differences in periodic, but not aperiodic activity.
More broadly, I have done a
[systematic review ](https://doi.org/10.1111/ejn.70255).
of the study of aperiodic neural activity in clinical populations,
reviewing current findings and making recommendations for future practice.

## Experimental Work: Task-Related Periodic & Aperiodic Activity

![Phase]({{ site.url }}/assets/pics/experiments_web.png)

Quick Version: How does task-related periodic and aperiodic activity support cognitive behavior

In other work, we investigate .
[task-related dynamics of aperiodic neural activity](https://doi.org/10.7554/eLife.70068).
This experiment, led by
[Leo Waschke](https://orcid.org/0000-0002-1248-9259), uses a task design including stimuli
with varying 1/f properties. By manipulating both the stimulus characteristics and the
attentional focus of the subjects, we were able to show how perceptual and attentional
task elements systematically affect event-related aperiodic neural activity.

In other work led by
[Quirine van Engen](https://orcid.org/0000-0002-7488-211X),
we investigated periodic and aperiodic activity in a
[visual working memory task](https://doi.org/10.1523/JNEUROSCI.2340-24.2025),
finding task-related variations in aperiodic activity that appear to at least
partially explain changes in the theta band.

## Physiological Work: Examining the Activity of Individual Neurons

![Neurons]({{ site.url }}/assets/pics/neurons_web.png)

Quick Version: Investigating patterns of single-unit activity.

The aforementioned work examines patterns of neural activity that can be examined from the
local field potential, which reflects activity across large numbers of neurons.
To also examine the activity of individual neurons, I also work on projects that examine
the activity of individual neurons as recorded from neuro-surgical patients.
To support these project methodologically, we developed the
[Human Single-Neuron pipeline](https://hsnpipeline.github.io/), a pipeline for
[managing human single-neuron projects](https://doi.org/10.52294/001c.160356),
which also includes the
[spiketools](https://github.com/spiketools/spiketools) Python module for analyzing
single-neurons recordings, also with a
[documentation website](https://spiketools.github.io/spiketools/) and
[software paper](https://doi.org/10.21105/joss.05268).

In empirical single-neuron work, with [Claire Z Han](https://orcid.org/0000-0001-9710-8381)
and [Runnan Cao](https://orcid.org/0000-0001-5827-9903) we ran a multi-task experiment examining
neural responses to faces and objects, comparing between an n-back memory task and a spatial
navigation episodic memory task, finding neurons in the human medial temporal lobe that
[flexibly shift representations across different behavioral contexts](https://doi.org/10.1002/hipo.23539).
We further discuss this design of paired tasks in this
[perspective piece](https://doi.org/10.1002/hipo.23540).
In other work led by
[Weijia Zhang](https://orcid.org/0000-0003-2644-9976), we investigated
[methodological properties of place-cell analyses](https://doi.org/10.1371/journal.pcbi.1013488),
including examinations across species.

## Meta-Science: Automated Meta-Analyses of the Scientific Literature

![ERP]({{ site.url }}/assets/pics/literature_web.png)

Quick Version: Computationally summarizing and investigating the scientific literature.

I also develop and use automated measures to examine literature data,
in order to examine trends and patterns in the ever-growing scientific literature.
To do so, I created the
[lisc](https://github.com/lisc-tools/lisc)
Python module to collect and analyze the scientific literature,
which also has a
[documentation website](https://lisc-tools.github.io/lisc/) and
[software paper](https://doi.org/10.21105/joss.01674).
This tool uses the PubMed API to find and collect relevant literature,
with associated functionality for analyzing large collections of scientific literature.

Applications of this approach are included in several previously mentioned projects
(band-ratios, aperiodic methods, etc). Another application is the
[ERPscanr project](https://doi.org/10.1038/s41598-022-05939-9),
also hosted on a [project website](http://erpscanr.github.io/), which is a
an automated literature analysis of the event-related potential (ERPs) literature,
including data-driven summaries of individual ERPs, and comparisons across components.
