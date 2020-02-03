# Jupylet

_jupylet_ is the marriage of Jupyter and the pyglet game programming library. It is intended for two types of audiences:
* Kids and their parents interested in learning to program, 
* Researchers and students of deep reinforcement learning.

A Jupyter notebook is in essence a laboratory for programming. It is the ideal environment for playing around with code, experimenting, and exploring ideas. It is used by professional machine learning scientists who come every day to play at work, so why not by kids?

pyglet is a powerful game programming library. It is wonderfully easy to use for creating simple 2D games, and since it is built on top of OpenGL it is powerfull enough for creating 3D engines if you really want to. The sky is the limit really.

By marrying Jupyter and pyglet, you get the best of both worlds. Learn to program by creating games interactively. Watch the game change as you type new code. Change a variable or a function and the game will be affected immediately. 

_jupylet_ is also a tool for **reinforcement learning research and development**. It is easy to use to create novel environments in which to experiment with reinforcement learning algorithms, and it can render thousands of frames per second. Head to [examples/pong-RL.ipynb](https://github.com/nir/jupylet/blob/master/examples/pong-RL.ipynb) to see how to programmatically control and render a 2-player version of pong.

# Try It Online

You can try Jupylet online on a Binder server without installing it by clicking:  

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nir/jupylet/master?filepath=examples%2Fspaceship.ipynb)

# Requirements

_jupylet_ should run on Python 3.4+ on Windows, Mac, and Linux.

# How to Install

If you are new to Python, I strongly recommend that you install and use the [Miniconda Python](https://docs.conda.io/en/latest/miniconda.html) distribution. Download and run the 64-bit installer and stick to the default install options.

Once Miniconda is installed start a Miniconda Prompt. To do this on Windows click the Windows key, search for "Miniconda Prompt", and click it. This should open a small dark window that programmers call _console_ or _shell_ in which you can enter commands and run programs.

To run _jupylet_ first install it with:

    pip install jupylet

Next, download the _jupylet_ archive or use [git](https://git-scm.com/) to clone this repository with:

    git clone https://github.com/nir/jupylet.git

Then enter the _jupylet/examples/_ folder and start a jupyter notebook with:

    jupyter notebook spaceship.ipynb

Run the notebook and a game canvas should appear with the spaceship example:

<img src="https://raw.githubusercontent.com/nir/jupylet/master/docs/images/spaceship.gif" width="256" height="256" />

You can run essentially the same code from the console with:

    python spaceship.py

The only difference in the code is that the application object is instantiated with:

    app = App(mode='window')

# Documentation

In terms of its interface _jupylet_ introduces only minor additions and modifications to the underlying pyglet library. Therefore the bulk of learning to use it is covered by the [pyglet documentation](https://pyglet.readthedocs.io/en/stable/). I have started writing a [guide](https://jupylet.readthedocs.io/en/latest/) and will add documentation in the comming days; in the mean time head to the [spaceship.ipynb](https://github.com/nir/jupylet/blob/master/examples/spaceship.ipynb) example to get started. 

# Contact

For questions and feedback send an email to [Nir Aides](mailto:nir@winpdb.org).
