---
title: Cog-Sci of Data Wrangling
date: 2017-04-16
categories: ds
layout: post
comments: true
show: true
---

This week I gave a guest lecture in the Data Science class, a slightly terrifying experience given it’s a ~400 person class, and it being my first big talk on more hands-on programming topics - but I think it went pretty well. The topic was ‘Data Wrangling’ - the largely ‘administrative’ process of getting all your data ‘wrangled’ together into a usable format to do the actual analysis for a project. It’s a really messy process, and takes forever. The actual talk was a largely a tutorial, focused on being a practical guide to wrangling data by providing a crash course on file types, databases and APIs. If you’re at all interested, the Jupyter notebook I used for the talk is publicly available [here](https://github.com/COGS108/DataWrangling), and the talk was actually recorded for the class, and is also publicly available [here](https://podcast.ucsd.edu/podcasts/default.aspx?PodcastId=4122&l=6&v=1) (which I find very weird…).

Since I’m really just a cognitive scientist temporarily masquerading as someone qualified to TA for Data Science, preparing for this talk I started thinking more broadly about the context of Data Wrangling. More specifically, about how we got to this state - what factors led us to current state of how difficult data is to wrangle. This post is basically some quick, assorted, thoughts on that (the ‘cog-sci’ of data wrangling, perhaps). I’m sure they are not original, and they are perhaps more broad and hand-wavey than practical (it’s explicitly not about practical engineering issues such as standards, formats and tools, etc), but here they are:

- *Data is everywhere, but relatively little of it is actually collected as data.* This availability of data is, in some sense, the founding premise of data science, and yet, this is also perhaps the biggest break from academia. Where academia spends an inordinate amount of time and effort collecting data for data’s sake, much of the data in data science is simply a by-product of human activity in the modern world, and thus inherits the messiness of real life activity.

- *Data wrangling is a HCI problem.* Since so much of the data does come from normal interactions, it’s worth considering the difference between human-computer interaction (HCI) and computer-computer interaction. So much potentially useful data (the entire web, anything in a pdf, unstructured text, audio files, etc) is structured as it is for human consumption - but in such a way that computers have a really hard time with it (in terms of automatically aggregating across data and organizing it).

So, what to do?
I mean, I don’t know. Data Science is often ad hoc, pulling data and tools together that were not designed to go together, and we don’t have any universal solutions for collecting, storing and analyzing data. Ultimately, then, many of these problems are probably here to stay, for now at least.

Despite this, some general thoughts:
- Consider the context of the data. How was it generated / collected, and why? In particular, consider the ‘ecological validity’ - the degree to which it’s naturalistic data on human behaviour. I have a hunch that a reasonable heuristic is that data wrangling problems often scale with ecological validity.
- Develop a ‘theory of mind’ for your computer / software. It’s a weird idea, sure, but it’s another hunch that having a sense of recognizing when ‘data’ is in a format optimized for human consumption (as opposed to being in a computer friendly version) will let you eyeball data wrangling issues, and pick data sources strategically. More generally, understanding a bit about how your computer/software ‘thinks’, and what it ‘wants’, will (perhaps) also give you an intuition about what kind of things you need to check and fix in your data.
- TA a huge data science class and hope that by the end of it some of savvy undergrads want to join the lab and do all your data wrangling for you (I’ll get back to you on the efficacy of this one).

Anyways, that’s that. There are surely tons of other relevant point to be made, and very possibly I’m wildly missing the mark, but these were some broader thoughts I thought I’d jot down, since they didn’t make it into the talk in a detailed form. Let me know if you have any thoughts / comments / suggestions / retorts / questions / criticisms / magical skills on offer to wrangle all my data for me.
