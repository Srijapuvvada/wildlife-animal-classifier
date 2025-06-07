# Wildlife Animal & Habitat Classification 

##  Project Objective

Build a deep learning model to classify wildlife animal images into 6 categories and predict their natural habitat.  
This project demonstrates the power of Transfer Learning in real-world image classification tasks.

##  Example Predictions

| Image | Predicted Animal | Habitat | Confidence |
|-------|------------------|---------|------------|
|  fox.png | Fox | Forest | 97.3% |
|  cheetah.png | Cheetah | Grasslands | 95.2% |
|  wolf.png | Wolf | Tundra | 96.8% |

##  Project Pipeline

1 **Dataset Preparation**  
- Images organized by class  
- Corrupted images removed  
- Dataset split: 70% training, 15% validation, 15% testing  

2️ **Data Augmentation & Loading**  
- Real-time augmentation applied to training set  
- Standard resizing to 224x224 pixels  

3️ **Model Building (Transfer Learning)**  
- Pre-trained CNN base:
    - MobileNetV2
    - EfficientNetB0
    - ResNet50V2  
- Added custom dense layers  
- Softmax output for 6 animal classes  

4️ **Training**  
- Optimizer: Adam  
- Loss: Sparse Categorical Crossentropy  
- Callbacks: ModelCheckpoint, ReduceLROnPlateau, EarlyStopping  

5️ **Evaluation**  
- Test accuracy reported  
- Classification report generated  
- Confusion matrix plotted  

6️ **Predictions**  
- Test images used to predict:
    - Animal class  
    - Corresponding habitat  
    - Model confidence  

##  Classes & Habitat Mapping

| Animal | Habitat |
|--------|---------|
| Lion   | Savannah |
| Tiger  | Rainforest |
| Cheetah| Grasslands |
| Fox    | Forests |
| Wolf   | Tundra |
| Hyena  | Savannah |

##  Tools & Libraries

- **Python**
- **TensorFlow / Keras**
- **OpenCV**
- **Matplotlib / Seaborn**
- **NumPy**
- **scikit-learn**
- **splitfolders**

##  Results

- Achieved **XX% test accuracy** (update after training)
- Good generalization on unseen test images
- Habitat prediction aligned with biological mappings

##  Future Work

- Expand to more animal classes and habitats
- Fine-tune deeper layers of pre-trained models
- Build a web/mobile app to deploy the model
- Add habitat prediction as a separate multi-label classification task

##  Contributions

This project was built as part of my **AI/Deep Learning learning journey**.  
Feel free to fork, star , and contribute!

---

