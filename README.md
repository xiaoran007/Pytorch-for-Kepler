# Pytorch-for-Kepler
Pytorch wheel package built for Nvidia Kepler GPUs. Currently supports newer Kepler GPUs (cuda compute capability 3.5 and 3.7) on Linux. 

# How to use
to use this pre-build package, simply download whl file from the release, and install it using pip:
```python
python -m pip install ./torch-2.1.0a0+git7bcf7da-cp39-cp39-linux_x86_64.whl # change whl package name to real file name.
```

# OS Support
This pre-build package only supports Linux (only tested on Ubuntu). The supported architecture is amd64. If you want to use Kepler GPU on arm64 or other architecture, please follow this [guide](https://github.com/xiaoran007/Old-GPUs-DL) to build pytorch from source.

# GPU Support
This pre-build package only supports CUDA cc3.5 and cc3.7.  The Kepler architecture is already 13 years, and considering the practical performance, only the top-line chips are still usable today. Here is a brief description of these chips.

## Support Matrix

| **Chip Name** | **CUDA CC** |                       **Product Name**                       |
| :-------: | :-----: | :----------------------------------------------------------: |
|  GK 110   |   3.5   |                GTX 780, GTX TITAN, Tesla K20                 |
|  GK 110B  |   3.5   | GTX 780Ti, GTX TITAN BLACK, GTX TITAN Z, Tesla K40, Quadro 5200, Quadro 6000 |
|  GK 180   |   3.5   |                          Tesla K40c                          |
|  GK 210   |   3.7   |                          Tesla K80                           |


