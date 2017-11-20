---
layout: default
---

# Overview

The brain is constantly receiving a dizzying amount of information. Somehow, amidst this onslaught of information, it is (usually) able to pick out the important parts of the sensory information, figure out what is going on, and come up with appropriate responses.

Doing all this requires powerful processes to parse, select, and organize incoming information, and flexibly chose outputs. Understanding the mechanisms by which the brain does this will hopefully not only provide new insight to the basic science of the brain, but also help us to understand some of the the myriad ways in which it can go wrong.

The projects outlined here seek to investigate some of these functions of the brain, typically proping hypotheses that it is neural oscillations - systematic rythmicities of brain activity - that potentially act as a mechanism underlying at least some of these processes.

All of the projects outlined here are done at the [Voytek Lab](http://voyteklab.com), with thanks and credit due to Professor Voytek and the whole lab there, and in particular research assistants Will Fox, Aeri Kim, Priya Sebastian and Luyanda Mdanda, who have worked on these projects.

Conference posters are available by clicking on the links, and where projects are close to completion, links are available to pre-prints and/or project websites. In addition to the narrative description, a chronological list of all available links is at the bottom of the page.

## Oscillation Mapping

![MEG]({{ site.url }}/assets/pics/MEG_web.png)

tl-dr: The 'what, when, and where' of cortical oscillations.

At it's core, this project simply aims to provide some extra details on the 'where, when and what' of neural oscillations. We do know quite a bit about this already, with about 100 years of investigations about these questions. However, the results thus far are often more qualitative than quantitive and often don't separate oscillations from arythmic background activity (the 1/f 'slope'). In this project, using open-access magnetoencephalography (MEG) data, we aim to systematically characterize oscillatory processes across the cortex. Using these quantitative topographies, we are also working to integrate often disparate parts of neuroscience, relating these oscillation maps to structural connectivity, gene expression and functional associations.

This project has been presented at [Biomag-2016](https://www.dropbox.com/s/actfrml5efszd4u/TDonoghue_MEGmapping_BIOMAG2016.pdf?dl=0), and [SfN-2016](https://www.dropbox.com/s/4sqn0pudpqycu4r/SebastianDonoghueEtal_MEGmapping_SfN2016.pdf?dl=0).

## Oscillatory Phase

![Phase]({{ site.url }}/assets/pics/Phase_web.png)

tl-dr: What's up with oscillatory phase? Who knows. Let's try and find out!

If I flash a very brief, dim light repeatedly, for the exact same event that happens in the world, sometimes you may see it, but sometimes you won't. Why does the brain react so differently to the same input? We're not sure, but one finding is that oscillatory phase, that is, the precise part of the rhythmic brain activity at which the flash occurs, systematically relates to your perception. This is consistent with ideas that low-frequency oscillations serve as a way to parse incoming inputs - this selection process creating rhythmic fluctuations of better (and worse) processing. We are trying to investigate these ideas, in part by using tasks to infer whether these processes relate to perceptual and/or attentional processes. We are also developing a brain-computer interface (BCI) that can selectively present stimuli at particular phases of subject's ongoing oscillations. This BCI will allow us to try new experiments, and further probe the behavioural relevance of oscillatory phase, for example, selectively presenting at particular phases to investigate whether phase-effects relate to more complex forms of cognition, such as (perceptual) learning.

The online presentation brain-computer interface and task validation was presented at [SfN-2015](https://www.dropbox.com/s/1o5whrrrukd5oy3/GougeletDonoghueEtal_RealTimePhasePresentation_SfN2015.pdf?dl=0). A follow up (offline) experiment examining the role of oscillatory phase in perceptual and/or attentional processes was presented at [SfN-2016](https://www.dropbox.com/s/gvcsj2l2dzw3ler/TDonoghue_PhaseAttention_SfN2016.pdf?dl=0).

## Automated Meta-Analysis of ERPs (and Cognition)

![ERP]({{ site.url }}/assets/pics/ERP_web.png)

tl-dr: I tried to find a shortcut to reading the ERP literature.

The neuroscience literature is already huge, with thousands of new articles published every month. Informatics offers us tools to help parse, organize and summarize the literature, but there has been limited adoption of these approaches in cognitive neuroscience. In this project, we leverage tools and ideas from informatics to help summarize and explore a particular subset of the neuroscience literature - that using the method of event-related potentials (ERPs). Using the PubMed API allows us to scrape relevant literature, and use automated procedures to create data-driven summaries of ERPs, as well as work to extract patterns from across the literature.

This project was presented at [CNS-2017](https://www.dropbox.com/s/sgnz7ecd3qp6tb7/TDonoghue_ERPSCANR_CNS2017.pdf?dl=0), and the full project is hosted online [here.](tomdonoghue.github.io/ERP_SCANR)

I have been involved in some work generalizing this text-mining approach to more broad topics, namely, all of cognition. Lead author Richard Gao worked on text-mining relations between cognitive terms, presenting and publishing a conference paper at Cognitive Science 2017, available [here](https://mindmodeling.org/cogsci2017/papers/0395/paper0395.pdf). At Neurohackweek 2017, I worked with a group on extending this code and analysis to the Cognitive Atlas, a work in progress repository is [here](https://github.com/neurohackweek/DataDrivenCognitiveOntology).

## Fitting Oscillations and One-Over F

tl-dr: Decomposing neural recordings into oscillations and background activity

This project is more a collective / lab group project in developing a method to pull apart different components of neural activity, namely rhythmic (oscillatory) activity from arrythmic, 1/f, 'background' activity. Currently, I am the core code-developer, and a big user, of this method (it's the approach behind the oscillation mapping mentioned above). For a frequency representation of neural activity, it fits a model to characterize different components of the signal. Though relatively straight-forward as a method, it comes with what we think is an important (and opinionated) conceptual advance: that oscillatory activity and 1/f background are separate processes, both independently important, but often conflated in current analyses and that they should be separated and each should only be analyzed while controlling for the other. Conveniently, this method does just that!

A piece of this work, validating the background-fitting procedure, was presented at [SfN2017](https://www.dropbox.com/s/d5zxqdw55my79dx/DonoghueT_SfN2017.pdf?dl=0).

## Links to Posters & Papers - Chronological Order

### Conference Papers

- CogSci 2017 - [Automated Generation of Cognitive Ontology via Web Text-Mining](https://mindmodeling.org/cogsci2017/papers/0395/paper0395.pdf)

### Conference Posters

- SfN 2017 - [Assessing Approaches for Estimating the Electrophysiological 1/f Background Spectrum](https://www.dropbox.com/s/d5zxqdw55my79dx/DonoghueT_SfN2017.pdf?dl=0)
- CNS 2017 - [Automated Meta-Analysis of Event-Related Potentials and their Correlates through Text-Mining](https://www.dropbox.com/s/sgnz7ecd3qp6tb7/TDonoghue_ERPSCANR_CNS2017.pdf?dl=0)
- SfN 2016 - [Data Mining to Generate Novel Hypotheses for the Genetic Underpinnings and Functional Roles of Cortical Oscillations](https://www.dropbox.com/s/4sqn0pudpqycu4r/SebastianDonoghueEtal_MEGmapping_SfN2016.pdf?dl=0)
- SfN 2016 - [The Relation of Oscillatory-Phase to Visual Perception is Dependent on Attention and Location of the Stimuli](https://www.dropbox.com/s/gvcsj2l2dzw3ler/TDonoghue_PhaseAttention_SfN2016.pdf?dl=0)
- Biomag 2016 - [Automated Analysis of Resting State Cortical Oscillatory Characteristics using Magnetoencephalography (MEG)](https://www.dropbox.com/s/actfrml5efszd4u/TDonoghue_MEGmapping_BIOMAG2016.pdf?dl=0)
- SfN 2015 - [Influencing Visual Target Detection with Oscillatory Phase-Specific Stimulus Presentation](https://www.dropbox.com/s/1o5whrrrukd5oy3/GougeletDonoghueEtal_RealTimePhasePresentation_SfN2015.pdf?dl=0)
