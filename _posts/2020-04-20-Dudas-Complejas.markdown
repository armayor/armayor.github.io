---
layout: post
title:  "Dudas Estadísticas"
date:   2020-04-20 18:55:14 +0200
categories: Statistical Mechanics
mathjax: true
comments: true
---
$$\newcommand{\ket}[1]{\vert#1\rangle}$$
$$\newcommand{\bra}[1]{\langle#1\vert}$$
$$\newcommand{\braket}[2]{\langle#1\vert#2\rangle}$$
$$\newcommand{\mvop}[3]{\langle#1\vert#2\vert #3\rangle}$$

**Definitions of phase space**

We denote by $$\Gamma(E)$$ the volume of the phase space between energies $$E$$ and $$E+\Delta$$, that is

$$\Gamma(E)=\int_{E\leq H(\pmb{q},\pmb{p})\leq E+\Delta} \textrm{d}\pmb{q}\,\textrm{d}\pmb{p}$$

If $$\Delta$$ is sufficiently small we may rewrite the integral above using Dirac's Delta function

$$\Gamma(E)=\Delta\underbrace{\int \textrm{d}\pmb{q}\,\textrm{d}\pmb{p}\,\delta(H(\pmb{q},\pmb{p})-E)}_{\omega(E)}$$

We denote by $$\Sigma(E)$$ the volume of the phase space below energy $$E$$:

$$\Sigma(E)=\int_{H(\pmb{q},\pmb{p})\leq E} \textrm{d}\pmb{q}\,\textrm{d}\pmb{p}$$

Again, if Delta is sufficiently small

$$\dfrac{\Gamma(E)}{\Delta}=\dfrac{\Sigma(E+\Delta)-\Sigma(E)}{\Delta}\rightarrow\dfrac{\partial\Sigma}{\partial E}$$

and thus $$\Gamma(E)=\Delta\dfrac{\partial\Sigma}{\partial E}$$. We will show $$\dfrac{\partial\Sigma}{\partial E}=\omega(E)$$:

$$\Gamma(E)=\Delta\dfrac{\partial\Sigma}{\partial E}=\Delta\dfrac{\partial}{\partial E}\int_{H(\pmb{q},\pmb{p})\leq E}\textrm{d}\pmb{q}\,\textrm{d}\pmb{p}=$$

$$=\Delta\dfrac{\partial}{\partial E}\int \textrm{d}\pmb{q}\,\textrm{d}\pmb{p}\, \theta(E-H)=\Delta\int \textrm{d}\pmb{q}\,\textrm{d}\pmb{p}\, \dfrac{\partial}{\partial E}\,\theta(E-H)=\Delta\int\textrm{d}\pmb{q}\,\textrm{d}\pmb{p}\,\delta(H(\pmb{q},\pmb{p})-E)$$

where $$\theta(\cdot)$$ is Heaviside's step function and $\dfrac{d}{dx}\theta(x)=\delta(x)$ is an equality of distributions.

Note units are correct for volume but we need dimensionless "volume".

**Definition of entropy**

Motivation. Suppose we have A system of volume $$V$$, temperature $$T$$ and $$N$$ particles. there are many number of ways in which this system can exist. Consider the complessive system subdivided in two. For each way subsystem 1 exists, there are $$W_2$$ ways in which system 2 may exist. Hence, if $$W_1$$ denotes the number of microstates for subsystem 1, there are in total $$W_1W_2$$ ways.

Entropy is aditive and hence $$S(W_1W_2)=S(W_1)+S(W_2$$), so we look for a function of the form $$S(W)=C\,\log(W)$$.


Right now take $$S=k_B\log\Gamma(E)$$ as the definition. However adjustments are to be made since what is to count are the number of microstates and $$\Gamma(E)$$ represents a volume. Note that according to Heisenberg's uncertainty principle $$\Delta q\Delta p\geq\dfrac{\hbar}{2}$$. For simplicity, in $d$ dimensions and for $N$ particles, we take the smallest possible "box" in phase space to be of size $$h^{dN}$$. Hence the number of microstates is the volume divided by the size of each box, so

$$\Gamma(E)=\dfrac{\Delta}{h^{dN}}\int\textrm{d}\pmb{q}\,\textrm{d}\pmb{p}\,\delta(H(\pmb{q},\pmb{p})-E)$$

Now it makes perfect sense to use the given definition of entropy.