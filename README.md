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
using Kaggle instead.

**Part 1 • "Classical" spiking neural networks**

* Leaky integrate-and-fire neuron: 
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/1-lif.ipynb) 
[![Open In kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://raw.githubusercontent.com/neural-reckoning/cosyne-tutorial-2022/main/1-lif.ipynb)
* Coincidence detection (and exercise): 
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/2-coincidence-detection.ipynb) 
[![Open In kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://raw.githubusercontent.com/neural-reckoning/cosyne-tutorial-2022/main/2-coincidence-detection.ipynb)


## Run locally 💻 

Follow the instructions below to install the software 
necessary to run the notebooks on your own computer.

In short, if you already use `conda`:
download this repository, and run, in this directory:
```
conda env create -f environment_brian.yml
conda activate cosyne22_brian
jupyter notebook
```
This is for the first part (which uses [Brian](https://brian2.readthedocs.io/)).
For the second part (which uses PyTorch), do the same 
but with `-f environment_torch.yml` and `activate cosyne22_torch`.

In more detail (click on a section to expand it):

<details>
<summary>1. <b>Install Conda</b></summary>

- If you do not have `conda` already installed, 
  download and run the latest _Miniconda_ installer for your OS 
  [here](https://docs.conda.io/en/latest/miniconda.html#latest-miniconda-installer-links).  

- In step 5 of the installer ("Advanced Options") tick the checkbox next to 
  "Add Miniconda3 to my PATH environment variable".
</details>

<details>
<summary>2. <b>Download the exercises</b></summary>

- Here on GitHub, at the top of the page, click the green "Code" button 
  and "Download ZIP", then uncompress the downloaded `.zip`.

- Alternatively, if you use Git, you can optionally fork and `git clone` this repository.
</details>

<details>
<summary>3. <b>Open a terminal in the exercise directory</b></summary>

- On Windows, either search the Start menu for the built-in 'Command Prompt', 
  or install the more modern [Windows Terminal](https://github.com/microsoft/terminal#readme)
  from the Microsoft Store ([link](https://www.microsoft.com/store/productId/9N0DX20HK701)).

- To run the commands in the following steps, either type or copy-paste them
  into the terminal, and then hit `Enter`.

- After starting the terminal, you can use the `cd` command to point it
  to the exercise directory. For example, if you extracted the `.zip` contents
  to `C:\Users\jane\Desktop`, run
  ```
  cd C:\Users\jane\Desktop\cosyne-tutorial-2022-main
  ```
  Your final directory should be the one where this `README.md` 
  and the `environent_….yml` files are located.
</details>

<details>
<summary>4. <b>Install dependencies</b></summary>

- With your terminal pointing to the exercise directory, run the following commands.
  ```
  conda env create -f environment_brian.yml
  ```
  This will download and install all dependencies. It can take a while.
  
- If any errors pop up, try restarting your terminal with elevated privileges
  (on Windows: "Run as Administrator"), and run the above command again.

- When the installation was succesful, run
  ```
  conda activate cosyne22_brian
  ```
  This makes sure all commands next launched from the current terminal
  will use the software installed with the previous command.

</details>

<details>
<summary>5. <b>Run the notebook server</b></summary>

- Still in this terminal in the exercise directory,
  with the `cosyne22_brian` conda environment activated, run
  ```
  jupyter notebook
  ```
  This should open your browser, showing a list of the files in the current directory. 

- Click on one of the exercise notebook files to open it.
  Try running some of the cells using `Shift`-`Enter`.
  If no error apear below these cells: congratulations! The installation was succesful.

- Some more information on how to work with a Jupyter Notebook can be found
  e.g. [here](https://realpython.com/jupyter-notebook-introduction/#running-cells).

- When you are done with the notebooks, you can exit the notebook server application
  that is still running in your terminal with `Ctrl`-`c`
</details>
