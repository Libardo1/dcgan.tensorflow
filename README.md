# Deep Convolutional Generative Adversarial Networks with TensorFlow
##  implementation based on http://arxiv.org/abs/1511.06434
  "Unsupervised Representation Learning with
  Deep Convolutional Generative Adversarial Networks",
  Alec Radford, Luke Metz and Soumith Chintala

## Author
  Il Gu Yi

## Requirements
* TensorFlow rc1.0-alpha (didn't check 1.0 version)
* opencv (for generate.py)

## Training
### dataset download (celebA_tfrecords.zip)
* [celebA tfrecords](https://www.dropbox.com/s/vd0nuybgvo9uvx0/celebA_tfrecords.zip?dl=1)
    
### editing dcgan_train.sh
* Set the "WORKING_DIR path" to path you want
* Set the dataset path or move to where dcgan/datasets/celebA/tfrecords
* Set the hyper-parameters

### run ./dcgan_train.sh
```shell
$ ./dcgan_train.sh
```
* You can use tensorboard for monitoring loss and generated images
```shell
$ tensorboard --logdir=exp1
```

## Generating images
```shell
$ ./generate.sh batch_size (the number of images you want)
```
