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

## Datasets

- [TCGA-NuCLS](https://sites.google.com/view/nucls/home) (image and nuclei localization and classication)
- [TCGA-BCSS](https://bcsegmentation.grand-challenge.org/) (image and region segmentation)
- [TCGA-BRCA](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=3539225) (image and metadata of patients)

## Usage

TBD
