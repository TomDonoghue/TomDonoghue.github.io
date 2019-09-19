---
layout: default
---

# Overview

The brain is constantly receiving dizzying amounts of information. Despite this, it is (usually) able to select important inputs, figure out what is going on, and come up with appropriate responses. Doing all this requires powerful processes to parse, select, and organize incoming information, and flexibly choose and direct systematic outputs.

In my research, I am broadly interested in questions about how we are able to do this - in particular, questions about functional brain organization, mechanisms of coordinated activity, and how it is that the brain is able to have such flexible and powerful dynamics. In practice, I try to investigate these kinds of questions by analyzing neuro-electrophysiological data, usually EEG / MEG / ECoG recordings with human subjects, and developing methods and software tools to analyze such data.

In practice, my research falls into a few different components, including:
- 1) Methods Development: developing methods and software tools to analyze neural data
- 2) Descriptive Work: exploring properties and patterns of neural data at scale
- 3) Experimental Work: hypothesis-driven experiments of periodic & aperiodic neural activity
- 4) Text-Mining & Meta-Science: automated meta-analyses on the scientific literature

All of the projects outlined here are done at the [Voytek Lab](http://voyteklab.com), with Professor Bradley Voytek, including work with collaborators. Special thanks to research assistants inclduing Will Fox, Aeri Kim, Priya Sebastian, Luyanda Mdanda, Julio Dominguez, Fenglin Zhang, Tyler Farnan, Meyhaa Buvanesh and Lakshmi Menon.

Journal articles, preprints, conference proceedings, posters and project websites are available by clicking on the links. In addition to the narrative description organized by project topic, a chronological list of all available links is at the bottom of the page.

## Parameterizing Neural Power Spectra

Quick Version: Methods for measuring periodic and aperiodic neural activity.

Neuroelectrophysiological data contains periodic or rhythmic components, often referred to as 'neural oscillations', as well as an aperiodic or '1/f-like' component. When trying to measure and interpret one or the other of tese components in neural data, it is important to explicitly control for the other, else measurements and interpretations can be confounded. Measuring these components specifically requires tools and approaches that explicitly deal with both components.

We have developed a method for measuring periodic and aperiodic activity from neural data, that operates on neural power spectra (frequency representations). This approach seeks to parameterize and measure each component explicitly and separately, so that analyses can investigate which components of neural data are changing. The code for this method is available [here](https://github.com/fooof-tools/fooof), and a full description is currently available as a [preprint](https://www.biorxiv.org/content/early/2018/04/11/299859).

This approach embodies the notion that that oscillatory activity (periodic components) and 1/f-like activity (the aperiodic component) are separate processes, and should be measured explicitly, else measures can conflate the two. In related work, we have explored how these components can be conflated in many analysis approaches, for example, examing how 1/f-like activity influences oscillatory band-ratio measures, a project that was presented at [CNS-2019](https://www.dropbox.com/s/4lghj9218s4hgix/DomiguezEtal_BandRatiosPoster.pdf?dl=0).

As part of this work, we have been evaluating and exporing related methods to analyze periodic and aperiodic neural activity. Part of this line of work, exploring 1/f methods and results, was presented at [SfN-2017](https://www.dropbox.com/s/d5zxqdw55my79dx/DonoghueT_SfN2017.pdf?dl=0). Follow up work developing a simulation based approach and using this to explore method properties and adjudicate between them has been presented at [CCN-2019](https://www.dropbox.com/s/9qrxrswf4x6w4iq/DonoghueEtal-CCN2019.pdf?dl=0), with an associated conference proceedings [paper](https://ccneuro.org/2019/proceedings/0000783.pdf).

## Electrophysiological Data Mapping & Data Integration

![MEG]({{ site.url }}/assets/pics/MEG_web.png)

Quick Version: The 'what, when, and where' of neuroelectrophysiological data.

At it's core, this project simply aims to provide some extra details on the 'where, when and what' of periodic and aperiodic  neural activity. There is a rich history of exploring and mapping periodic activity in particular, often referred to as neural oscillations. However, the majority of this work has not systematically separated periodic components from aperiodic neural activity, and typically uses pre-defined frequency ranges.

In this project, using open-access datasets, including a large corpus of magnetoencephalography (MEG) data, we aim to systematically characterize oscillatory processes and aperiodic components across the cortex. Using these quantitative topographies, we are also working to integrate often disparate parts of neuroscience, relating these oscillation maps to structural connectivity, gene expression and functional associations.

This project has been presented at [Biomag-2016](https://www.dropbox.com/s/actfrml5efszd4u/TDonoghue_MEGmapping_BIOMAG2016.pdf?dl=0), and [SfN-2016](https://www.dropbox.com/s/4sqn0pudpqycu4r/SebastianDonoghueEtal_MEGmapping_SfN2016.pdf?dl=0).

## Experimental Investigations of Oscillatory Phase

![Phase]({{ site.url }}/assets/pics/Phase_web.png)

Quick Version: How do momentary fluctuations in oscillations relate to cognition?

If I flash a very brief, dim light repeatedly, for the exact same event that happens in the world, sometimes you may see it, but sometimes you won't. Why does the brain react so differently to the same input? We're not sure, but one finding is that oscillatory phase, that is, the precise part of the rhythmic brain activity at which the flash occurs, systematically relates to your perception. This is consistent with ideas that low-frequency oscillations serve as a way to parse incoming inputs - this selection process creating rhythmic fluctuations of better (and worse) processing. We are trying to investigate these ideas, in part by using tasks to infer whether these processes relate to perceptual and/or attentional processes. We are also developing a brain-computer interface (BCI) that can selectively present stimuli at particular phases of subject's ongoing oscillations. This BCI will allow us to try new experiments, and further probe the behavioural relevance of oscillatory phase, for example, selectively presenting at particular phases to investigate whether phase-effects relate to more complex forms of cognition, such as (perceptual) learning.

The online presentation brain-computer interface and task validation was presented at [SfN-2015](https://www.dropbox.com/s/1o5whrrrukd5oy3/GougeletDonoghueEtal_RealTimePhasePresentation_SfN2015.pdf?dl=0). A follow up (offline) experiment examining the role of oscillatory phase in perceptual and/or attentional processes was presented at [SfN-2016](https://www.dropbox.com/s/gvcsj2l2dzw3ler/TDonoghue_PhaseAttention_SfN2016.pdf?dl=0).

## Automated Meta-Analysis of Scientific Literature: Cognition, ERPs & Scientific Communication

![ERP]({{ site.url }}/assets/pics/ERP_web.png)

Quick Version: Computationally summarize and investigating the scientific literature.

The scientific literature is vast and ever growing. While informatics offers tools and approaches to help parse, organize and summarize the literature, there has been relatively little adoption of these approaches in cognitive neuroscience. In this work, we develop tools and apply analyses to the scientific literature to.

This started with an automated meta-analysis of a subset of the neuroscientific literature - that using the method of event-related potentials (ERPs). Using the PubMed API allows us to scrape relevant literature, and use automated procedures to create data-driven summaries of ERPs, as well as work to extract patterns from across the literature. This project was presented at [CNS-2017](https://www.dropbox.com/s/sgnz7ecd3qp6tb7/TDonoghue_ERPSCANR_CNS2017.pdf?dl=0), and the full project is hosted online [here.](tomdonoghue.github.io/ERP_SCANR)

In collaborative work lead by [Richard Gao](http://www.rdgao.com), we generalized this approach to more broad topics, namely, all of cognition. Using similar approaches, Richard mined and investigated relations between cognitive terms. This work is available as a conference paper from Cognitive Science 2017, available [here](https://mindmodeling.org/cogsci2017/papers/0395/paper0395.pdf).

In work lead by Will Fox, we have extended this project to investigating aspects of scientific communication, in particular examining differences in conveyed confidence in the scientific literature, comparing between primary literature and press releases. This work is also available as a conference paper from Cognitive Science 2018 [here](http://mindmodeling.org/cogsci2018/papers/0323/index.html), as well as the associated [poster](https://www.dropbox.com/s/i41jllv5ojf9qno/Fox%26Donoghue_ConfidenceScanner_CogSciPoster.pdf?dl=0).

If you are interested in these kinds of analysis, our Python module for performing collection and analysis of the scientific literature is available [here](https://github.com/lisc-tools/lisc).

## Links to Posters & Papers - Chronological Order

### Pre-Prints

- Biorchiv 2018 - [Parameterizing Neural Power Spectra](https://www.biorxiv.org/content/early/2018/04/11/299859)

### Conference Proceedings

- CCN 2019 - [A Simulation-Based Comparison of Methods for Analyzing Aperiodic Neural Activity](https://ccneuro.org/2019/proceedings/0000783.pdf) DOI: https://doi.org/10.32470/CCN.2019.1394-0
- CCN 2019 - [Aperiodic EEG activity tracks 1/f stimulus characteristics and the allocation of cognitive resources](https://ccneuro.org/2019/proceedings/0000936.pdf) DOI: https://doi.org/10.32470/CCN.2019.1111-0
- CCN 2019 - [The Structure of Cognition Across Computational Cognitive Neuroscience](https://ccneuro.org/2019/proceedings/0001130.pdf) DOI: https://doi.org/10.32470/CCN.2019.1426-0
- CogSci 2018 - [Confidence Levels in Scientific Writing: Automated Mining of Primary Literature and Press Releases](http://mindmodeling.org/cogsci2018/papers/0323/index.html)
- CogSci 2017 - [Automated Generation of Cognitive Ontology via Web Text-Mining](https://mindmodeling.org/cogsci2017/papers/0395/paper0395.pdf)

### Conference Posters

- CCN 2019 - [A Simulation-Based Comparison of Methods for Analyzing Aperiodic Neural Activity](https://www.dropbox.com/s/9qrxrswf4x6w4iq/DonoghueEtal-CCN2019.pdf?dl=0)
- CNS 2019 - [Electrophysiological Frequency Band Ratio Measures Conflate Periodic & Aperiodic Changes](https://www.dropbox.com/s/4lghj9218s4hgix/DomiguezEtal_BandRatiosPoster.pdf?dl=0)
- SfN 2018 - [Parameterization of Periodic and Aperiodic Human Electrophysiology](https://www.dropbox.com/s/alwwb6ahb1wjank/MdandaEtal-SfN2018.pdf?dl=0)
- Biomag 2018 - [Large-Scale Topographical Analysis of Electrophysiological 1/f and Oscillations Reveals Patterns of Spatial Variation](https://www.dropbox.com/s/k5koyibwuaclx5k/DonoghueEtal-Biomag2018.pdf?dl=0)
- INCF 2018 - [Integrating Human Electrophysiology, Gene Expression and Functional Data](https://www.dropbox.com/s/al0bggj4mgqffat/DonoghueEtal-Neuroinformatics2018.pdf?dl=0)
- CogSci 2018 - [Confidence Levels in Scientific Writing](https://www.dropbox.com/s/i41jllv5ojf9qno/Fox%26Donoghue_ConfidenceScanner_CogSciPoster.pdf?dl=0)
- CNS 2018 - [Alpha Power and 1/f Slope Provide Independent Decoding of Visual Spatial Attention](https://www.dropbox.com/s/72y86jege2lx0sf/Donoghue&Voytek_CNS2018_EEGDecoding.pdf?dl=0)
- SfN 2017 - [Assessing Approaches for Estimating the Electrophysiological 1/f Background Spectrum](https://www.dropbox.com/s/d5zxqdw55my79dx/DonoghueT_SfN2017.pdf?dl=0)
- CNS 2017 - [Automated Meta-Analysis of Event-Related Potentials and their Correlates through Text-Mining](https://www.dropbox.com/s/sgnz7ecd3qp6tb7/TDonoghue_ERPSCANR_CNS2017.pdf?dl=0)
- SfN 2016 - [Data Mining to Generate Novel Hypotheses for the Genetic Underpinnings and Functional Roles of Cortical Oscillations](https://www.dropbox.com/s/4sqn0pudpqycu4r/SebastianDonoghueEtal_MEGmapping_SfN2016.pdf?dl=0)
- SfN 2016 - [The Relation of Oscillatory-Phase to Visual Perception is Dependent on Attention and Location of the Stimuli](https://www.dropbox.com/s/gvcsj2l2dzw3ler/TDonoghue_PhaseAttention_SfN2016.pdf?dl=0)
- Biomag 2016 - [Automated Analysis of Resting State Cortical Oscillatory Characteristics using Magnetoencephalography (MEG)](https://www.dropbox.com/s/actfrml5efszd4u/TDonoghue_MEGmapping_BIOMAG2016.pdf?dl=0)
- SfN 2015 - [Influencing Visual Target Detection with Oscillatory Phase-Specific Stimulus Presentation](https://www.dropbox.com/s/1o5whrrrukd5oy3/GougeletDonoghueEtal_RealTimePhasePresentation_SfN2015.pdf?dl=0)
