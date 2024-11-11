---
layout: post
title:  "Pyenv Basic Setup Instructions"
date:   2024-01-29 10:36:24 -0500
---

## Install Multiple Python Versions for Specific Project

- Home project: https://github.com/pyenv/pyenv

- Reference to: https://www.tecmint.com/pyenv-install-and-manage-multiple-python-versions-in-linux/

## 1. Install pyenv in Linux

### 1.1. Install all the required packages

```shell
# On Debian/Ubuntu/Linux Mint ------------ 
sudo apt install curl git-core gcc make zlib1g-dev libbz2-dev 
libreadline-dev libsqlite3-dev libssl-dev

# On CentOS/RHEL ------------
sudo yum -y install epel-release
sudo yum -y install git gcc zlib-devel bzip2-devel readline-devel sqlite-devel openssl-devel

# On Fedora 22+ ------------
sudo yum -y install git gcc zlib-devel bzip2-devel readline-devel sqlite-devel openssl-devel
```

### 1.2. Grab the the latest **pyenv** source tree from its Github repository

```shell
git clone https://github.com/pyenv/pyenv.git $HOME/.pyenv
```

### 1.3. Set the environment variable **PYENV_ROOT**

```shell
vim $HOME/.bashrc
```

```bash
## pyenv configs
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"

if command -v pyenv 1>/dev/null 2>&1; then
  eval "$(pyenv init -)"
fi
```

### 1.4. source **$HOME/.bashrc** file or restart the shell

```shell
source $HOME/.bashrc
# or:
exec "$SHELL"
```

## 2. How to install Multiple Python Versions in Linux

```shell
# View all available versions with this command.
pyenv install -l

# You can now install multiple Python version via pyenv, for example.
pyenv install 3.6.4
pyenv install 3.6.5

# List all Python versions available to pyenv
pyenv versions

# Check the global Python version
pyenv global

# Set the global python version using the pyenv command
pyenv global 3.6.5
pyenv global

# Set the local Python version on per-project basis
# For instance, if you have a project located in $HOME/python_projects/test,
# you can set the Python version of it using following command.
cd python_projects/test
pyenv local 3.6.5
pyenv version		#view local python version for a specific project, or:
pyenv versions
```

## 3. Extra:

Pyenv manages virtual environments via the **pyenv-virtualenv plugin** which automates management of **virtualenvs** and **conda** environments for Python on Linux and other UNIX-like systems.

### 3.1. Installing this plugin using following commands

```shell
git clone https://github.com/yyuu/pyenv-virtualenv.git $HOME/.pyenv/plugins/pyenv-virtualenv
source $HOME/.bashrc
```

### 3.1. Create a test virtual environment

called **venv_project1** under a project called **project1** as follows

```shell
cd python_projects
mkdir project1
cd project1
pyenv virtualenv 3.6.5 venv_project1
```

