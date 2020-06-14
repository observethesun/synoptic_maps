[![Python](https://img.shields.io/badge/python-3-blue.svg)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-1.4-orange.svg)](https://tensorflow.org)

## Construction of synoptic maps and coronal holes segmentation

This repository contains the source code to reproduce coronal holes segmentation in synoptic maps following the paper [Machine-learning approach to identification of coronal holes in solar disk images and synoptic maps]().

### Online catalogue

Dataset of SDO/AIA 193 Angstrom and CHs synoptic maps is available online at [https://sun.njit.edu/coronal_holes/](https://sun.njit.edu/coronal_holes/). Feel free
to download and explore it in your research.

### Installation

Clone the repository with its submodules
```
git clone --recursive https://github.com/observethesun/synoptic_maps.git
``` 

### Usage

The code is based on [helio](https://github.com/observethesun/helio) framework. See the API [documentation](http://observethesun.github.io/helio/) to learn more about its features.

To start building synoptic maps you will need a dataset of solar disk images in JPEG or FITS formats.
Note that for JPEG images there will be required additional information on solar disk location.
Follow the steps in the notebook [Make_synoptic_maps](./notebooks/1.Make_synoptic_maps.ipynb) 
to complete the process.

For CHs segmentation we apply a neural network model trained on solar disk images. Visit the repository
[coronal_holes](https://github.com/observethesun/coronal_holes) to prepare the model.
It is recommended to use the same source of solar disk images for model training and synoptic maps
construction. Follow the notebook [CHs_segmentation](./notebooks/2.CHs_segmentation.ipynb) 
to apply the model for synoptic maps.


### Citing this work

```
Illarionov E., Kosovichev А., Tlatov A., 2020.
```