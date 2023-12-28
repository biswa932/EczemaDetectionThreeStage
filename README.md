# Eczema Detection using three model stages:
Three stage detection of eczema
This program uses 3 stages/ models:
1. Human Skin Detection model : if passed image is of human skin or not
2. Eczema detection model: if passed image of human skin has eczema or not
3. Eczema classification model: the level of eczema (mild, moderate, severe)

Pre-trained model used: https://www.kaggle.com/models/google/mobilenet-v2/frameworks/TensorFlow2/variations/140-224-feature-vector/versions/2
This pre-trained model "mobilenet-v2" has been retrained using new dataset and a single dense layer for each case.


Eczema images Dataset:
The eczema dataset was downloaded from: https://www.kaggle.com/datasets/shubhamgoel27/dermnet

Dataset structure:
dataset
  eczema_photos
    allSkin: 2428 items
    clearSkin: 1204 items
    eczema: 1224 items
    invalid: 2400 items
    mild: 351
    moderate: 566
    severe: 307

Accuracy:
1. Human Skin Detection model : Training(loss: 0.0083 - acc: 0.9997), Evaluation(loss: 0.0149 - acc: 0.9949)
2. Eczema detection model: Training(loss: 0.0116 - acc: 0.9994), Evaluation(loss: 0.0145 - acc: 0.9933)
3. Eczema classification model: Training(loss: 0.3640 - acc: 0.8998), Evaluation(loss: 0.8092 - acc: 0.6144)

System specification:
OS: Windows 11
AMD Ryzen 5 5600G with Radeon Graphics
RAM: 16.0 GB

All the models were converted to CoreML (*.mlmodel) using "Colab" due to Core ML installation issues on Windows.
