# Bayesian modelling for bioprocesses

Hands-on notebook for the lecture *Bayesian modelling for bioprocesses* in the course **AI Fundamentals for Biotechnology** (Delft, 27 November 2026).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lhelleckes/bayesian-modelling-delft/blob/main/bayesian_modelling_bioprocesses.ipynb)

## 📁 Contents

[`bayesian_modelling_bioprocesses.ipynb`](bayesian_modelling_bioprocesses.ipynb) has three parts that follow the slides:

| Part | What you will do |
|---|---|
| 🧪 **1. Fully mechanistic model** | Fit first-order kinetics $P(t) = S_0 (1-e^{-kt})$ to four enzymes with [PyMC](https://www.pymc.io) |
| 📏 **2. Calibration models** | Turn calibration data into a likelihood with [calibr8](https://github.com/JuBiotech/calibr8) and combine it with a linear process model |
| 🧠 **3. Hybrid model** | Learn how the rate constant depends on temperature and pH with a Gaussian process |

All data are simulated inside the notebook, so nothing needs to be downloaded.

## 🚀 Running the notebook

The easiest way is Google Colab: click the badge above, then *Runtime → Run all* (about 3 minutes).

To run it locally instead:

```bash
conda create -c conda-forge -n pymc_env "pymc>=5"
conda activate pymc_env
pip install calibr8 jupyter
```

## 📚 Further reading

Helleckes, L.M., Osthege, M., Wiechert, W., von Lieres, E., & Oldiges, M. "Bayesian calibration, process modeling and uncertainty quantification in biotechnology." *PLoS Computational Biology* 18(3): e1009223 (2022). [doi:10.1371/journal.pcbi.1009223](https://doi.org/10.1371/journal.pcbi.1009223)
