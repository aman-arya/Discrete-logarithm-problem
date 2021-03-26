# Discrete-logarithm-problem

Given a large prime number *p*, a large intgeger *a*, and a number *g* such that every number *b* coprime to *p* is congruent to a power of *g mod p* (i.e. g is a primite root mod p), then *g<sup>a</sup> mod p* = *s* is very easy to compute using the repeated squaring algorithm.  However, determining the value of *a* if we are given *g*, *p* and *s* is extremely diffucult, and thus discrete log is considered a one way function.  Several important public-key cryptographic systems base their security on the assumption that the discrete logarithm problem over carefully chosen groups has no efficient solution. These include Diffie-Hellman Key Exchange, ElGamal encryption, and the Digital Signature Algorithm. 

While the discrete log problem is considered cryptographically sound, this repository provides three algorithms that provide significant improvement over a brute-force tactic.  They include the Pohlig-Hellman Algorithm (practically the fastest), the Baby Step Giant Step Algorithm and the Rho Algorithm.


## Setup
This script requires that [SageMath](https://www.sagemath.org/) be installed to solve the system of linear equations. The `primefac` module is also required and can be installed with `pip install -r ./requirements.txt`
