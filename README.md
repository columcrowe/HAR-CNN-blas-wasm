# HAR CNN - A WebAssembly BLAS Demo

A WebAssembly BLAS Demo modified for human activity recognition (HAR) using IMU data.

Forked from https://github.com/georgestagg/mnist-classifier-blas-wasm.
With modifications from https://github.com/lfortran/mnist-classifier-blas-wasm/

A 1D CNN model is used for the classification of accelerometer signals (3-channels).

The pre-training of model weights has been performed ahead of time using Pytorch.

A private dataset was used to train the model. Data and classifier output is shown interactively using uPlot.

A pipeline is provided to convert .cwa files to binary format using scikit-digital-health. 


python train/utils.py <path_to_file.cwa>


The resulting .dat file can be uploaded for processing which runs using JavaScript and WebAssembly.


Eg., accsamp.dat


# Interactive Website

https://columcrowe.github.io/HAR-CNN-blas-wasm/
