# **The Second Eigen Value And Its Applications**
## **'Project Overview'**
This project investigates the second eigenvalue of the Google Matrix and its applications, particularly in detecting link spamming and enhancing PageRank stability. The project is based on the paper "The Second Eigenvalue of the Google Matrix" by Taher H. Haveliwala and Sepandar D. Kamvar. The primary objective is to analytically determine the modulus of the second eigenvalue for the web hyperlink matrix used by Google for computing PageRank.

## Table of Contents

1. [Introduction](#introduction)
2. [Preliminaries and Notations](#preliminaries-and-notations)
3. [Results](#results)
4. [Applications](#applications)
    - [Link Spamming](#link-spamming)
    - [Energy in PageRank](#energy-in-pagerank)
    - [Methods to Boost PageRank](#methods-to-boost-pagerank)
    - [Irreducible Closed Subsets and Link Spamming](#irreducible-closed-subsets-and-link-spamming)
    - [Second Eigenvector and Link Spamming](#second-eigenvector-and-link-spamming)
5. [Algorithms](#algorithms)
    - [Block Power Method](#block-power-method)
    - [Simple Power Method](#simple-power-method)
6. [Work Distribution](#work-distribution)
7. [Appendix](#appendix)
8. [References](#references)

## Introduction

This report analyzes the second eigenvalue of the Google Matrix. Specifically, it proves the following statement:
"For any matrix \( A = [cP + (1 − c)E]^T \), where \( P \) is an \( n × n \) row-stochastic matrix, \( E \) is a non-negative \( n × n \) rank-one row-stochastic matrix, and \( 0 ≤ c ≤ 1 \), the second eigenvalue of \( A \) has modulus \( |λ_2| ≤ c \). Furthermore, if \( P \) has at least two irreducible closed subsets, the second eigenvalue \( λ_2 = c \)."

This has implications for the convergence rate of PageRank, its stability to link structure perturbations, the detection of Google spammers, and the design of algorithms to speed up PageRank.

## Preliminaries and Notations

- \( P \): \( n × n \) row-stochastic matrix.
- \( E \): \( n × n \) rank-one row-stochastic matrix, \( E = ev^T \), where \( e \) is an \( n \)-vector with elements \( e_i = 1 \).
- \( A \): Column-stochastic matrix, \( A = [cP + (1− c)E]^T \).
- \( λ_i \): \( i \)-th eigenvalue of \( A \).
- \( x_i \): Corresponding eigenvector of \( λ_i \).

## Results

### Theorem 1

For \( P \) as an \( n × n \) stochastic matrix and \( c \) such that \( 0 ≤ c ≤ 1 \), with \( E \) a rank-one row-stochastic matrix \( E = ev^T \), the eigenvalue \( |λ_2| ≤ c \).

### Theorem 2

If \( P \) has at least two irreducible closed subsets, then the second eigenvalue \( λ_2 = c \).

## Applications

### Link Spamming

Link spamming manipulates the PageRank algorithm to artificially boost the ranking of websites. This section discusses how the second eigenvalue helps in detecting such manipulative tactics.

### Energy in PageRank

Introduces the concept of energy in PageRank, which relates to the distribution and retention of PageRank within a network of web pages.

### Methods to Boost PageRank

Two methods are described to increase PageRank:
1. **Method 1:** Addition of promotion nodes.
2. **Method 2:** Creation of an irreducible closed subset.

### Irreducible Closed Subsets and Link Spamming

Analyzes the impact of irreducible closed subsets on PageRank and their role in link spamming.

### Second Eigenvector and Link Spamming

Examines how the second eigenvector aids in detecting abnormalities in PageRank caused by link spamming.

## Algorithms

### Block Power Method

Algorithm to compute the second eigenvector using the block power method.

### Simple Power Method

Algorithm to compute the second eigenvector using the simple power method.

## Work Distribution

Details the distribution of work among team members.

## Appendix

Contains supplementary materials and proofs of theorems and lemmas discussed in the report.

## References

List of references used in the project.
