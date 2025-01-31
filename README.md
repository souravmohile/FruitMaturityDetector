# Fruit Maturity Detection Project

This project is a deep learning-based application for **fruit classification** using a **pretrained VGG16 model**. The model classifies fruits into 15 categories and includes real-time classification via a webcam feed. This project was made as my **undergraduate final year project**.

---

## Features
1. **Pretrained VGG16 Transfer Learning**:
   - The VGG16 model is used without the top layers, and custom layers are added for a 15-class classification task.
   - The model is trained using data augmentation to improve generalization.

2. **Real-Time Classification**:
   - Classifies fruits in real time using a webcam.
  
3. **Uploaded Image Classification**:
   - Additionally, you can opt to upload a single image of the fruit to classify it.

---

## Files

1. **train.py**
  - Loads the pretrained VGG16 model without its top layers.
  - Freezes the pretrained layers to retain the learned features.
  - Dropout layers reduce overfitting and improve generalisation
  - Adds custom dense layers for a 15-class classification task.
  - Trains the model using data augmentation (ImageDataGenerator).
    
2. **inference.py**
  - Loads the trained fruit_classifier.h5 model.
  - Uses OpenCV to access the webcam feed.
  - Preprocesses each frame for VGG16 input requirements.
  - Predicts the fruit class and displays the label.

---

## Future work

1. Using visual transformers for classification
2. Comparing results from visual transformers and CNNs
3. Improve the dataset with better samples

---

You can view some real-time predictions from the model in the folder - "sample predictions"
