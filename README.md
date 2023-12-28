# Eczema Detection using three model stages:
Three stage detection of eczema
This program uses 3 stages/ models:
1. Human Skin Detection model : if passed image is of human skin or not
2. Eczema detection model: if passed image of human skin has eczema or not
3. Eczema classification model: the level of eczema (mild, moderate, severe)

Pre-trained model used: [a link](https://www.kaggle.com/models/google/mobilenet-v2/frameworks/TensorFlow2/variations/140-224-feature-vector/versions/2)
This pre-trained model "mobilenet-v2" has been retrained using new dataset and a single dense layer for each case.


Dataset:
The eczema dataset was downloaded from: https://www.kaggle.com/datasets/shubhamgoel27/dermnet
