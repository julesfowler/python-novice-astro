---
layout: page
title: Setup
permalink: /setup/
root: ..
---

### Install Python:

0. Test if you already have Anaconda or Miniconda installed. In your terminal type the folloing commands:

~~~
$ bash
$ which conda
~~~
{: .source}

If this returns nothing, please proceed to the next step. If it produces a path such as /Users/yourname/anaconda/bin/conda (yours may be different), skip the next step and go straight to step 2.

1. Install Miniconda Python 3 by following the directions here:

https://astroconda.readthedocs.io/en/latest/getting_started.html#getting-started-jump

(Video tutorial here: http://swcarpentry.github.io/python-novice-gapminder/setup/)

You do not need root access. We recommend Miniconda rather than Anaconda because it is a faster and more light-weight installation.

2. Install Astroconda by following the instructions here - the first 4 yellow boxes on this page:
https://astroconda.readthedocs.io/en/latest/installation.html#standard-install

You will need terminal access for this. Ping the workshop instructor if you don't know how to do that. If you have already have an astroconda environment that prefer not to touch, then name the new one something different.

3. Clean up your workspace. Check your default profile files (.cshrc, .bashrc, .bash_profile) and comment any entries that define or add to $PYTHONPATH. Start a fresh Terminal window and type echo $PYTHONPATH - you should not see a long jumble of paths to unknown corners of your hard drive. If you don't know what this means, skip to the next one.

4. Get yourself a nicer terminal. [iTerm](https://www.iterm2.com/) is really nice for OSX. For Windows, here is [Git Bash](https://gitforwindows.org/).

5. For this class we can use Nano, Emacs or VIM, but if you want a nicer text editor, download Sublime Text, Atom, BBEdit or TextWrangler. We will not cover IDEs such as PyCharm or Spyder. 

### Obtain lesson materials

1. Download [intro_python_data.tar.gz](https://www.dropbox.com/s/gvw6fxq2du67vaz/intro_python_data.tar.gz?dl=1).
2. Create a folder called `swc-python` on your Desktop.
3. Move downloaded file into this newly created folder.
4. Unzip the files (gunzip file.tar.gz) and untar (tar -xvf file.tar) or all in one go (tar -zxvf file.tar.gz).

You should now see a new folder called `data` in your `swc-python` directory on your
Desktop.

&nbsp; <!-- vertical spacer -->

### Navigate to the `data` folder

If you're using a Unix shell application, such as the Terminal or iTerm app in macOS, Console or Terminal in
Linux, or [Git Bash](https://gitforwindows.org/) on Windows, execute the following command:

~~~
$ cd ~/Desktop/swc-python/data
~~~
{: .source}

On Windows, you can use its native Command Prompt program.  The easiest way to start it up is by
pressing <kbd>Windows Logo Key</kbd>+<kbd>R</kbd>, entering `cmd`, and hitting <kbd>Enter</kbd>. In
the Command Prompt, use the following command to navigate to the `data` folder:
~~~
$ cd /D %userprofile%\Desktop\swc-python\data
~~~
{: .source}

&nbsp; <!-- vertical spacer -->

### Activate your Python environment

In the terminal, type the following commands:

~~~
$ bash
$ source activate astroconda
~~~
{: .source}

&nbsp; <!-- vertical spacer -->

### Option 1: Launch Plain Vanilla Python interpreter

To start working with Python, we need to launch a program that will interpret and execute our Python
commands. To launch a "plain vanilla" Python interpreter, execute:
~~~
$ python
~~~
{: .source}

If you are using Git Bash on Windows, you have to call Python _via_ `winpty`:
~~~
$ winpty python
~~~
{: .source}

&nbsp; <!-- vertical spacer -->


### Option 2: Start IPython interpreter

IPython is an alternative solution situated somewhere in between the plain vanilla Python
interpreter and Jupyter notebooks.  It provides an interactive command-line based interpreter with
various convenience features and commands.  You should have IPython on your system if you installed
[Anaconda Distribution](http://carpentries.github.io/workshop-template/#python).

To start using IPython, execute:
~~~
$ ipython
~~~

&nbsp; <!-- vertical spacer -->

### Option 3: Start Jupyter notebook

Jupyter notebooks provide a browser-based interface for working with Python.  If you would like to
use a notebook during the lesson, make sure to install [Anaconda
Distribution](http://carpentries.github.io/workshop-template/#python).

To start a Jupyter server, execute:
~~~
$ jupyter notebook
~~~
{: .source}

Then create a new notebook by clicking "New" button on the right and selecting "Python 3" from the
drop-down menu:

![](../fig/new-notebook.png)
{: .source}

[zipfile1]: {{ page.root }}https://www.dropbox.com/s/gvw6fxq2du67vaz/intro_python_data.tar.gz?dl=0
