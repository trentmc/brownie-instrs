# brownie-play
Play with Brownie

# Install Brownie & related

This takes us through the key steps of [Brownie tutorial 1](https://medium.com/@iamdefinitelyahuman/getting-started-with-brownie-part-1-9b2181f4cb99). 

## Update Python packages

Get packages, updated
```console
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install python3.8
sudo apt-get install python3.8-dev
sudo apt-get install python3.8-venv
sudo apt-get install python3-pip
```

Check python version
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
```console
git clone https://github.com/oceanprotocol/brownie-play.git
cd brownie-play
```

# Get started with Brownie
This is part of [Brownie tutorial 2](https://medium.com/better-programming/getting-started-with-brownie-part-2-615a1eec167f).

## Bake token

We could use `brownie init` to start our own Brownie project. But for now let's use [`token-mix`](https://github.com/brownie-mix/token-mix), a simple pre-created project to play with ERC20.
```
brownie bake token
cd token
```

Compile the project.
```
brownie compile
```

Note: Brownie automatically tracks the files in your project’scontracts/ folder and will run the compiler when a file is added or changed. There isn’t often a need to manually compile — but it’s still good to know how.


# Build / play

These can be in any order.

## Play with token project

Go to project directory
```
cd token
```

Run tests, optionally showing code coverage
```
brownie test
brownie test --coverage
```

Run the deployment script. It will deploy to Ganache. (To deploy to a live network, use --network flag.)
```
brownie run token
```

Launch Brownie console.

## Explore Brownie's functionality

[See Brownie Tutorial 3](https://medium.com/better-programming/getting-started-with-brownie-part-3-ef6bfa9867d7)

## Play more in this repo
Code!

# Appendix: Currently Unneeded

## Virtual Env't 

Initalize virtual env't
```console
python -m venv myenv
```

Get going in new session
```console
source myenv/bin/activate 
<<create and fill myenv_requirements.txt>>
pip install -r myenv_requirements.txt 
```

Wind down session // turn off env't
```console
deactivate
```
