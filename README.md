# cosyne-tutorial-2022
Cosyne workshop tutorial 2022

## Run via cloud (Google Colab)

Part 1 - "Classical" spiking neural networks

* Leaky integrate-and-fire neuron: [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/1-lif.ipynb)
* Coincidence detection (and exercise): [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/2-coincidence-detection.ipynb)

## Local installation instructions

For part 1 using Brian:

```
conda env create -f environment_brian.yml
conda activate cosyne22_brian
jupyter notebook
```