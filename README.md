# Cosyne Tutorial 2022

These are the exercises for the [COSYNE](https://www.cosyne.org/) 2022 Tutorial, _Spiking Neural Network Models in Neuroscience_, by Dan Goodman.

The exercises are in Python, in the Jupyter Notebook format.
You can run these notebooks either locally, or in the cloud (via Google Colab or Kaggle). 
We recommend following the installation instructions for running locally
(found [below](#run-locally-)) before the conference: the on-site
Wi-Fi might be flaky and not able to handle all participants simultaneously.



## Run in the cloud ☁

If you have a Google account, you can launch with Colab.
If you are in a country that blocks Google, such as China, use Kaggle.
(To have the notebook kernel on Kaggle persist more than 15', register for a Kaggle account).

**Part 1 • "Classical" spiking neural networks**

* Leaky integrate-and-fire neuron: 
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/1-lif.ipynb) 
[![Open In kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://raw.githubusercontent.com/neural-reckoning/cosyne-tutorial-2022/main/1-lif.ipynb)
* Coincidence detection (and exercise): 
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neural-reckoning/cosyne-tutorial-2022/blob/main/2-coincidence-detection.ipynb) 
[![Open In kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://raw.githubusercontent.com/neural-reckoning/cosyne-tutorial-2022/main/2-coincidence-detection.ipynb)


## Run locally 💻 

Follow the instructions below to install the software 
necessary to run the exercise notebooks on your own computer.

In short, if you already use `conda`:
download this repository, and in this directory, run:
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

- For Windows users: in step 5 of the installer ("Advanced Options"),
  tick the checkbox next to "Add Miniconda3 to my PATH environment variable".
</details>

<details>
<summary>2. <b>Download the exercises</b></summary>

- Here on GitHub, at the top of the page, click the green "Code" button, then "Download ZIP".
  Uncompress the downloaded `.zip` to a location of your choosing.

- Alternatively, if you use Git, you can `git clone` this repository
  (or even a new GitHub fork of it, if you plan on contributing).
</details>

<details>
<summary>3. <b>Open a terminal in the exercise directory</b></summary>

- On Windows, either search the Start menu for the built-in 'Command Prompt', 
  or install the more modern [Windows Terminal](https://github.com/microsoft/terminal#readme)
  from the Microsoft Store ([link](https://www.microsoft.com/store/productId/9N0DX20HK701)).
  
- On MacOS or e.g. Ubuntu, run 'Terminal'.

- To run the commands in the following steps, either type or copy-paste them
  into the terminal, and hit `Enter`.

- After starting the terminal, you can use the `cd` command to point it
  to the exercise directory. For example, if you extracted the `.zip` contents
  to `C:\Users\jane\Desktop`, run
  ```
  cd C:\Users\jane\Desktop\cosyne-tutorial-2022-main
  ```
  
- Alternatively, you can open a terminal in the right directory directly
  from your OS's file explorer (Explorer on Windows, GNOME on Ubuntu, …),
  by right clicking in the directory.
  - If you've installed Windows Terminal or are e.g. on Ubuntu,
    simply select "Open in (Windows) Terminal" from the right-click menu.
  - If using vanilla Windows, hold `Shift` while right-clicking,
    then select "Open PowerShell window here" from the right-click menu.
  
- Your final directory should be the one where this `README.md` 
  and the `environent_….yml` files are located.
</details>

<details>
<summary>4. <b>Install dependencies</b></summary>

- With your terminal pointing to the exercise directory, run the following command:
  ```
  conda env create -f environment_brian.yml
  ```
  This will download and install all dependencies. It will likely take a while.
  
- If any errors pop up, retry the command with elevated privileges.
  - On Windows, close the terminal and reopen it with "Run as Administrator".
  - On most other OSes (including MacOS), prepend `sudo` to the command;
    i.e. `sudo conda env create …`.

- When the installation was succesful, run
  ```
  conda activate cosyne22_brian
  ```
  This makes sure that all future commands ran in this terminal
  will use the installed software.

</details>

<details>
<summary>5. <b>Run the notebook server</b></summary>

- Still in this terminal in the exercise directory,
  with the `cosyne22_brian` conda environment activated, run
  ```
  jupyter notebook
  ```
  After a short while, this should open your browser,
  showing a list of the files in the current directory. 

- Click on one of the exercise notebook files to open it.
  Try running some of the cells using `Shift`-`Enter`.
  If no errors apear below these cells: congratulations! The installation was succesful.

- Some more information on how to work with a Jupyter Notebook can be found
  e.g. [here](https://realpython.com/jupyter-notebook-introduction/#running-cells).

- When you are done with the notebooks, you can exit the notebook server application
  that is still running in your terminal with `Ctrl`-`C`
</details>
