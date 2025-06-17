# Hyperspectral Band Selection

This repository contains code for hyperspectral band selection and evaluation using attention-based neural networks.

## Table of Contents

- [Overview](#overview)
- [Requirements](#requirements)
- [Datasets](#datasets)
- [Usage](#usage)
- [Results](#results)
- [References](#references)

## Overview

This project implements neural network-based band selection for hyperspectral images, with options for both clustering-based and threshold-based selection strategies.

## Requirements

- PyTorch
- scikit-learn
- matplotlib
- ...

## Datasets

The code uses three public hyperspectral datasets. Download them from:

- [Hyperspectral Remote Sensing Scenes (EU)](https://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes)[3]

For example, to use the Pavia University dataset:
- Data: `datasets/PaviaU.mat`
- Ground Truth: `datasets/PaviaU_gt.mat`

Place the downloaded `.mat` files in the `datasets/` directory.

## Usage

To train and evaluate the band selection model, run:

python main.py --mode band_selection --dataset pavia

Replace arguments as needed for your use case.

## Results

Results will be printed to the console and saved as figures in the project directory.
Visualisations:
  - Confusion matrix
  - TSNE graph

## References
- https://ieeexplore.ieee.org/document/9511339
- https://ieeexplore.ieee.org/document/9737043
- https://ieeexplore.ieee.org/document/10290100
