---
layout: default
title:  "Python Setup"
date:   2016-12-25 17:50:00
categories: Python-Tutorial
---


# PYTHON INSTALLATION GUIDE

In this text article we'll go over a written guide to installing the course materials. If you prefer to follow a video guide, check out the next lectures that correspond to your OS anywhere online (or even Youtube), however, installation is actually very straight-forward.

I will be using Jupyter Notebook as it makes it easier to type and execute python scripts than running it the traditional way. Jupyter Notebook is a browser based IDE. 

# COURSE INSTALLATION STEPS

* Go to the [Jupyter Website](http://jupyter.org)
* Scroll down and and click the Install the Notebook button
* The button will take you to the [installation documentation](http://jupyter.readthedocs.org/en/latest/install.html).
* Follow the instructions there that best suit your set-up, but I recommend following the instructions for downloading Jupyter and Python with the Anaconda Distribution.
* Go to the [Anaconda Installation](https://www.continuum.io/downloads) page and click on the Graphical Installer for your system to download the installer.
* Follow the directions for the graphical installer you chose.
* Once you've successfully downloaded Anaconda you can begin with the installation commands for Jupyter. All installation commands should be run in the Terminal (for Mac and Linux) or the Command Prompt/Powershell (Windows). (Mac users should just search for `terminal` in Spotlight search, Windows Users just search ofr either `powershell` or `cmd` in your windows search tool to find your approriate installation tool). You also have the option of using the `Anaconda Command Prompt` as shown in the videos.
* Go to your terminal/command prompt and type `conda install jupyter`
* You should see some text show up describing the installation.
* Once the installation is done, in your `terminal/command prompt` `mkdir python-learning` (or any directory name you like) and then type: `jupyter notebook`
* You should eventually see a new tab open up in your browser for you to begin using Jupyter Notebooks. Click on New and select `Python 2`
* For more information on how to use the Jupyter Notebooks, refer to the other lectures in this section.
* For more information on the Jupyter Notebook system in general, check out the [official documentation](official documentation).

You should see something like this:![alt text](/src/images/jupyter.png)

We will be using this throughout the course. In the empty cell we type our code and shift+tab will run the code or you may also click on the 'Play' button at the top to run/execute the code.

You can try a simple ```print ('Hello World')``` and press shift+tab and see the code execute. Use this to try out all the code examples throughout this course. Hope it works out well. If no go, feel free to use any IDE you like. I would recommend PyCharm and Sublime over anything else. I also favor VIM and EMACS.

Now lets quickly take a look at other resources that can help you learn and practice python along the way. 
### [Click here](/python-tutorial/2016/12/25/practice.html)