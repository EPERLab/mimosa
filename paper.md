---
title: 'mimosa: A Modern Graphical User Interface for 2-level Mixed Models'
tags:
  - mixed models
  - hierarchical linear models
  - shiny
  - R
authors:
  - name: Johannes Titz
    orcid: 0000-0002-1102-5719
    affiliation: 1
affiliations:
 - name: Department of Psychology, TU Chemnitz, Germany
   index: 1
date: 04 February 2020
bibliography: library.bib
---

# Summary
The mixed models special agent (``mimosa``) is a ``shiny`` [@chang2019] app for 2-level mixed models. Mixed models are rapidly becoming the gold standard of statistical analysis techniques in the behavioral sciences. Yet there is only a small number of user-friendly programs for conducting mixed model analyses. The most common tools often lack a graphical user interface, are proprietary, and involve a tedious process of getting data in and publication-ready tables out. An exception is the shiny app ``mimosa`` which offers an alternative that is free, open source, intuitive, and runs in a browser, making it easily accessible (see https://www.mimosa.icu).

The software is targeted at behavioral scientists who frequently use 2-level mixed models and want a solution that is tailored for this particular use case. For instance, researchers studying groups (e.g. students clustered in schools, individuals clustered in work groups) and researchers employing within-subjects designs almost exclusively analyze their data with 2-level mixed models. Unlike other software, ``mimosa`` was designed for this use case. It helps the analyst by automatically detecting potential grouping variables and categorizing these variables in level 1 and level 2. Furthermore, ``mimosa`` is researcher-oriented because it produces a single summary table via ``sjPlot`` [@ludecke2018] that can be published in a scientific journal without any modifications.

To my knowledge, there are only a couple of free, open source, software packages for mixed models that have a graphical user interface. For a slightly outdated comparison of different mixed model software (including proprietary and command-line software) see @west2012. ``LMMgui`` focuses on within-subjects-designs and as such can be seen as a direct competitor of ``mimosa``. ``LMMgui`` offers diagnostic plots and can compare two models, which is missing in ``mimosa``. The disadvantage of ``LMMgui`` is that it is only available for Windows, while ``mimosa`` runs on any platform because it is a browser application. Furthermore, ``mimosa`` has a cleaner interface, is easier to use, and produces a publication-ready output.

The ``GAMLj`` [@gallucci2020] module for ``jamovi`` [@thejamoviproject2019] is a more comprehensive tool for mixed model analysis. It is possible to model more than two levels and specify more complex models in general. ``GAMLj``'s functionality is close to the command line interface of ``lme4`` [@bates2015]. This is a clear benefit, but it also comes with a downside: ``GAMLj``'s interface is less clean than ``mimosa``'s. ``GAMLj`` has many dialogues and the specification of a model is not as intuitive as in ``mimosa``. Still, ``GAMLj`` is an almost perfect software for mixed models in general. On the other hand, ``mimosa`` follows the idea of doing one type of analysis well, which is the one that many behavioral researchers do most of the time: 2-level mixed models.

In contrast to the software packages I am aware of (including the ones discussed by @west2012), ``mimosa`` is the only one that runs in a browser. While this might be seen as a trivial advantage, it has clear benefits. There is no need to install or update ``mimosa`` or its dependencies, and the application can be used at any place with an internet connection---for instance, at the office of a colleague who does not have ``jamovi`` and ``GAMLj`` installed, in the classroom, or at a conference presentation for a live analysis.

# Acknowledgments
I want to sincerely thank Maria Reichert for writing a first scaffold for ``mimosa``. Further, I want to thank Markus Burkhardt, Karin Matko, Thomas Schäfer, Peter Sedlmeier, and Isabell Winkler for testing ``mimosa`` and giving helpful comments on the documentation.

# References
