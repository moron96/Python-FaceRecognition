# Face Authenication System
cloned from [Building a face recognition system with FaceNet](https://medium.com/@athul929/building-a-facial-recognition-system-with-facenet-b9c249c2388a)
This is a TensorFlow implementation of the face recognizer described in the paper ["FaceNet: A Unified Embedding for Face Recognition and Clustering"](http://arxiv.org/abs/1503.03832).


## Pre-trained models
| Model name      | LFW accuracy | Training dataset | Architecture |
|-----------------|--------------|------------------|-------------|
| [20180408-102900](https://drive.google.com/open?id=1R77HmFADxe87GmoLwzfgMu_HY0IhcyBz) | 0.9905        | CASIA-WebFace    | [Inception ResNet v1](https://github.com/davidsandberg/facenet/blob/master/src/models/inception_resnet_v1.py) |
| [20180402-114759](https://drive.google.com/open?id=1EXPBSXwTaqrSC0OhUdXNmKSh9qJUQ55-) | 0.9965        | VGGFace2      | [Inception ResNet v1](https://github.com/davidsandberg/facenet/blob/master/src/models/inception_resnet_v1.py) |

NOTE: If you use any of the models, please do not forget to give proper credit to those providing the training dataset as well.


## Compatibility
See and run setup.py


## How To Run
1. Populate ./src/photos folder with your data
2. Run ./facenet/src/classifier.py with param `TRAIN <path to your photos> <path to your models> classifier.pk`
3. Move ./facenet/src/classifier.pk to ./src/
4. Run ./src/main.py