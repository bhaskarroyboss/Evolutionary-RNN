# Evolutionary RNN
[![DOI](https://zenodo.org/badge/1315991560.svg)](https://doi.org/10.5281/zenodo.21675360)
> **An experimental hybrid recurrent neural network that allows individual neurons to adaptively evolve between Backpropagation and Contrastive Hebbian Learning.**

Developed by **Bhaskar Roy** as part of the **Neuromatch Academy NeuroAI Project**.

---

## Overview

Evolutionary RNN is an experimental research framework that investigates whether neurons should use a single global learning algorithm or independently adapt their learning strategy throughout training.

Instead of relying exclusively on Backpropagation (BP), every neuron dynamically balances between **Backpropagation (BP)** and **Contrastive Hebbian Learning (CHL)** using an evolutionary preference mechanism. During training, neurons evaluate the effectiveness of each learning rule, compete based on performance, and gradually specialize through local neighborhood interactions.

The goal is to explore biologically inspired adaptive learning mechanisms for sequential learning tasks.

---

## Features

- 🧠 Neuron-level adaptive learning rule selection
- ⚡ Hybrid Backpropagation + Contrastive Hebbian Learning
- 🧬 Evolutionary preference optimization
- 🌐 Neighborhood-driven learning dynamics
- 📈 Sequential MNIST evaluation
- 🔬 PyTorch implementation
- 📊 Training and evolutionary visualizations

---

## Experimental Setup

**Dataset**

- Sequential MNIST

**Tasks**

- Normal
- Affine
- Elastic
- Perspective
- Gaussian Blur
- Random Erasing
- Random Transform
- Mixed Augmentation

**Framework**

- PyTorch

---

## Preliminary Observations

Across eight sequential MNIST tasks, the adaptive framework exhibited different dominant learning strategies depending on the input perturbation.

| Task | Dominant Learning Rule |
|-------|------------------------|
| Normal | Backpropagation |
| Affine | Backpropagation |
| Elastic | Backpropagation |
| Perspective | Backpropagation |
| Blur | Contrastive Hebbian Learning |
| Random Erasing | Contrastive Hebbian Learning |
| Random Transform | Backpropagation |
| Mixed | Contrastive Hebbian Learning |

These observations suggest that different learning rules may be better suited to different data distributions, supporting further investigation into adaptive neuron-level optimization.

---

## Repository

```
Evolutionary-RNN/
│
├── Evolutionary_RNN.ipynb
├── README.md
├── LICENSE
```

---

## Project Status

⚠️ This repository contains an active research prototype.

The implementation is under continuous development as part of an ongoing investigation into biologically inspired learning algorithms. Experimental results, documentation, and benchmarks will continue to evolve.

---


## Citation

If you use this repository in your research, please cite this repository.

A Zenodo DOI and formal citation will be added upon the first stable release.

---

## Acknowledgements

This work was developed during participation in the **Neuromatch Academy NeuroAI Project**.

The implementation, experiments, and analyses presented in this repository represent the independent research work of the author.

---

## Author

**Bhaskar Roy**

GitHub: https://github.com/bhaskarroyboss

---

## License

Licensed under the Apache License 2.0.
