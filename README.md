# Cosyne Tutorial 2022

These are the exercises for the [COSYNE](https://www.cosyne.org/) 2022 Tutorial, _Spiking Neural Network Models in Neuroscience_, by Dan Goodman.

The exercises are in Python, in the Jupyter Notebook format.
You can run these notebooks either locally, or in the cloud (via Google Colab or Kaggle). 
We recommend following the installation instructions for running locally
(found [below](#run-locally-)) before the conference: the on-site
Wi-Fi might be flaky and not able to handle all participants simultaneously.



## Run in the cloud ☁

If you have a Google account, launch with Colab.
If you are in a country that blocks Google, such as China, you can try
using Kaggle instead. [Some instructions from Neuromatch Academy are here.](https://deeplearning.neuromatch.io/tutorials/TechnicalHelp/Tutorial_kaggle.html)

### Part 1 – "Classical" spiking neural networks

* Leaky integrate-and-fire neuron: 
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/1-lif.ipynb) 
[![Open In kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://raw.githubusercontent.com/neural-reckoning/cosyne-tutorial-2022/main/1-lif.ipynb)
* Coincidence detection (and exercise): 
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/2-coincidence-detection.ipynb) 
[![Open In kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://raw.githubusercontent.com/neural-reckoning/cosyne-tutorial-2022/main/2-coincidence-detection.ipynb)


## Run locally 💻 

For part 1 using Brian:

```
conda env create -f environment_brian.yml
conda activate cosyne22_brian
jupyter notebook
```
