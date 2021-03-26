# Discrete-logarithm-problem

Given a large prime number *p*, a large intgeger *a*, and a number *g* such that every number *b* coprime to *p* is congruent to a power of *g mod p* (i.e. g is a primite root mod p), then *g<sup>a</sup> mod p* = *s* is very easy to compute using the repeated squaring algorithm.  However, determining the value of *a* if we are given *g*, *p* and *s* is extremely diffucult, and thus discrete log is considered a one way function.  Several important public-key cryptographic systems base their security on the assumption that the discrete logarithm problem over carefully chosen groups has no efficient solution. These include Diffie-Hellman Key Exchange, ElGamal encryption, and the Digital Signature Algorithm. 

While the discrete log problem is considered cryptographically sound, this repository provides three algorithms that provide significant improvement over a brute-force tactic.  They include the Pohlig-Hellman Algorithm (practically the fastest), the Baby Step Giant Step Algorithm and the Rho Algorithm.

## Syntax is specifice sagemath/python 
## You can use any langauge for your choice for the computation

Fp = GF(p)

## Group order
n = p-1

## Factprisation of group order. Multiply the list element to get the value n

ftr_n = [2 , 1125899907906331 , 1125899907913247 , 1125899907914539 ,1125899907971257 , 1125899907981367 , 1125899907985417 , 1125899908035107 , 1125899908108333 , 1125899908156603 , 1125899908170071 , 1125899908189519 , 1125899908193707 , 1125899908226623 , 1125899908245053 , 1125899908252771 , 1125899908254119 , 1125899908293109 , 1125899908300403 , 1125899908340533 , 1125899908346471 , 1125899908373231 , 1125899908381643 , 1125899908403467 , 1125899908425989 , 1125899908436179 , 1125899908486477 , 1125899908494437 , 1125899908507817 , 1125899908578527 , 1125899908591721 , 1125899908663727 , 1125899908685441 , 1125899908726763 , 1125899908734893 , 1125899908781537 , 1125899908797227 , 1125899908872191 , 1125899908903723 , 1125899908906081 ,1125899908907581]

## Generator of Fp*
g = Fp(2)


## h is 
h = Fp(p-YourRollNumber)

### My roll no = 17025


## Find out log_g(h) = ? 


## Setup
This script requires that [SageMath](https://www.sagemath.org/) be installed to solve the system of linear equations.
