# LW3_Custom-Image-Classifier

## Google Colab Link: https://colab.research.google.com/drive/18O5egTCVrzEfVBU-Gz__i75G5BSXFM7I?usp=sharing

--- 

# Activity 3 — Building a Custom Image Classifier with TensorFlow Using Personal Image Datasets from Google Drive

## Guide Questions (Student Reflection & Explanation)

### 1. Dataset Preparation

### How did you organize your dataset in Google Drive? 

I organized my dataset in Google Drive by creating separate folders for each class or category of images. Each folder contained images belonging to a specific label (e.g., “Class A,” “Class B,” etc.). This structure made it easier for TensorFlow to automatically assign labels during data loading.

### Why is folder structure important for TensorFlow image loading?

The folder structure is important because TensorFlow uses it to identify and label images correctly. When using functions like image_dataset_from_directory, the folder names serve as class labels. Without proper organization, the model may misclassify images or fail to load the dataset properly.

---

### 2. Model Training

### What is the role of convolutional layers in image classification?  

Convolutional layers play a crucial role in image classification by extracting important features from images such as edges, textures, and shapes. These layers help the model understand visual patterns and hierarchies in the data. 

### Why do we split data into training and validation sets?  

We split the dataset into training and validation sets to evaluate the model’s performance. The training set is used to teach the model, while the validation set is used to test how well the model generalizes to unseen data. This helps prevent overfitting and ensures reliable performance.

---

### 3. Performance Analysis

### What accuracy did your model achieve?  

The model achieved an accuracy of approximately (insert your actual accuracy here, e.g., 85%) on the validation dataset. 

### How did the number of images affect the model’s performance?  

The number of images significantly affected the model’s performance. A larger dataset improved accuracy and generalization, while a smaller dataset led to lower accuracy and increased chances of overfitting.

---

### 4. Critical Thinking

### What challenges did you encounter while using your own dataset?  

One challenge I encountered when using my own dataset was inconsistency in image quality, size, and lighting conditions. Additionally, having a limited number of images made it difficult for the model to generalize well.

### How can data augmentation improve your model? 

Data augmentation improves the model by artificially increasing the diversity of the dataset. Techniques such as rotation, flipping, and zooming help the model learn different variations of the same image, making it more robust and accurate.

---

### 5. Application

### Suggest a real-world application for your trained model.  

A real-world application of this model could be an object recognition system, such as identifying recyclable materials, plants, or products.

### How can this system be integrated into a mobile or web application?  

This system can be integrated into a mobile or web application by converting the trained model into a deployable format (e.g., TensorFlow Lite for mobile or TensorFlow.js for web). The app can then use the device camera to capture images and classify them in real time. 

---

# Activity 3A: Improving and Evaluating a Custom Image Classifier

## Guide Questions (Student Explanation & Reflection)

### Visualization & Overfitting

1. What signs indicated overfitting in your first model?

Signs of overfitting in the first model included high training accuracy but low validation accuracy, as well as a large gap between training and validation loss.
    
2. How did data augmentation affect validation accuracy?

Data augmentation improved validation accuracy by exposing the model to more varied data, reducing overfitting and improving generalization.

---

### Model Improvement

3. What is the purpose of dropout layers?

Dropout layers are used to randomly deactivate some neurons during training. This prevents the model from becoming too dependent on specific features and reduces overfitting.

4. Why does data augmentation improve generalization?

Data augmentation improves generalization by providing more diverse training examples, allowing the model to perform better on unseen data.

---

### Performance Comparison

5. Compare accuracy before and after improvements.

Before improvements, the model had lower validation accuracy (e.g., around 70%). After applying techniques like data augmentation and dropout, the accuracy improved (e.g., up to 85%).

6. Which technique contributed most to improvement?

Data augmentation contributed the most to improvement because it effectively increased the dataset size and variability.

---

### Deployment & Application

7. Why is saving the model important?

Saving the model is important so it can be reused without retraining. It allows deployment in applications and ensures consistency in predictions.

8. How can this model be deployed in a real-world system?  

The model can be deployed in real-world systems by integrating it into applications such as mobile apps, websites, or embedded systems. For example, it can be used in a mobile app that scans objects and provides instant classification results.





