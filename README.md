# The Intelligent Bitcoin Miner, Part II

## At a Glance

This app simulates the behavior and profitability of Bitcoin miners
for The Intelligent Bitcoin Miner Part II.

The code is divided into four main files: 

- `config.py`, which sets user-adjustable parameters; 

- `constants.py`, which sets hard-coded parameters; 

- `CMDataLoader.py`, which fetches historical data from the [Coin
Metrics API](https://charts.coinmetrics.io/network-data/);


- `agents.py`, which specifies agent behavior; 

- `generators.py`, which generates agents according to specified
distributions; 

- `Simulator.py`, which specifies the behavior for a simulation run
over one or several trials; 

- and `main.py`, which runs simulations and outputs summary plots in
`/plots/`.

For more information on the model parameters, please see the attached
article or dive into the code!

We use historical price and hashrate data from [Coin
Metrics](https://charts.coinmetrics.io/network-data/) and rig price
data from [Hashrate
Index](https://hashrateindex.com/machines/sha256-rig-index) and
General Mining Research to seed our model.

## Installing

This project requires python3 and virtualenv.

On debian 12, install following packages.

```bash
sudo apt install python3 virtualenv python-is-python3
```

Python version should be 3:

```bash
python --version
```

Clone the repository to your computer, and cd into the cloned
directory.  Start a new virtual environment and install the
requirements:

```bash
python -m venv .venv
source ./.venv/bin/activate
./.venv/bin/pip install -r requirements.txt
```

## Running

```bash
./.venv/bin/python main.py
```

## Afterword

Happy hashing!
