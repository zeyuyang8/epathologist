# E-Pathologist

## Resources

[cellseg-models-pytorch](https://pypi.org/project/cellseg-models-pytorch/)

## Introduction

E-Pathologist is a python toolbox for digital pathology image analysis.

## Installation

Create a virtual environment and install the dependencies:

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

## Observations

When I trained the Mask-RCNN model on the NuCLS data, it has a big overfitting problem. The reasons incldue:

- Number of classes in NuCLS is 15, which is too many.
- I cannot gaurrenttee the cell type is distinguishable
- The backbone I used is ResNet50, but it may help if I train the classifer first on cropped nucleis
- Weighted cross entropy loss for the classifier.
