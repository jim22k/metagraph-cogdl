# metagraph-cogdl

[![Conda Version](https://img.shields.io/conda/v/metagraph/metagraph-cogdl.svg)](https://anaconda.org/metagraph/metagraph-cogdl)
[![Build Status](https://github.com/metagraph-dev/metagraph-cogdl/actions/workflows/test_and_deploy.yml/badge.svg?branch=main)](https://github.com/metagraph-dev/metagraph-cogdl/actions/workflows/test_and_deploy.yml?query=branch%3Amain)
[![Daily Health Check](https://github.com/metagraph-dev/metagraph-cogdl/actions/workflows/daily_checkup.yml/badge.svg)](https://github.com/metagraph-dev/metagraph-cogdl/actions/workflows/daily_checkup.yml)

A collection of metagraph plugins using CogDL

To install, run the following:

```
conda env create
conda activate mgcogdl

pip install torch==1.4.0
export CUDA=cu101
pip install torch-scatter==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.4.0.html
pip install torch-sparse==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.4.0.html
pip install torch-cluster==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.4.0.html
pip install torch-spline-conv==latest+${CUDA} -f https://pytorch-geometric.com/whl/torch-1.4.0.html
pip install torch-geometric
pip install dgl-cu101
git clone https://github.com/THUDM/cogdl.git
cd cogdl
pip install -e .
cd ..

pre-commit install
python setup.py develop
```
