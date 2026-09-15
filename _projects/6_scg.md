---
layout: page
title: Scaled conjugate gradient methods for deep learning optimisation
description: A dynamic scaling factor inside the conjugate-gradient update, benchmarked against Adam and AdaBelief.
importance: 2
category: coursework projects
---

**National University of Singapore · 2025**

**Study context.** The team studied a hybrid optimiser that introduces a dynamic scaling factor into the conjugate-gradient update rule, with convergence rates argued at O(1/N) under a constant step size and O(1/√N) under a decaying one, benchmarked against SGD, Adam and AdaBelief on CIFAR-10, CIFAR-100 and IMDb classification.

**My contribution.** I wrote the discussion and possible-extensions analysis: which assumptions in the convergence argument constrain the method's applicability to non-convex settings, and which extensions are worth pursuing. The derivation and the empirical work were carried out by other team members.
