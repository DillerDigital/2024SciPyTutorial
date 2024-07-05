# 2024 SciPy Tutorial - A Practical Introduction to NumPy

Materials for the NumPy Tutorial at SciPy 2024

# Setup Intructions

## Download Tutorial Materials

- The easiest way to get the materials is to clone this repository (SSH, HTTPS, or GitHub CLI should all work) using commands in the green "Code" button above.  For example, using the SSH method, type:

```
git clone git@github.com:DillerDigital/2024SciPyTutorial.git
```

- You can also download the zipped folder directly using GitHub's download features.
- Open a terminal session and navigate to the tutorial folder.


## Create a Python Environment
I **strongly recommend** that you work in a dedicated environment for this tutorial (and for each project you work on).  For a host of reasons, it's better not to modify your base (or system) Python by installing packages globally, and it's better not to do all of your work in the same Python environment.  [Here](https://stackoverflow.com/a/41972262/1001165) is one nicely articulated explanation.  The internet has many more.

There are at least three good methods of using Python environments.  It doesn't matter so much which one you select;  they each have their strengths and weaknesses.  The biggest advantage will be with the one you're already familiar with.

### Python + `pip`
- If you don't have Python on your system, [download version 3.11](https://www.python.org/downloads/release/python-3119/) and install it now.  (Some data science libraries are still working on complete compatibility with 3.12, but that is coming soon.)
- In your tutorials folder, type the following to create a `venv` and use `pip` to install the necessary dependencies.  Note:  depending on your system, you may need to type `python3` instead of `python` for the first line below to work:

#### On MacOS or Linux/Unix:
- In a terminal, type:
```
$ python -m venv numpy_tutorial_venv
$ source numpy_tutorial_venv/bin/activate
(numpy_tutorial_venv) $ pip install jupyterlab numpy matplotlib
```

#### On Windows
- In a PowerShell terminal, type:
```
C:\Users\you\Tutorial> python -m venv numpy_tutorial_venv
C:\Users\you\Tutorial> numpy_tutorial_venv\Scripts\Activate.ps1
(scipy_2024_tutorial)C:\Users\you\Tutorial> pip install jupyterlab numpy matplotlib
```

### Enthought Deployment Manager
- The Enthought Deployment Manager `edm` will install Python executables and well-tested packages.  Currently delivering Python 3.8 and soon to deliver 3.11, the focus of packages delivered by `edm` is stability, thorough testing, and seamless interoperability.  There is is no need to install Python separately, as `edm` will install runtime executables.
- [Download](https://assets.enthought.com/downloads/edm/) and [install](http://docs.enthought.com/edm/installation.html) Enthought's EDM.
```
$ edm envs create numpy_tutorial
$ edm shell -e numpy_tutorial
(numpy_tutorial) $ edm install jupyterlab numpy matplotlib
```

### Conda
- Download the [`conda` installer](https://www.anaconda.com/download/) from Anaconda.  `conda` is a popular and widely-used distribution of Python and packages suitable for scientific computing.
```
$ conda create -n numpy_tutorial_venv jupyterlab numpy matplotlib
$ conda activate numpy_tutorial_venv
```

## Start Jupyter Lab
- From your terminal, change to the directory you cloned or the direcotry where you downloaded the notebook and data directory.
- Type the following to launch Jupyer Lab:

```
(numpy_tutorial_venv) $ jupyter lab
```

- Click the folder icon at the left edge of the browser window.
- Double-click the file `scipy_2024_numpy_tutorial.ipynb`.
- Appearance of the tutorial notebook indicates a successful installation.
