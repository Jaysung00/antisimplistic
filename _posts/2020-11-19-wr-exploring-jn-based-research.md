---
toc: true
layout: post
description: "A collection of links describing tools and methods that support nb-based research and publishing workflows with good software engineering practices."
categories: [worthreading, jupyter]
title: "Exploring Jupyter Notebook-Based Research"
image: images/jupyternb.png
comments: true
---

Much of my life has been centered around software. In middle school I was writing [vertical blank interrupts in assembly language for the 6502 in my Atari 800](https://playermissile.com/dli_tutorial/). In 1994 I co-founded the first of two software development companies that I've run ever since. Despite all that, I've never considered myself a "software guy." The traditional pattern of write code, compile, check is... well, hard. And discouraging. I have tremendous respect for folks that have mastered this, and consider myself very fortunate to have employed many great, and a few truly exceptional software engineers.

But for me, there had to be a better way. Upon returning to graduate school for Dan 2.0, I found it. Python and Jupyter Notebooks (JNs). The combination of Python's interpreted nature and the way that JNs combine code, output, and text provided an approach that was much more natural and welcoming to me. Over time, it allowed me to build enough skill and confidence "hacking away" at data science projects to begin exploring software engineering and carpentry.

To that end, I've recently spent a lot of time reading about workflows built around notebooks, especially those that facilitate good software engineering practices, single-source publishing, integration, and deployment. Below I've shared some of the most insightful links I encountered in that search, along with short summaries and relevant background information. As my PhD focus transitions from classes to research, my goal is to leverage some of these methods to improve the efficiency, quality, and reproducibility of my work while making it easier to publish in a variety of ways.

- [**nbdev: use Jupyter Notebooks for everything**](https://www.fast.ai/2019/12/02/nbdev/): this article first opened my eyes to very interesting things going on in the JN ecosystem, leading to many of the articles linked below. nbdev is a "highly opinionated" Python programming environment that supports software engineering best practices (automated documentation, package creation, testing, continuous integration, source control, and more) for JNs. [nbdev](https://nbdev.fast.ai) was created by [the team](https://www.fast.ai/about/) that created the deep learning PyTorch front-end [fastai](https://docs.fast.ai) and the JN-based blogging tool [fastpages](https://github.com/fastai/fastpages), which this page is built with. Not at all coincidentally, fastpages is powered, at least in part, by nbdev. All of this was developed by the article's author [Jeremy Howard](https://twitter.com/jeremyphoward), former President and Chief Data Scientist of [Kaggle](https://www.kaggle.com), and [Sylvain Gugger](https://twitter.com/GuggerSylvain), now at [Hugging Face](https://huggingface.co). Together, they co-authored [_Deep Learning for Coders with Fastai and PyTorch: AI Applications Without a PhD_](https://amzn.to/3p3MpIJ). I am working with nbdev and will share my experience in future updates.
- [**How to use Jupyter Notebooks in 2020**](https://ljvmiranda921.github.io/notebook/2020/03/06/jupyter-notebooks-in-2020/): the first of an insightful three-part series on the JN ecosystem. In it, author [Lj Miranda](https://twitter.com/ljvmiranda921) covers the evolution of methods of practice in the data science landscape, current tools and best practices for notebook-based development workflows, and thoughts on the future. I found the second part particularly useful, with lots of technical detail.
- [**Beyond Interactive: Notebook Innovation at Netflix**](https://netflixtechblog.com/notebook-innovation-591ee3221233): continuing with the JN theme, this article discusses how "notebooks are the most popular tool for working with data" at Netflix. It describes the workflow, including scheduled runs of parameterized notebooks and collecting code and output into notebooks to create a record of various jobs. It also describes the extensive infrastructure required to support this at scale. At the time of its writing in 2018, the authors were planning to run more than 150,000 notebook-based jobs per day. This is the first of a two-part series. The second, [Scheduling Notebooks at Netflix](https://netflixtechblog.com/scheduling-notebooks-348e6c14cfd6), dives more deeply into the details. Note that two of the original authors, [Matthew Seal](https://twitter.com/codeseal) and [Michelle Ufford](https://twitter.com/MichelleUfford) have since left Netflix to found [noteable.io](https://noteable.io), a "SaaS offering for integrated Jupyter Notebooks."
- [**How to share Jupyter Notebooks**](https://zonca.dev/2020/09/how-to-share-jupyter-notebooks.html): complements the previous article by providing more ways to share JNs including gist, nbviewer, and binder. By [Andrea Zonca](https://twitter.com/andreazonca)
- [**Presenting Code Using Jupyter Notebook Slides**](https://medium.com/@mjspeck/presenting-code-using-jupyter-notebook-slides-a8a3c3b59d67): I was today years old when I learned that the ability to run slide-based presentations was built into JNs! A very short tutorial on how to do it by [Matthew Speck](https://twitter.com/mjspeck).

My focus above is on Jupyter Notebooks, but there are lots of cool things going on in the RStudio world as well, especially related single-source, "one-click" publishing. Many great web-books about/using R have been published from R Notebooks using [R markdown](https://rmarkdown.rstudio.com) and [bookdown](https://bookdown.org), including [Hadley Wickham's](https://twitter.com/hadleywickham) classic [R for Data Science](https://amzn.to/2IHlRgd). A list of other examples can be found on [the bookdown archive page](https://bookdown.org/home/archive/).

Here are a few relevant and timely R-related links:

- [**RStudio 1.4 Preview: Citations**](https://blog.rstudio.com/2020/11/09/rstudio-1-4-preview-citations/): a close look at the deep support for citations included in the upcoming [RStudio](https://twitter.com/rstudio) v1.4, currently [available as a preview release](https://www.rstudio.com/products/rstudio/download/preview/). Other features in the update include improved support for Python and a [visual markdown editor](https://www.rstudio.com/products/rstudio/download/preview/).
- [**Single-source publishing for R users**](https://masalmon.eu/2020/11/06/single-source-publishing-r/): describes a typical process for generating html- and pdf-based books from R Markdown using bookdown and ways to simplify and automate the process. I don't pretend to understand everything going on here, but know enough to appreciate the author, [Maëlle Salmon's](https://twitter.com/ma_salmon) work enough to share and bookmark it!