# brownie-instrs
This repo has instructions of how to install and play with Brownie. It distills the Brownie tutorials (linked below) and helps with installations gotchas.

# Installation

[Install Brownie & dependencies](README_install.md)

# Bake Existing Brownie Token
This is part of [Brownie tutorial 2](https://medium.com/better-programming/getting-started-with-brownie-part-2-615a1eec167f).

We could use `brownie init` to start our own Brownie project. But for now let's use [`token-mix`](https://github.com/brownie-mix/token-mix), a simple pre-created project to play with ERC20.
```
brownie bake token
cd token
```

Compile the project.
```
brownie compile
```

Note: Brownie auto tracks the files in your project’s `contracts/` folder and will run the compiler when a file is added or changed. There isn’t often a need to manually compile — but it’s still good to know how.


# Build / play

Subsections below can be in any order.

Ensure that `python` uses Python 3.8. If not, use alias like above.

## Play with `token` project

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
```
brownie console
```

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
