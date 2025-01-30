# Cat vs Dog Image Classifier 🐱🐶  

This repository contains a machine learning project that uses the **VGG16 model** (pre-trained on ImageNet) to classify images of cats and dogs. The model has been fine-tuned to adapt to the binary classification task and achieve high accuracy.  

---

## Overview  

### **Model**  
We use **VGG16**, a deep Convolutional Neural Network (CNN), as the base model. VGG16 is well-known for its effectiveness in image classification tasks and has been pre-trained on the large-scale ImageNet dataset.  
- **Transfer Learning**: We leverage the pre-trained weights of VGG16 to extract useful features.  
- **Custom Top Layers**: Additional layers were added for binary classification (cat vs. dog).  
- **Fine-tuning**: The model's deeper layers were partially unfrozen and fine-tuned for better performance on this specific dataset.  

---

### **Dataset**  
The dataset is organized into two main folders, one for training and one for testing, each containing subfolders for the two classes:  
- **Training Folder**:  
  - `/train/cat/` – Contains training images of cats.  
  - `/train/dog/` – Contains training images of dogs.  
- **Testing Folder**:  
  - `/test/cat/` – Contains testing images of cats.  
  - `/test/dog/` – Contains testing images of dogs.  

The images are resized to **224x224** pixels before being fed into the model. Data augmentation techniques such as rotations, flips, and zooming are applied to the training data to improve generalization.
