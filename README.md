# brownie-play
Play with Brownie

# Installation

## Update packages
```console
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install python3.8
sudo apt-get install python3.8-dev
sudo apt-get install python3.8-venv
sudo apt-get install python3-pip
```

## Use latest version of Python (3.8)

```console
python --version
```

If it isn't 3.8, then:
```console
alias python=python3.8
alias python3=python3.8
su
alias python=python3.8
alias python3=python3.8
```

## Brownie needs
Do installs as [Brownie requests](https://medium.com/@iamdefinitelyahuman/getting-started-with-brownie-part-1-9b2181f4cb99). These include the following.

Check that npm and nodejs are installed. 
```console
node -v
npm -v
```

We need nodejs >= 6.11.5 to run ganache-cli. [Here's](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) installation instructions if needed.

Install ganache-cli:
```console
sudo npm install -g ganache-cli
```

Install pipx:
```console
python -m pip install --user pipx
python -m pipx ensurepath
```

Install Brownie:
```console
pipx install eth-brownie
```

## Get code
```console
git clone https://github.com/oceanprotocol/brownie-play.git
cd brownie-play
```

# Build / play

Some actions here:
* Coding in to this repo, with git and friends
* Brownie tutorials [1](https://medium.com/@iamdefinitelyahuman/getting-started-with-brownie-part-1-9b2181f4cb99), [2](https://medium.com/better-programming/getting-started-with-brownie-part-2-615a1eec167f), [3](https://medium.com/better-programming/getting-started-with-brownie-part-3-ef6bfa9867d7)

# Appendix: Currently Unneeded

## Virtual Env't 

Initalize virtual env't
```console
python -m venv myenv
```

Get going in new session
```console
source myenv/bin/activate 
pip install -r myenv_requirements.txt 
```

Wind down session // turn off env't
```console
deactivate
```
