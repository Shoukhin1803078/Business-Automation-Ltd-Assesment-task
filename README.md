# Business-Automation-Ltd-Assesment-task Resume Categorization Model Implement

## 1. Overview
The goal of this project is to automatically categorize resumes into different domains (e.g., IT, Marketing, Finance) based on their content. This helps in streamlining the recruitment process by allowing for quick sorting and better matching of candidates to job openings.

## 2. Data Preprocessing
Here I use some methods include loading data
- Text cleaning through tokenization
-	Lowercasing
-	Stopword removal
-	Non-alphanumeric removal.
  
These steps help me to prepare the text data by reducing noise and focusing on relevant words.



## 3. Feature Extraction
For feature extraction I used is TF-IDF Vectorization, which measures the originality of a word by comparing the number of times a word appears in a document with the number of documents the word appears in. This helps in accentuating important words and downplaying common words across documents.

## 4. Model Selection and Training

**Chosen Model:** RandomForest Classifier. 
I chosen RandomForest Classifier Model. I think for this dataset RandomForest Classifier is more suitable than another model because  its robustness to high dimensional data, general high performance and effective management of bias and variance and its ability to provide insights on feature importance. Here I mention some point why I choose it:
-	Robustness: It can handles high dimensional data well and is less likely to overfit compared to other algorithms.
-	Performance: It provides high accuracy and handles the balance between bias and variance effectively.
-	Feature Importance:  This classifer offers good insights into which features are most influencing the predictions, which is valuable for text data.

These are the main reason for choosing this classifier.
I use train validation and test ratio is 80% : 10% : 10%

For visualization of precision, recall, and F1-score metrics for each category,
Here is the classification report:
![Screenshot (57)](https://github.com/user-attachments/assets/f2779cfd-001a-42c1-a7ee-eda61dd1131a)



## 5. Result analysis and Evaluation
For evaluation here I give confusion matrix, ROC curve and feature importance curve etc. 
**Confusion Matrix:**
![Screenshot (58)](https://github.com/user-attachments/assets/b9d153b2-679b-4f03-a9f3-84ff0541b5a2)
**Feature Importance curve:**
![Screenshot (59)](https://github.com/user-attachments/assets/9fe78fcd-6186-4f96-a21b-bcb906895a54)
**ROC curve:**
![Screenshot (61)](https://github.com/user-attachments/assets/1cca978f-5fd5-46b8-9e1e-bb4de06f0add)

## 6. Deployment
I uploaded the dataset into my drive (publicly accessable). I do all code in google colab . If you want to run the whole code please go to this link where I put my code:
https://colab.research.google.com/drive/1Bn0UI92yi-KXCJvrw-McXieZeVlBGClc?usp=sharing
