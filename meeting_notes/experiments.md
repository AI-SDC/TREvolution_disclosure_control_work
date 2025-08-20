# Experiments

## Datasets

### Images

#### Standard MIA Benchmarks

Available from [PyTorch](https://docs.pytorch.org/vision/main/datasets.html) and [Hugging Face](https://huggingface.co/datasets):

* MNIST - 10 classes, 60,000 samples, 1024 features
* FMNIST - 10 classes, 70,000 samples, 1024 features
* CIFAR10 - 10 classes, 60,000 samples, 3072 features
* CIFAR100 - 100 classes, 60,000 samples, 3072 features
* CINIC10 - 10 classes, 270,000 samples, 3072 features
* ImageNet - 1000 classes, 1,431,167 samples, (typically resized to) 150,528 features 

### Tabular

#### Standard MIA Benchmarks

First used in [Shokri et al. (2017)](https://www.computer.org/csdl/proceedings-article/sp/2017/07958568/12OmNBUAvVc):

* Purchase100 - 100 classes, 39,464 samples, 600 (binary) features
    - Available from [kaggle](https://www.kaggle.com/c/acquire-valued-shoppers-challenge/data)
* Location - 30 classes, 4,000 samples, 446 (binary) features
    - Available from [google](https://sites.google.com/site/yangdingqi/home/foursquare-dataset)

#### [OpenML](https://www.openml.org) 

OpenML provide open datasets and **tasks** which define specific problems to be solved using a given dataset. Task IDs specify train and test sets, which target feature(s) to predict for supervised problems, and possibly which evaluation measure to optimise.

See [scikit-learn docs](https://docs.openml.org/ecosystem/Scikit-learn/)

OpenML Task IDs used previously for [Bertran et al. (2023)](https://proceedings.neurips.cc/paper_files/paper/2023/hash/01328d0767830e73a612f9073e9ff15f-Abstract-Conference.html):

Task IDs:
* 361057
* 361064
* 361067
* 361070 

Additional OpenML tabular dataset Task IDs, previously used for benchmarking tree-based models and deep neural networks can be found in [Grinsztajn et al. (2022)](https://arxiv.org/abs/2207.08815)

OpenML datasets used previously for [Preen and Smith (2025)](https://arxiv.org/abs/2502.09396):

DataSet IDs (**note: identify appropriate Task ID instead for consistency**):
* 41946 - Sick
* 310 - Mammography

Additional datasets used previously for [Preen and Smith (2025)](https://arxiv.org/abs/2502.09396):

* [Indian Liver](https://doi.org/10.24432/C5D02C)
* [MIMIC-II](https://doi.org/10.13026/C2NC7F)
* In-hospital-mortality---extracted from [MIMIC-III](https://doi.org/10.5061/dryad.0p2ngf1zd)

## Target Models

### Images

Standard CNNs previously used for MIA benchmarking:

* ResNet18 - from [He et al. (2016)](https://ieeexplore.ieee.org/document/7780459)
* DenseNet121 - from [Huang et al. (2017)](https://ieeexplore.ieee.org/document/8099726)
* WideResNet - from [Zagoruyko et al. (2016)](https://arxiv.org/abs/1605.07146)
* AlexNet

Also available are some [pre-trained PyTorch models](https://github.com/bearpaw/pytorch-classification), used previously in [Nasr et al. (2019)](https://ieeexplore.ieee.org/document/8835245) for white-box neural net MIA.

### Tabular

Neural networks:

* Same as those used previously.

Trees from [scikit-learn](https://scikit-learn.org):

* XGBoost
* Random Forest
* Decision Tree
* Which hyperparameters --- same as [Preen and Smith (2025)](https://arxiv.org/abs/2502.09396)?

## Attacks

* Running LiRA will create and save shadow models, which can be reused later.

## Results Collection

* Currently **sacroml** produces JSON reports, which may not be the same outputs as previously recorded for [Preen and Smith (2025)](https://arxiv.org/abs/2502.09396).
* Does this need to be modified?
