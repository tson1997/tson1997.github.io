# DDPM: Denoising Diffusion Probabilistic Model

Paper link: [link]

Code link: [link]

****
## Introduction

This paper used a very interesting ideas of non-equilibrium thermo-dynamics: We would like to reverse the diffusion process by learning a reverse diffusion function. 

## Problem Formation

Given an image, we will introduce noises over time step so that: each noise would be in Gaussian distribution, and at the end, the distribution of the whole image would be Gaussian. This can be achieve by diffusion process (discuss later).

Our goal is to reverse this process, i.e. to find a reverse function that can convert noise to actual data. If this function is possible to obtain, we can generate data from just random set of Gaussian pixel.


## Methods

1. Diffusion Process

Starting from initial stage x0, we diffuse from x0 using parameter beta, using following formula:

<img src="https://render.githubusercontent.com/render/math?math=x_{k + 1} = \beta_k \epsilon"> + <img src="https://render.githubusercontent.com/render/math?math=\sqrt{1-\beta_k} x_k">

in which epsilon is a random variable that has Standard Normal Distribution.

2. Reverse Diffusion Process

3. Training and Sampling
