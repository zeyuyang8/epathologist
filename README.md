# E-Pathologist

## Resources

[cellseg-models-pytorch](https://pypi.org/project/cellseg-models-pytorch/)

## Introduction

E-Pathologist is a python toolbox for digital pathology image analysis.

## Installation

Before installing the dependencies, run the following commands:

```bash
apt-get -y install libopenjp2-7-dev libopenjp2-tools openslide-tools
```

Then, create a virtual environment and install the dependencies:

```bash
conda create -n epathologist python=3.9
conda activate epathologist
pip install -r requirements.txt
pip install -e .
```

## Usage

TBD
