# brownie-play
Play with Brownie

# Installation

## Update packages
```console
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install python3.8
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

## Get code
```console
git clone https://github.com/oceanprotocol/brownie-play.git
cd brownie-play
```

## Initalize virtual env't
```console
python -m venv myenv
```

# Get going in new session

```console
source myenv/bin/activate 

[[unneeded: python3.8 has pipx]] python -m pip install --user pipx
[[unneeded: python3.8 has ensurepath]] python -m pipx ensurepath
[[unneeded: no other reqts right now]] pip install -r myenv_requirements.txt 

pipx install eth-brownie
```


# Wind down session

Turn off env't
```console
deactivate
```
