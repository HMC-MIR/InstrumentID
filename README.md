# InstrumentID

The goal of this project is to predict the instrument for which a page of sheet music is written by framing it as a text classification task. Our approach converts sheet music images into a sequence of musical words using the bootleg score representation, then utilizes language model pretraining to improve the performance of various neural network architectures on this task.

This repository contains both the code for training the neural networks and the precomputed features used in our experiments. It also contains a notebook for downloading the raw PDFs that make up the dataset.

## Getting Started

First install the dependencies by running:

```python
pip install -r requirements.txt
```

## Usage
If you want to download the PDFs that make up the dataset used, run the notebook 00_downloadScores.ipynb. The folder `cfg_files` contains the download links for all the PDFs in the dataset, the manual annotations for the labeled subset of the data, and the train/valid/test split used in the experiments.

The other notebooks can be used to train individual models with various levels of pretraining.
