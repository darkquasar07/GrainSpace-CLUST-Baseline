# GrainSpace CLUST Baseline

This repository provides a baseline implementation of the **CLUST** method for unsupervised domain adaptation on the **GrainSpace** dataset.

## References

**Original GrainSpace repository:** [hellodfan/GrainSpace](https://github.com/hellodfan/GrainSpace)

**CLUST paper:** [Prototype-oriented class-conditional clustering transport for unsupervised domain adaptation](https://doi.org/10.1038/s41598-025-21560-y)

## Overview

The objective of this work is to evaluate a recent unsupervised domain adaptation method on GrainSpace wheat-domain transfer tasks. The baseline follows the CLUST framework, which combines:

- source-supervised training
- prototype-based pseudo-labeling
- class-conditional feature clustering transport
- prototype clustering transport
- prediction consistency regularization
- information maximization

The current experiments focus on wheat-only domain adaptation tasks, for example:

- `WHEAT_R1-14_M600 -> WHEAT_R15-18_M600`

## Dataset

This project uses the **GrainSpace** dataset. Dataset access, licensing, and original benchmark details are available in the official repository:

[https://github.com/hellodfan/GrainSpace](https://github.com/hellodfan/GrainSpace)

The dataset is **not redistributed** in this repository.

Expected folder structure:

```text
GrainSpace_Dataset/
├── Train/
│   ├── WHEAT_R1-14_M600_TRAIN/
│   ├── WHEAT_R15-18_M600_TRAIN/
│   └── WHEAT_R19-22_M600_TRAIN/
├── Validation/
│   ├── WHEAT_R1-14_M600_VAL/
│   ├── WHEAT_R15-18_M600_VAL/
│   └── WHEAT_R19-22_M600_VAL/
└── Test/
    ├── WHEAT_R1-14_M600_TEST/
    ├── WHEAT_R15-18_M600_TEST/
    └── WHEAT_R19-22_M600_TEST/
