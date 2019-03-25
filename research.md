---
layout: default
---

# Overview

The brain is constantly receiving a dizzying amount of information. Somehow, amidst this onslaught of information, it is (usually) able to pick out the important parts of the sensory information, figure out what is going on, and come up with appropriate responses. Doing all this requires powerful processes to parse, select, and organize incoming information, and flexibly choose and direct systematic outputs. Ultimately, these questions about the fundamentals of brain organization are what interest me the most, both as a question within basic neuroscience, and also for the potential to relate these findings to issues within the clinical domain.

In practice, I study these general questions by investigating patterns and experiments using neuro-electrophysiological data, usually EEG / MEG / ECoG recordings with human subjects. This research program broadly falls into 4 components - 1) a methods development component, in which we work to develop better methods to analyze this kind of data  2) descriptive work, in which we apply these methods at scale, systematically exploring properties of the data and integrating these findings with other areas of neuroscience 3) an experimental component, in which we design and run hypothesis driven experiments investigating how these properties relate to behaviour and cognition and 4) a more general meta-science component, in which we apply computational approaches to meta-analyze the scientific literature.

All of the projects outlined here are done at the [Voytek Lab](http://voyteklab.com), with thanks and credit due to Professor Voytek and the whole lab there, as well as our collaborators. Special thanks are due to research assistants Will Fox, Aeri Kim, Priya Sebastian, Luyanda Mdanda, Tianyu Zhang and Julio Dominguez who have worked on these projects, sometimes as the lead researcher.

Journal articles, preprints, conference papers, posters and project websites are available by clicking on the links. In addition to the narrative description organized by project topic, a chronological list of all available links is at the bottom of the page.

## Parameterizing Neural Power Spectra

tl-dr: Methods development for decomposing neuro-electrophysiological recordings into periodic and aperiodic components.

Neuro-electrophysiological data contain periodic components, called neural oscillations, that sit atop an aperiodic '1/f' background. Properly separating these two components is fundamentally important for good measurement and appropriate interpretations of neuro-electrophysiological data. We have developed a method to do, that operates on neural power spectra (frequency representations), and seeks to parameterize them by 'fitting oscillations and one-over f' components, and is thus called FOOOF. Though relatively straight-forward as a method, it comes with what we think is an important (and opinionated) conceptual advance: that oscillatory activity and 1/f background are separate processes, both independently important, but often conflated in current analyses and that they should be separated and each should only be analyzed while controlling for the other. Conveniently, this method does just that!

The code for this method is available on Github[here](https://github.com/voytekresearch/fooof), and a full description is currently available as a [preprint](https://www.biorxiv.org/content/early/2018/04/11/299859). A piece of this work, validating the background-fitting procedure, was also presented at [SfN2017](https://www.dropbox.com/s/d5zxqdw55my79dx/DonoghueT_SfN2017.pdf?dl=0).

## Electrophysiological Data Mapping & Data Integration

![MEG]({{ site.url }}/assets/pics/MEG_web.png)

tl-dr: Descriptive work exploring the 'what, when, and where' of electrophysiological data, and integrating this with other modalities

At it's core, this project simply aims to provide some extra details on the 'where, when and what' of neural oscillations. We do know quite a bit about this already, with about 100 years of investigations about these questions. However, the results thus far are often more qualitative than quantitive and often don't separate oscillations from arythmic background activity (the 1/f 'slope'). In this project, using open-access magnetoencephalography (MEG) data, we aim to systematically characterize oscillatory processes across the cortex. Using these quantitative topographies, we are also working to integrate often disparate parts of neuroscience, relating these oscillation maps to structural connectivity, gene expression and functional associations.

This project has been presented at [Biomag-2016](https://www.dropbox.com/s/actfrml5efszd4u/TDonoghue_MEGmapping_BIOMAG2016.pdf?dl=0), and [SfN-2016](https://www.dropbox.com/s/4sqn0pudpqycu4r/SebastianDonoghueEtal_MEGmapping_SfN2016.pdf?dl=0).

## Experimental Investigations of Oscillatory Phase

![Phase]({{ site.url }}/assets/pics/Phase_web.png)

tl-dr: Hypothesis driven experimental work probing questions about how patterns of brain activity relate to behaviour and cognition

If I flash a very brief, dim light repeatedly, for the exact same event that happens in the world, sometimes you may see it, but sometimes you won't. Why does the brain react so differently to the same input? We're not sure, but one finding is that oscillatory phase, that is, the precise part of the rhythmic brain activity at which the flash occurs, systematically relates to your perception. This is consistent with ideas that low-frequency oscillations serve as a way to parse incoming inputs - this selection process creating rhythmic fluctuations of better (and worse) processing. We are trying to investigate these ideas, in part by using tasks to infer whether these processes relate to perceptual and/or attentional processes. We are also developing a brain-computer interface (BCI) that can selectively present stimuli at particular phases of subject's ongoing oscillations. This BCI will allow us to try new experiments, and further probe the behavioural relevance of oscillatory phase, for example, selectively presenting at particular phases to investigate whether phase-effects relate to more complex forms of cognition, such as (perceptual) learning.

The online presentation brain-computer interface and task validation was presented at [SfN-2015](https://www.dropbox.com/s/1o5whrrrukd5oy3/GougeletDonoghueEtal_RealTimePhasePresentation_SfN2015.pdf?dl=0). A follow up (offline) experiment examining the role of oscillatory phase in perceptual and/or attentional processes was presented at [SfN-2016](https://www.dropbox.com/s/gvcsj2l2dzw3ler/TDonoghue_PhaseAttention_SfN2016.pdf?dl=0).

## Automated Meta-Analysis of Scientific Literature: Cognition, ERPs & Scientific Communication

![ERP]({{ site.url }}/assets/pics/ERP_web.png)

tl-dr: Trying to computationally summarize and investigate scientific literature

The scientific literature is already huge, with thousands of new articles published every month. Informatics offers us tools to help parse, organize and summarize the literature, but there has been limited adoption of these approaches in cognitive neuroscience. In a group of related projects, we leverage tools and ideas from informatics to help summarize and explore particular subsets and components of the scientific literature.

This started with an automated meta-analysis of a subset of the neuroscientific literature - that using the method of event-related potentials (ERPs). Using the PubMed API allows us to scrape relevant literature, and use automated procedures to create data-driven summaries of ERPs, as well as work to extract patterns from across the literature. This project was presented at [CNS-2017](https://www.dropbox.com/s/sgnz7ecd3qp6tb7/TDonoghue_ERPSCANR_CNS2017.pdf?dl=0), and the full project is hosted online [here.](tomdonoghue.github.io/ERP_SCANR)

In collaborative work lead by [Richard Gao](http://www.rdgao.com), we generalized this approach to more broad topics, namely, all of cognition. Using similar approaches, Richard mined and investigated relations between cognitive terms. This work is available as a conference paper from Cognitive Science 2017, available [here](https://mindmodeling.org/cogsci2017/papers/0395/paper0395.pdf).

Working with my student Will Fox, we have extended this project to investigating aspects of scientific communication, namely by examing differences in conveyed confidence in the scientific literature, comparing between primary literature and press releases. This work is also available as a conference paper from Cognitive Science 2018 [here](http://mindmodeling.org/cogsci2018/papers/0323/index.html), as well as the associated [poster](https://www.dropbox.com/s/i41jllv5ojf9qno/Fox%26Donoghue_ConfidenceScanner_CogSciPoster.pdf?dl=0).

If you are interested in these kinds of analysis, a generalized Python module for performing the text-mining is available [here](https://github.com/TomDonoghue/lisc).

## Links to Posters & Papers - Chronological Order

### Pre-Prints

- Biorchiv 2018 - [Parameterizing Neural Power Spectra](https://www.biorxiv.org/content/early/2018/04/11/299859)

### Conference Papers

- CogSci 2018 - [Confidence Levels in Scientific Writing: Automated Mining of Primary Literature and Press Releases](http://mindmodeling.org/cogsci2018/papers/0323/index.html)
- CogSci 2017 - [Automated Generation of Cognitive Ontology via Web Text-Mining](https://mindmodeling.org/cogsci2017/papers/0395/paper0395.pdf)

### Conference Posters

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
