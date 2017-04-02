---
layout: default
---

# Overview

The brain is constantly receiving a dizzying amount of information. Somehow, amidst this onslaught of information, it is (usually) able to pick out the important parts of the sensory information, figure out what is going on, and come up with appropriate responses.

Doing all this requires powerful processes to parse, select, and organize incoming information, and flexibly chose outputs. Understanding the mechanisms by which the brain does this will hopefully not only provide new insight to the basic science of the brain, but also help us to understand some of the the myriad ways in which it can go wrong.

The projects outlined here seek to investigate some of these functions of the brain, typically proping hypotheses that it is neural oscillations - systematic rythmicities of brain activity - that potentially act as a mechanism underlying at least some of these processes.

All of the projects outlined here are done at the [Voytek Lab](http://voyteklab.com), with thanks and credit due to Professor Voytek and the whole lab there, and in particular research assistants Will Fox, Aeri Kim, Priya Sebastien and Luyanda Mdanda, who have worked on these projects.

Conference posters are available by clicking on the links, and where projects are close to completion, links are available to pre-prints and/or project websites.

## Oscillation Mapping

![MEG]({{ site.url }}/assets/{{ page.title }}/pics/MEG_web.png)

tl-dr: The 'what, when, and where' of cortical oscillations.

At it's core, this project simply aims to provide some extra details on the 'where, when and what' of neural oscillations. We do know quite a bit about this already, with about 100 years of investigations about these questions.However, the results thus far are often more qualitative than quantitive and often don't separate oscillations from arythmic background activity (the 1/f 'slope'). In this project, using open-access magnetoencephalography (MEG) data, we aim to systematically characterize oscillatory processes across the cortex. Using these quantitative topographies, we are also working to integrate often disparate parts of neuroscience, relating these oscillation maps to structural connectivity, gene expression and functional associations.

This project has been presented at [Biomag-2016](https://www.dropbox.com/s/actfrml5efszd4u/TDonoghue_MEGmapping_BIOMAG2016.pdf?dl=0), and [SfN-2016](https://www.dropbox.com/s/4sqn0pudpqycu4r/SebastianDonoghueEtal_MEGmapping_SfN2016.pdf?dl=0).

## Oscillatory Phase

![Phase]({{ site.url }}/assets/{{ page.title }}/pics/Phase_web.png)

tl-dr: What's up with oscillatory phase? Who knows. Let's try and find out!

If I flash a very brief, dim light repeatedly, for the exact same event that happens in the world, sometimes you may see it, but sometimes you won't. Why does the brain react so differently to the same input? We're not sure, but one finding is that oscillatory phase, that is, the precise part of the rhythmic brain activity at which the flash occurs, systematically relates to your perception. This is consistent with ideas that low-frequency oscillations serve as a way to parse incoming inputs - this selection process creating fluctuations of better - and worse - processing times. We are trying to investigate these ideas, in part by using tasks to infer whether these processes relate to perceptual and/or attentional processes, and also by developing a brain-computer interface (BCI) that can selectively present stimuli at particular phases of individuals subjects' ongoing oscillations. This BCI will allow us to try new experiments, and further probe the behavioural relevance of oscillatory phase, for example, selectively presenting at particular phases to investigate whether phase-effects relate to more complex forms of cognition, such as (perceptual) learning.

The online presentation brain-computer interface and task validation was presented at [SfN-2015](https://www.dropbox.com/s/1o5whrrrukd5oy3/GougeletDonoghueEtal_RealTimePhasePresentation_SfN2015.pdf?dl=0). A follow up (offline) experiment examining the role of oscillatory phase in perceptual and/or attentional processes was presented at [SfN-2016](https://www.dropbox.com/s/gvcsj2l2dzw3ler/TDonoghue_PhaseAttention_SfN2016.pdf?dl=0).

## Automated Meta-Analysis of ERPs

![ERP]({{ site.url }}/assets/{{ page.title }}/pics/ERP_web.png)

tl-dr: I tried to find a shortcut to reading the ERP literature.

The neuroscience literature is already huge, with thousands of new articles published every month. Informatics offers us tools to help parse, organize and summarize the literature, but there has been limited adoption of these approaches in cognitive neuroscience. In this project, we leverage tools and ideas from informatics to help summarize and explore a particular subset of the neuroscience literature - that using the method of event-related potentials (ERPs). Using the PubMed API allows us to scrape relevant literature, and use automated procedures to create data-driven summaries of ERPs, as well as work to extract patterns from across the literature.

This project was presented at [CNS-2017](https://www.dropbox.com/s/sgnz7ecd3qp6tb7/TDonoghue_ERPSCANR_CNS2017.pdf?dl=0), and the full project is hosted online [here.](tomdonoghue.github.io/ERP_SCANR)

