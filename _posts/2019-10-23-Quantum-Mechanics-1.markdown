---
layout: post
title:  "Quantum Mechanics I: Foundations"
date:   2019-10-19 18:55:14 +0200
categories: QM
mathjax: true
comments: true
---
$$\newcommand{\ket}[1]{\vert#1\rangle}$$
$$\newcommand{\bra}[1]{\langle#1\vert}$$
$$\newcommand{\braket}[2]{\langle#1\vert#2\rangle}$$
$$\newcommand{\mvop}[3]{\langle#1\vert#2\vert #3\rangle}$$

## Purpose of this post

My aim is to explain in detail how to construct the basics of Quantum Mechanics.

## 1. Commutators
## 2. Postulates

Firstly we will formulate the postulates using the less mathematical terms possible in order to clarify the subyacent ideas and make the math behind them follow naturally afterwards.

**Postulate I:** Physical states are represented by vectors (i.e. $$\ket{A}$$) in a Hilbert Space. 

We might wonder shat mystic properties can such a Hilbert Space have in order to become the primary foundation for out theory. Where does the necessity of using this mathematical consruction come from?

Firstly, since a Hilbert Space is in particular a vector space, if a system can be in two states $$\ket{A}$$ and $$\ket{B}$$, the state defined as $$\ket{C}:=\ket{A}+\ket{B}$$ is also a possible state of the system.

**Postulate II:** Two vectors correspond to the same physical state if they differ in a phase or constant (i.e. if $$\ket{A}=c\ket{B}$$ where $$c\in \mathbb{C}$$).

**Postulate III:** If an observable $$\Omega$$ is measured on a system and the result of the measurement is $$\omega$$, then inmediately after we measure, the system is in a state in which, if measure is to be repeated again, it would yield the value $$\omega$$.

This means that initially we may have our system in a state $$\ket{A}$$. We want to measure some physical magnitude we have previously called $$\Omega$$ (it could be the energy, the momentum, etc.). We measure and we get a value $\omega$. Upon measuring there is no reason to think that if we are to repeat the measurement we will get the same value $\omega$. This third postulate just states that, somehow, we will always get the same value. Thus, we will no longer say our system is in the state $$\ket{A}$$ but on a state we shall denote by $$\ket{\omega}$$. There could possibly be other states $$\ket{\omega'}$$ which would also yield the value $$\omega$$. Let us consider the set 

$$\mathcal{S}(\omega):=\{\ket{\omega_i}\,:\, \textrm{if } \Omega \textrm{ is measured it always yields the value } \omega\}$$

We might ask then what happens if upon measurement of $$\Omega$$ and getting a value $$\omega$$ the set $$\mathcal{S}(\omega)$$ has more than one element. Does the system collapse after measurement to a definte state $$\ket{\omega_{i_0}}$$ or can it, however be ranging among any of the $$\ket{\omega_i}$$'s.

**Postulate IV** The probability that upon measuring a system on the state $$\ket{A}$$ we get the value $$\omega$$ is defined as:

$$ P(\textrm{measure } \omega \textrm{ on } \ket{A})=\sum_i\dfrac{\vert\braket{\omega_i}{A}\vert^2}{\braket{\omega_i}{\omega_i}\braket{A}{A}}$$

Note that in case $$\vert\mathcal{S}(\omega)\vert=1$$ the sum on $i$ vanishes. However, I find it makes more sense to write it that way since if we are measuring a magnitude $$\Omega$$ and there are different mutually exclusive circumstances (states $$\ket{\omega_i}$$) which lead to same value $$\omega$$ it makes sense to add the probabilities of finding the system on each state $$\ket{\omega_i}$$.

## 3. Operators $$p$$ and $$q$$
## 4. Non-importance of operator choice
## 5. Schrödinger Equation
## 6. Summary

| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |

Rendered table with varied cell width