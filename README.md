# ABSA-PyTorch

> Aspect Based Sentiment Analysis, PyTorch Implementations.
>

![LICENSE](https://img.shields.io/packagist/l/doctrine/orm.svg)
[![Gitter](https://badges.gitter.im/ABSA-PyTorch/community.svg)](https://gitter.im/ABSA-PyTorch/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)


## Requirement

* pytorch >= 0.4.0
* numpy >= 1.13.3
* sklearn
* python 3.6 / 3.7
* transformers

To install requirements, run `pip install -r requirements.txt`.

* For non-BERT-based models,
[GloVe pre-trained word vectors](https://github.com/stanfordnlp/GloVe#download-pre-trained-word-vectors) are required, please refer to [data_utils.py](./data_utils.py) for more detail.

## Usage

### Training

```sh
python train.py --model_name bert_spc --dataset restaurant
```

* All implemented models are listed in [models directory](./models/).
* See [train.py](./train.py) for more training arguments.
* Refer to [train_k_fold_cross_val.py](./train_k_fold_cross_val.py) for k-fold cross validation support.

### Inference

* Refer to [infer_example.py](./infer_example.py) for both non-BERT-based models and BERT-based models.


## Licence

MIT
