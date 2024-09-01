# Flower: Raspberry Pi Cluster Apps

## Install dependencies and project

In any of the subdirectories start with installing the project.

```bash
pip install -e .
```

## Run with the Simulation Engine

In the `quickstart-docker` directory, use `flwr run` to run a local simulation:

```bash
flwr run .
```

## Run on the Raspberry Pi Cluster

```bash
flwr run . raspberry-pi-cluster
```

## Available Dependencies on ClientApp container

The ClientApp container has the following dependencies preinstalled as as it
is supposed to be used without internet access using exactly those will ensure
that apps can run without issues.

- flwr[simulation]>=1.11.0
- flwr-datasets[vision]>=0.3.0
- torch==2.2.1
- torchvision==0.17.1
- transformers>=4.30.0,<5.0
- evaluate>=0.4.0,<1.0
- datasets>=2.0.0, <3.0
- scikit-learn>=1.3.1, <2.0
- pandas>=2.2.2
