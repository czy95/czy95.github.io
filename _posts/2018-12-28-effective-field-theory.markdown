---
layout: post
title: Effective field theory
date:  2018-12-28 22:34:44 +0800
categories: [Physics]
comments: true
mathjax: true
---

**Contents**
* TOC
{:toc}
My struggle to catch up with physics as I transfer too much time in learning non relevant things.

## Fermi's four fermions theory of Weak interaction.
Processes at energies far below the W mass, such as β-decay

[Fermion rules for four fermions theory ](https://physics.stackexchange.com/questions/363654/feynman-rules-for-four-fermions-theory)

$$
\mathcal { L } = \overline { \psi } \left( i \partial _ { \mu } \gamma ^ { \mu } - m \right) \psi + G ( \overline { \psi } \psi ) ^ { 2 }
$$

> This theory is used as an effective theory of Yukawa lagrangian when the energies are much lower than the mass of the scalar propagator.

![](https://i.stack.imgur.com/Z8Ld6.png)

$$
i \mathcal { M } = i G \left[ \overline { \nu } \left( p _ { 1 } \right) u \left( p _ { 2 } \right) \overline { u } \left( p _ { 2 } ^ { \prime } \right) v \left( p _ { 1 } ^ { \prime } \right) \right]
$$

This amplitude can be reproduced to lowest order in $q ^ { 2 } / M _ { W } ^ { 2 }$ by a low energy EFT with a contact interaction
## Dimensional analysis
We use the condition that **action is dimensionless**. Why?

### [Why is the action dimensionless in natural units?](https://physics.stackexchange.com/questions/224232/why-is-the-action-dimensionless-in-natural-units)

It is dimensionless in the sense of *mass dimension*.

Setting $\hbar = c = 1$ means we only need to fix one base unit, which is usually taken to be the energy measured in $\mathrm{eV}$. Now, since $c=1$, this means that because of $E=mc^2$ becoming $E=m$ both $E$ and $m$ are measured in $\mathrm{eV}$. They might represent different *dimensions* (mass and energy), but they are measured in the same *unit*. Now, $E=h\nu$ means that inverse time is measured in $\mathrm{eV}$, so time is measured in $\mathrm{eV^{-1}}$. And so on.

Now, the "mass dimension" of a quantity is simply the power of $\mathrm{eV}$ it is measured in. Since the action is the integral of an energy against time, it has units of $\mathrm{eV}\cdot\mathrm{eV}^{-1} = \mathrm{eV}^0$, i.e. it has mass dimension zero.

You are right in that it is not "dimensionless". But having mass dimension zero means for any quantity $Q$ that there are powers of $\hbar$ and $c$ such that $\frac{Q}{\hbar^n c^m}$ *is* dimensionless, and since $\hbar = c = 1$, $\frac{Q}{\hbar^n c^m} = Q$, so there is no numerical difference between those quantities, and one sloppily says that $Q$ is dimensionless.

If you are somewhat worried that $\frac{Q}{\hbar^n c^m} = Q$ "looks wrong" from a dimensional analysis standpoint, then yes, that's right - the convenience in the formulae we get from $\hbar = c = 1$ comes inevitably  with the loss of a large part of dimensional analysis, all that is left is the mass dimension for that.

### <span style="color:#00bfff">Why the sky is blue?</span>
Another top-down application of EFT is to answer the question of <span style="color:#00bfff">why the sky is blue.</span> More precisely, why low energy light scattering from neutral atoms in their ground state is much stronger for blue light than red.

## Lagrangian for relativistic scalar field with a $\phi \rightarrow - \phi$ symmetry

$$
\mathcal { L } _ { E } = \frac { 1 } { 2 } ( \partial \phi ) ^ { 2 } + \frac { 1 } { 2 } m ^ { 2 } \phi ^ { 2 } + \frac { \lambda } { 4 ! } \phi ^ { 4 } + \sum _ { n = 1 } ^ { \infty } \left( \frac { c _ { n } } { \Lambda ^ { 2 n } } \phi ^ { 4 + 2 n } + \frac { d _ { n } } { \Lambda ^ { 2 n } } ( \partial \phi ) ^ { 2 } \phi ^ { 2 n } + \ldots \right)
$$

By doing dimensional analysis, it's not hard to get
$$
[ \phi ] = 1
$$

That means that the operator $[ \phi ]^6$ is dimension 6, and the contribution to the action has dimension 2, and so its coupling constant must have dimension −2, or $1/ \operatorname { mass } ^ { 2 }$. The operator $\phi ^ { 2 } \left( \partial ^ { 2 } \phi \right) ^ { 2 }$ is dimension 8 and must have a coefficient which is dimension −4, or  $1/ \operatorname { mass } ^ { 4 }$.

## References
* Howard Georgi review of effective field theory.
