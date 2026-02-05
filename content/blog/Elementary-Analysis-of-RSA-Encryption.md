---
author: Nihar Maheshwari
title: "Elementary Analysis of RSA Encryption"
date: 2026-02-05T18:50:30+05:30
draft: false
topics:
- Cryptography
- Cryptanalysis
- Number Theory
---
> This post aims to present an elementary (but rigorous) exposition on the RSA collection of functions and its relationship to the factorization problem. 

# Setup

RSA, named after its inventors Rivest, Shamir, Adleman, at its core, is simply a collection of functions (i.e, a family of number theoretic one-way functions indexed by a certain parameter). It is conjectured to be not only strongly one-way but also non-uniformly strongly one way.


>**Strongly One Way Functions:** A function $f(x)$ is strongly one way iff $\exists\, p(n) \in \mathcal{P}$ such that $f(x)$ is $\mathcal{O}(p(n))$ and 
$$\forall A \in \text{PPT}\,\, Pr\bigg[A[f(x)]=x'\,| f(x')=f(x)\bigg]<\frac{1}{p(n)}\,\,\,\forall p(n)\in \mathcal{P}, \forall n\geq N, N\in\mathbb{N}$$

where A is a probabilistic time algorithm (PPT) adversary and $n=\lceil\log_2 x \rceil$ is the number of bits required to express $x$. 

>**Non-uniformly Strongly One Way Functions:** A function $f(x)$ is non-uniformly strongly one way iff $\exists p(n) \in P$ such that $f(x)$ is $\mathcal{O}(p(n))$ and 
$$\forall \{C_n\}_{n\in\mathbb{N}} Pr\bigg[C_n[f(x)]=x'\,|f(x')=f(x) \bigg]<\frac{1}{p(n)}\,\,\, \forall p(n)\in \mathcal{P}, \forall n\geq N, N\in\mathbb{N}$$ 

where $\{C_n\}_{n\in\mathbb{N}}$ is a circuit. A circuit, in elementary terms, is effectively a collection of probabilistic and deterministic algorithms where an algorithm with desired behaviour is chosen on the basis of input size. A circuit is much more powerful than a single PPT adversary.
# Constructing RSA

# Inverting RSA 

## Polynomial-Time Reduction 

## Inverting RSA $\leq_P$ Factorization 
