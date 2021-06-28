# Monotone operator equilibrium networks

Repository to hold the code of final project of Course "Optimization Methods for Machine Learning". The code is based on the original forked [repository](https://github.com/locuslab/monotone_op_net).


**See the [tutorial notebook](tutorial.ipynb) for an introduction to the original paper and the code in this repo.**

Code to replicate the experiments can be found in [`experiments.ipynb`](experiments.ipynb). 

## Experiment Results

Training time (per epoch) of different operator splitting methods on Multi-tier network without data augmentation.

|       | Forward-Backward |  Peaceman | Douglas | ProxDecomp |
| ----- | --- | --- | ----- | --- |
| Time/s | 202.97 | **87.33** | 129.57 | 140.82 |

Model accuracy:

|       | Single conv | Multi-tier | Single conv lg. | Multi-tier lg. |
| ----- | --- | --- | ----- | --- |
| ReLU  | 74.10 | 72.14 | 81.40 | 88.62 |
| LeakyReLU | **74.13** | **72.70** | **81.60** | **88.87** |


## Requirements
Compatible with python 3.5+ and known to work with pytorch 1.4, torchvision 0.5, and numpy 1.18. Can install with `pip install -r requirements.txt`.
