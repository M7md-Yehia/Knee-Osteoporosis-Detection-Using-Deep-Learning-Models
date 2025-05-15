# Osteoporosis Diagnosis using Image-based Deep Learning and Tabular Machine Learning

---
## Project Overview
This repository contains two complementary projects aimed at osteoporosis classification:

1. **Image-based Classification:** Deep learning models trained on bone X-ray images.
2. **Tabular Data :** Machine learning models trained on structured patient data to predict osteoporosis.


---

## Dataset

### Image Dataset
The image dataset contains X-ray bone images classified into:
- Osteopenia
- Osteoporosis
- Normal

### Tabular Dataset
The tabular dataset contains structured patient clinical and demographic data, including the following features:

- Patient ID
- Joint Pain (presence or absence)
- Gender
- Age and Menopause Age
- Height (in meters) and Weight (in kilograms)
- Lifestyle factors: Smoking, Alcohol consumption
- Medical conditions: Diabetes, Hypothyroidism, Seizer Disorder
- Number of pregnancies
- Hormonal treatment: Estrogen Use
- Occupation
- History of fractures and dialysis
- Family history of osteoporosis
- Physical activity: Maximum walking distance (km)
- Daily eating habits
- General medical history
- Bone density scores: T-score and Z-score values
- Body Mass Index (BMI)
- Site of bone measurement
- Obesity status
- Final Diagnosis (Osteopenia, Osteoporosis, Normal)


### Tabular Data Analysis
Extensive data analysis was performed on the tabular dataset to prepare it for effective model training. This included:
- Data cleaning and handling missing values
- Exploratory Data Analysis (EDA) to understand feature distributions and relationships
- Feature engineering and selection to improve model performance
- Normalization and transformation of relevant variables


The file **The Final Patient Details.xlsx** represents the cleaned and fully processed tabular dataset obtained from the data analysis phase. This refined dataset comprises well-organized clinical and demographic features, optimized for training and evaluating machine learning models aimed at osteoporosis prediction.


This preprocessing ensured the tabular data was ready for training machine learning models such as Logistic Regression, Random Forest, and Support Vector Machine (SVM).


