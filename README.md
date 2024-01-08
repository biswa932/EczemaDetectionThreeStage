# Eczema Detection using 3 CNN model stages:
Three stage detection of eczema
This program uses 3 stages/ models:
1. Human Skin Detection model : if passed image is of human skin or not
2. Eczema detection model: if passed image of human skin has eczema or not
3. Eczema classification model: the level of eczema (mild, moderate, severe)

# Pre-trained model used: 
https://www.kaggle.com/models/google/mobilenet-v2/frameworks/TensorFlow2/variations/140-224-feature-vector/versions/2

This pre-trained model "mobilenet-v2" has been retrained using new dataset and a single dense layer for each case.


# Eczema images Dataset:
The eczema dataset was downloaded from: https://www.kaggle.com/datasets/shubhamgoel27/dermnet

# Dataset structure: dataset/eczema_photos
    1. allSkin: 2612 items
    2. clearSkin: 1204 items
    3. eczema: 1408 items
    4. invalid: 2400 items
    5. mild: 393
    6. moderate: 641
    7. severe: 373

# Accuracy:
1. Human Skin Detection model : Training(loss: 0.0086 - acc: 0.9995), Evaluation(loss: 0.0225 - acc: 0.9935)
2. Eczema detection model: Training(loss: 0.0690 - acc: 0.9752), Evaluation(loss: 0.0823 - acc: 0.9674)
3. Eczema classification model: Training(loss: 0.3653 - acc: 0.9041), Evaluation(loss: 0.7293 - acc: 0.6667)

# All the models were converted to CoreML (*.mlmodel) using Colab.

1. Code: ThreeStageEczemaDetection.ipynb
2. CoreML convertion: ThreeStageEczemaDetectionToCoreML.ipynb
