# cosyne-tutorial-2022
Cosyne workshop tutorial 2022

## Run via cloud (Google Colab / Kaggle)

If you have a Google account, launch with Colab. If you are in a country that blocks Google such as China, you can try
using Kaggle instead. [Some instructions from Neuromatch Academy are here.](https://deeplearning.neuromatch.io/tutorials/TechnicalHelp/Tutorial_kaggle.html)

Part 1 - "Classical" spiking neural networks

* Leaky integrate-and-fire neuron: [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/1-lif.ipynb) [![Open In kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://raw.githubusercontent.com/neural-reckoning/cosyne-tutorial-2022/main/1-lif.ipynb)
* Coincidence detection (and exercise): [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/2-coincidence-detection.ipynb) [![Open In kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://raw.githubusercontent.com/neural-reckoning/cosyne-tutorial-2022/main/2-coincidence-detection.ipynb)

## Local installation instructions

For part 1 using Brian:

```
conda env create -f environment_brian.yml
conda activate cosyne22_brian
jupyter notebook
```