|X-ray Images||||Classification|
|----------------------|----------------------|----------------------|----------------------|----------------------|
|![Normal](https://github.com/user-attachments/assets/bdbe54bf-a7f7-45ef-acaa-f54e38c6f6ae)|![Normal](https://github.com/user-attachments/assets/73aef2e4-d48e-4948-b681-39e68e7318c5)|![Normal](https://github.com/user-attachments/assets/92c02e3f-e4bb-4539-a8d4-a22d0190c783)|![Normal](https://github.com/user-attachments/assets/9aa1826a-3e18-482e-9e67-a623b3112462)|Normal|
|![Osteopenia](https://github.com/user-attachments/assets/58838b3b-7d38-478b-8cbd-1df131fc9baf)|![Osteopenia](https://github.com/user-attachments/assets/5bbfb755-1fef-4c97-a125-8f4f1a1428fb)|![Osteopenia](https://github.com/user-attachments/assets/894b6af5-99f4-45ce-9512-7bc04c9e5501)|![Osteopenia](https://github.com/user-attachments/assets/ad5a447d-d298-4cbb-97ff-658bb94bdd55)|Osteopenia|
|![Osteoporosis](https://github.com/user-attachments/assets/7456a0cc-38d0-4f14-a176-f22cdf0a5d63)|![Osteoporosis](https://github.com/user-attachments/assets/adf9ab78-dc4f-4ad7-8a25-cac85940d70a)|![Osteoporosis](https://github.com/user-attachments/assets/e8f2773a-d0a4-4753-a55a-0c434aebbea2)|![Osteoporosis](https://github.com/user-attachments/assets/a450f36f-aced-4f55-82a1-85250a0ccc71)|Osteoporosis|

## Model Architecture
![Model Architecture of Osteoporosis Prediction](https://github.com/user-attachments/assets/f7380181-ab19-41bf-b6c5-f159761a6057)
---

## Models and Methods

### Image-based Models
- VGG16, VGG19, InceptionV3, ResNet50, MobileNetV2, DenseNet121
### Tabular Data Models
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)

---
    

Each model was trained with the same dataset and evaluated using precision, recall, f1-score, accuracy, and confusion matrices.
---
## Performance Metrics
Below is a summary of the classification performance for each model:









| Model       | Accuracy | Precision | Recall | F1-Score | Confusion Matrix | Graphs |
|------------|----------|------------|--------|----------|------------------|--------|
| **VGG16**  | 72%      | 0.75       | 0.72   | 0.71     | ![5f15d185-70a4-4e34-ac45-95b0939d3492](https://github.com/user-attachments/assets/4f808014-ab3d-4e37-9ea2-0b36220a999c) | ![8a87efd6-74b4-4f83-82ca-762092f8dfea](https://github.com/user-attachments/assets/a47708b3-65c8-4405-85f7-11e52428684e)
| **VGG19**  | 75%      | 0.69       | 0.67   | 0.66     | ![39902dcb-cefb-4dcd-aff8-42a0733d5ca4](https://github.com/user-attachments/assets/107c4901-9faa-4979-8c82-9808d9858191) | ![93d817c0-affe-4bcd-9c3a-42622beae5cc](https://github.com/user-attachments/assets/6a965aa0-fc88-4450-bf90-b1826c545eec) |
| **InceptionV3** | 73% | 0.74       | 0.73   | 0.73     | ![dcae6ac3-1910-459f-89f6-a4752655949a](https://github.com/user-attachments/assets/0d5b10ca-534a-4129-a6d1-4e2a61bf5c7f) | ![3a1cda72-a6df-4219-9fe4-4224d11d332f](https://github.com/user-attachments/assets/2905fbdb-d3da-419b-bf33-cde8358dd65b) |
| **ResNet50** | 63%   | 0.67       | 0.63   | 0.61     | ![f827cbb6-bb1d-4f7a-af5a-b5d712735c40](https://github.com/user-attachments/assets/53dc8890-7117-422b-857b-17229cd98ad7) | ![572ea5a1-43e2-48bd-838c-6f91f456e288](https://github.com/user-attachments/assets/cedb864b-5cc4-49db-b931-58acf8ae6162) |
| **MobileNetV2** | 70%   | 0.73       | 0.70   | 0.69     | ![f1a4ec5a-87b7-452b-9854-e2511fd90038](https://github.com/user-attachments/assets/770f8810-2690-4ef6-8c68-8e71582b4c44) | ![52908211-aed7-4f1e-90a6-c40e91223abc](https://github.com/user-attachments/assets/e2a045a7-c48f-4924-a836-7204ec79fc7b) |
| **DenseNwt121** | 67%    | 0.70       | 0.67   | 0.66     | ![5cdbe23e-2ede-4f4a-a0fa-84b21bbe2f3f](https://github.com/user-attachments/assets/6943ad3d-1610-444f-bf4c-0eee14821a09)|![6b78c1c5-183f-4d9b-95a4-8db5a4c99c4a](https://github.com/user-attachments/assets/9d2811db-766b-46ec-a578-8f09707f2345) |
| **Logistic regression**| 96%      | 0.98        | 0.91     | 0.94       |
| **Random Forest**| 92%      | 0.96        | 0.83     | 0.87       |![93f73d7f-36ea-427e-8887-fd35641e1982](https://github.com/user-attachments/assets/4ee578bb-8cba-45ee-a01f-3dc1dae70b93)

| **ANN**         | 83%      | 0.85       |  0.71    | .73      |




---
## Classification Reports
### **VGG16**
```
              precision    recall  f1-score   support

      Normal       0.89      0.49      0.63       180
  Osteopenia       0.77      0.87      0.82       180
Osteoporosis       0.60      0.79      0.68       180

    accuracy                           0.72       540
   macro avg       0.75      0.72      0.71       540
weighted avg       0.75      0.72      0.71       540
```

### **VGG19**
```
              precision    recall  f1-score   support

  Osteopenia       0.81      0.73      0.77        75
Osteoporosis       0.68      0.88      0.77       159
      Normal       0.85      0.63      0.73       156

    accuracy                           0.75       390
   macro avg       0.78      0.75      0.75       390
weighted avg       0.77      0.75      0.75       390
```

### **InceptionV3**
```
              precision    recall  f1-score   support

      Normal       0.84      0.59      0.69       180
  Osteopenia       0.74      0.86      0.79       180
Osteoporosis       0.65      0.73      0.69       180

    accuracy                           0.73       540
   macro avg       0.74      0.73      0.73       540
weighted avg       0.74      0.73      0.73       540
```

### **ResNet50**
```
              precision    recall  f1-score   support

      Normal       0.77      0.31      0.44       180
  Osteopenia       0.74      0.82      0.78       180
Osteoporosis       0.50      0.75      0.60       180

    accuracy                           0.63       540
   macro avg       0.67      0.63      0.61       540
weighted avg       0.67      0.63      0.61       540
```

### **MobileNetV2**
```
              precision    recall  f1-score   support

      Normal       0.85      0.48      0.61       180
  Osteopenia       0.76      0.84      0.80       180
Osteoporosis       0.58      0.77      0.66       180

    accuracy                           0.70       540
   macro avg       0.73      0.70      0.69       540
weighted avg       0.73      0.70      0.69       540

```

### **DenseNwt121**
```
              precision    recall  f1-score   support

      Normal       0.83      0.45      0.58       180
  Osteopenia       0.72      0.81      0.76       180
Osteoporosis       0.56      0.74      0.64       180

    accuracy                           0.67       540
   macro avg       0.70      0.67      0.66       540
weighted avg       0.70      0.67      0.66       540
```

### **Logisitc Reg**
---
                        precision    recall  f1-score   support

    normal       1.00      0.86      0.92         7
    osteopenia       0.94      1.00      0.97        33
    osteoporosis       1.00      0.88      0.93         8

              accuracy                           0.96        48
             macro avg       0.98      0.91      0.94        48
          weighted avg       0.96      0.96      0.96        48
---

### **Logisitc**
---

              precision    recall  f1-score   support

           0       1.00      0.60      0.75         5
           1       0.88      1.00      0.94        23
           2       1.00      0.88      0.93         8

    accuracy                           0.92        36
    macro avg      0.96      0.83      0.87        36
    weighted avg   0.93      0.92      0.91        36
---

    
## Confusion Matrices & Graphs
Each model has an associated **confusion matrix** and **performance graphs** showcasing:
- **Training & Validation Accuracy**
- **Training & Validation Loss**
- **Comparative Model Performance**
---
## Conclusion
This project shows how we can use both X-ray images and patient data to detect osteoporosis. The deep learning models work well with the images, and the machine learning models use the patient info to help make better predictions.
By combining both approaches, we get a stronger, more accurate way to diagnose osteoporosis. This could help doctors make faster and more reliable decisions in the future.
---
## Authors
- **[Mohamed Yehia Youssef](https://www.linkedin.com/in/mohamed-yehia-4593792aa/)** - AI/ML Researcher
- **[Nezar Emad ELdin](https://www.linkedin.com/in/nezar-emad-eldin/)** - AI/ML Researcher

---
This project was developed as part of an ongoing research initiative in medical diagnosis combining medical image classification using deep learning and tabular data with machine learning.

