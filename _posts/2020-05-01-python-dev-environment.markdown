---
layout: post
title: "Guide to a wholesome Python dev environment"
date: 2020-05-01 18:41:35 +0100

---

I started coding with python, at the time I was 17 and barely knew about how much is the development environment important. Not just the computer itself is important but furthermore the Software. I was using windows and the basic Python IDE for an approx. 1000 lines project.

Module import was a nightmare for me as much as learning the language.

I recently faced a problem related to modules. My system's Python version was 3.8 and I needed the 3.6 version for the script to run. Furthermore, I needed 3.6 version cryptodome module.

Some Qwant searches, later on, I found about Pipenv and Pyenv.

## Pyenv

Pyenv allows us to have multiple python versions in one OS. By changing the symlinks and the Path variable it manages to change the direction of the Python commands and redirect to the other python versions.

Here is a link to the [documentation](https://github.com/pyenv/pyenv), I may have done mistakes while explaining the process. Here are the [main commands](https://github.com/pyenv/pyenv/blob/master/COMMANDS.md) of Pyenv.

But What if we want to install modules alongside our newly created Python version?

Well it's "complicated"

I had many problems and issues and that's why I recommend the following tool :

## Pipenv

Pipenv eases the problem of Python and Pip version Pyenv had. It creates a Pyenv environment with a Pip too.

Said like this, Pipenv is the dream come true of Python developers.

**It isn't.**

Pipenv has sometimes problems with its pipenv.lock. I had a problem when managing the modules for my Deep Reinforcement Learning you can look at [there](https://github.com/Ratatinator97/LunarLander-DQN). The Pipenv install &quot;module&quot; command was taking an eternity and I seemed broken.

And here's how I found [Poetry](https://python-poetry.org/).

# Poetry

From Poetry's website: *Python packaging and dependency management made easy*

And trust me it is easy!

I didn't experience bugs about *.lock or colossal wait during a command. It is simple and effective.

But Poetry doesn't change the Python version by itself, you have to create a Pyenv environment with the chosen version and then in the environment init a Poetry project. Look at their amazing documentation if you need some help.
