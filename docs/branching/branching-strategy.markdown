---
layout: page
title: Branching Strategy
nav_order: 2
permalink: /branching/branching-strategy/
parent: Branching Strategy
color_scheme: dark
---
# Git Flow
Gitflow is a branching model and workflow for Git, which is a popular version control system used in software development. Gitflow is designed to provide a structure for managing and organizing Git repositories, particularly for projects with multiple developers and complex release cycles.

## The Gitflow workflow consists of two main branches:

`Master/Main branch`: This branch represents the official release history of the project, and it contains only production-ready code.

`Develop branch`: This branch represents the ongoing development of the project, and it contains the latest code that is not yet ready for release.

### In addition to the main branches, Gitflow also includes several supporting branches:

`Feature branches`: These branches are used to develop new features, and they are based on the develop branch. Once a feature is complete, it is merged back into the develop branch.

![Feature Branching](/assets/images/feature-branching-small.svg){:class="img-responsive"}

`Release branches`: These branches are used to prepare the code for release, and they are based on the develop branch. Once a release is ready, it is merged into both the master and develop branches.

![Release Branching](/assets/images/release-branching.svg){:class="img-responsive"}

`Hotfix branches`: These branches are used to fix critical issues in the production code, and they are based on the master branch. Once a hotfix is complete, it is merged into both the master and develop branches.

![Hotfix Branches](/assets/images/hotfixes.svg){:class="img-responsive"}

`QA branches`: These branches are used to deploy single or combined feature sets for testing into a QA environment. Ideally one feature would be tested at a time but due to hardware constraints this branch allows for multiple in development features to be released into a single environment. These branches are intended for testing only and ***code will not be merged from this branch***.

![QA Branches](/assets/images/qa-branching.svg){:class="img-responsive"}

By using the Gitflow model, developers can work on new features and bug fixes in a structured and organized way, without disrupting the main development and release cycles. Gitflow also provides a clear separation between stable production code and ongoing development, making it easier to manage releases and deploy updates.

