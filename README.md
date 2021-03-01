# Installation of TensorRT on Google Colab (or other environments)

TensorRT is an SDK by Nvidia for optimizing deep learning inference. Installation of TensorRT might be problematic, especially on Google Colab and/or your default environment owing to the following reasons:

- Conflict in default CUDA version and those supported by TensorRT
- Unmet dependencies introduced when installing the libnvinfer packages required.
- Trouble in setting up the cuDNN and other environment configuration in line with those expected by TensorRT

This notebook includes a set of commands which you can run to setup TensorRT 7.0 in your Google Colab without any hassle.

## Requirements

- Download the .deb file of the appropriate version of TensorRT from the [Nvidia developer portal](https://developer.nvidia.com/nvidia-tensorrt-7x-download). This notebook includes setup instructions for TensorRT 7.0.0 for Ubuntu 18.04 and CUDA 10.0. Make appropriate changes in the configuration values in the notebook if your version differs.
- In case of Google Colab, upload the .deb file to your Drive and make sure to connect to drive before executing the notebook. Also set the hardware accelerator to GPU before beginning execution.
