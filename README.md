# Business-Automation-Ltd-Assesment-task Resume Categorization Model

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
**Objective:** Convert preprocessed text into a numerical format that can be used by the machine learning model.

**Method used:** TF-IDF Vectorization, which measures the originality of a word by comparing the number of times a word appears in a document with the number of documents the word appears in. This helps in accentuating important words and downplaying common words across documents.

## 4. Model Selection and Training
**Objective:** Train a machine learning model to categorize resumes into domains.

**Chosen Model:** RandomForest Classifier. The rationale for this choice includes its robustness to high dimensional data, general high performance and effective management of bias and variance, and its ability to provide insights on feature importance.

## 5. Evaluation
**Objective:** Assess the performance of the trained model.

**Evaluation Methods:**
- Using a confusion matrix to visualize performance.
- A classification report to provide precision, recall, and F1-score metrics for each category.

## 6. Deployment
**Objective:** Deploy the trained model to categorize new resumes.

**Instructions:**
- Ensure all dependencies are installed.
- Load the trained model.
- Input the directory path of new resumes.
- Run the script to categorize resumes and save the results.

**Expected Outputs:**
- Categorized resumes sorted into domain-specific folders.
- A summary CSV file named 'categorized_resumes.csv' containing resume identifiers and their predicted categories.
