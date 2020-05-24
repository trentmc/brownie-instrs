# Installation

Here, we install Brownie and dependencies.

This includes going through the key steps of [Brownie tutorial 1](https://medium.com/@iamdefinitelyahuman/getting-started-with-brownie-part-1-9b2181f4cb99). It also addresses gotchas that I encountered when installing.

## Update Python packages

Get packages, updated
```console
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install python3.8
sudo apt-get install python3.8-dev
sudo apt-get install python3.8-venv
sudo apt-get install python3-pip
sudo apt-get install python3-apt
```

Check python version
```console
python --version
```

If it isn't 3.8, then do the following. (We can't put this into .bashrc because Ubuntu needs python2.7 in some places :/ )
```console
alias python=python3.8
alias python3=python3.8
su
alias python=python3.8
alias python3=python3.8
```

 

Install pipx:
```console
python -m pip install --user pipx
python -m pipx ensurepath
```

## Update npm and nodejs

Check that npm and nodejs are installed. 
```console
node -v
npm -v
```

We need nodejs >= 6.11.5 to run ganache-cli. [Here's](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) installation instructions if needed.

## Install ganache-cli and brownie

```console
sudo npm install -g ganache-cli
pipx install eth-brownie
```

## Get this repo

Clone this repo, then cd into the directory and play:)
