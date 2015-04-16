title: "Frontend third-party extension management with Bower and javascript modules"
date: 2015-04-15 13:13:24
tags:
---

Writing huge web application requires an intuitive workflow and a solid architecture. Designing a well formed bottom application layer that allows contributors to collaborate with ease, whether they are working inside the same pool or if they are working independantly, can be tricky.

This article will present a way to provide a robust base layer, using the combination of the reference frontend package manager (Bower) and Javascript modules.


This guide is not intended to expose "the perfect way" to solve the problem, it is more a combination of all my thoughts on the problem, after having experienced by myself the need of such a system, and my conclusion after an analysis on how people tend to solve contribution problems in such cases.

The need
========

Writing a big javascript frontend app involves contributions from several developpers that works in the same time on different aspects of the application. Specifications can be quite complex to establish when kickstarting a project, but most of the time, allowing aware integrators to plug in third-party extensions is not a bad idea :

- Extensions can be installed, providing new features to the final user, or disabled, making the application lighter, and completely removing features, without breaking the frontend mecanics
- Installing or upgrading a third party extension does not always (and actually, should not) require a full upgrade of the core of the application.
- Version numbers can be different amongst provided extensions, allowing the flexibility to upgrade or downgrade extensions up to a major and breaking change on the system


Modules loaders to your rescue !
================================

Javascript modules concepts are more and more used speaking about code organisation. Organizing your code in javascript modules helps to correctly manage dependancies, and prevent 


Downsides
=========

- Minification policies

