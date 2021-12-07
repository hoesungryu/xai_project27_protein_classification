# xai_project27_protein_classification

This is a PyTorch implementation of several Graph Convolutional Neural networks. 

## Requirements
* python==3.8
* TORCH==1.10
* CUDA=cu102
```
pip install torch-scatter -f https://pytorch-geometric.com/whl/torch-${TORCH}+${CUDA}.html
pip install torch-sparse -f https://pytorch-geometric.com/whl/torch-${TORCH}+${CUDA}.html
pip install torch-cluster -f https://pytorch-geometric.com/whl/torch-${TORCH}+${CUDA}.html
pip install torch-spline-conv -f https://pytorch-geometric.com/whl/torch-${TORCH}+${CUDA}.html
pip install torch-geometric
pip install easydict # https://ddiri01.tistory.com/302
```

## Run
```
run main.ipynb
```

## Results 

```sh
> GCN: 0.727 ± 0.032
> GraphSAGE: 0.722 ± 0.034
> GIN: 0.720 ± 0.032
> SAGPool: 0.725 ± 0.028
> SortPool: 0.737 ± 0.020
> TopK: 0.722 ± 0.024
```

## Dataset
Graph classification benchmarks are publicly available at [here](https://ls11-www.cs.tu-dortmund.de/staff/morris/graphkerneldatasets).