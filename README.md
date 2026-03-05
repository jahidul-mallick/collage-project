# Classification of Online Toxic Comments Using Machine Learning Algorithms

## Project Overview

Online platforms such as forums, social media, and discussion boards often contain toxic comments that may include insults, threats, hate speech, or abusive language. Detecting and filtering such comments is important for maintaining healthy online communities.

This project implements a **machine learning based system to automatically classify toxic comments** using multiple classification algorithms. The application provides a **graphical user interface (GUI)** built using **Tkinter** and applies several machine learning models to classify comments into different toxicity categories.

The system performs **text preprocessing, feature extraction using TF-IDF, model training, evaluation, and prediction** of toxic comments.

---

## Objectives

- Detect and classify toxic comments automatically.
- Compare multiple machine learning algorithms for toxicity detection.
- Provide a GUI interface to upload datasets, train models, and predict toxicity.
- Evaluate models using **Accuracy** and **Hamming Loss**.

---

## Toxic Comment Categories

The dataset labels comments into six toxicity classes:

1. **Toxic**
2. **Severe Toxic**
3. **Obscene**
4. **Threat**
5. **Insult**
6. **Identity Hate**

Each comment may belong to one or more categories.

---

## Machine Learning Algorithms Used

The project evaluates the performance of the following classification algorithms:

- Support Vector Machine (SVM)
- Logistic Regression
- Naive Bayes
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)

Each algorithm is trained separately for all toxicity categories.

---

## System Architecture

The workflow of the system is as follows:

```

Dataset Upload
↓
Text Preprocessing
↓
Tokenization & Lemmatization
↓
Stopword Removal
↓
TF-IDF Feature Extraction
↓
Train/Test Split
↓
Model Training
↓
Model Evaluation
↓
Prediction on New Comments
↓
Performance Visualization

```

---

## Technologies Used

| Technology | Purpose |
|------------|--------|
| Python | Core programming language |
| Tkinter | GUI development |
| Pandas | Dataset processing |
| NumPy | Numerical computations |
| NLTK | Text preprocessing |
| Scikit-learn | Machine learning algorithms |
| Matplotlib | Graph visualization |

---

## Libraries Used

The project uses the following Python libraries:

```

tkinter
pandas
numpy
nltk
scikit-learn
matplotlib

```

Install dependencies using:

```

pip install pandas numpy nltk scikit-learn matplotlib

```

Download required NLTK resources:

```

import nltk
nltk.download('stopwords')
nltk.download('wordnet')

```

---

## Dataset

The dataset used contains toxic comments with labeled categories.

Example columns in the dataset:

```

comment_text
toxic
severe_toxic
obscene
threat
insult
identity_hate

```

Each row contains a comment and binary labels indicating toxicity types.

---

## Text Preprocessing

Before training the models, the text data undergoes several preprocessing steps:

1. Convert text to lowercase
2. Remove punctuation
3. Remove stopwords
4. Remove non-alphabetic words
5. Lemmatization
6. Tokenization

This improves the quality of features used for machine learning.

---

## Feature Extraction

The system uses **TF-IDF (Term Frequency - Inverse Document Frequency)** to convert text into numerical feature vectors.

Advantages of TF-IDF:

- Captures word importance
- Reduces influence of common words
- Improves classification performance

---

## Model Evaluation Metrics

The models are evaluated using:

### 1. Accuracy
Measures how many predictions are correct.

```

Accuracy = Correct Predictions / Total Predictions

```

### 2. Hamming Loss
Measures the fraction of incorrectly predicted labels.

```

Hamming Loss = Incorrect Labels / Total Labels

```

Lower Hamming Loss indicates better performance.

---

## Application Features

The GUI application provides the following features:

### Upload Dataset
Allows the user to load a toxic comment dataset.

### Preprocess Dataset
Cleans and processes the text data.

### Apply TF-IDF Vectorization
Converts comments into numerical feature vectors.

### Train Machine Learning Models
Runs the following models:

- SVM
- Logistic Regression
- Naive Bayes
- Decision Tree
- Random Forest
- KNN

### Accuracy Comparison
Displays a bar graph comparing the performance of all algorithms.

### Toxic Comment Prediction
Allows testing new comments and predicts whether they are toxic.

---

## GUI Interface

The application interface includes the following controls:

- Upload Toxic Comments Dataset
- Preprocess Dataset
- Apply Count Vectorizer (TF-IDF)
- Run SVM Algorithm
- Run Logistic Regression
- Run Naive Bayes
- Run Decision Tree
- Run Random Forest
- Run KNN
- Accuracy Comparison Graph
- Predict Toxic Comments

Results are displayed in the output panel.

---

## How to Run the Project

### Step 1: Clone or Download the Project

```

git clone <repository_url>

```

or download the project files manually.

---

### Step 2: Install Dependencies

```

pip install pandas numpy nltk scikit-learn matplotlib

```

---

### Step 3: Download NLTK Resources

Run once in Python:

```

import nltk
nltk.download('stopwords')
nltk.download('wordnet')

```

---

### Step 4: Run the Application

```

python main.py

```

---

### Step 5: Use the GUI

1. Upload dataset
2. Preprocess dataset
3. Apply TF-IDF vectorizer
4. Train models
5. Compare accuracy
6. Test prediction on new comments

---

## Sample Output

The system outputs:

- Model accuracy
- Hamming loss
- Graph comparison of algorithms
- Prediction of toxic comments

Example prediction output:

```

You are stupid and useless
[CONTAINS INSULT COMMENTS]

```

---

## Advantages of the System

- Automated toxic comment detection
- Multiple algorithm comparison
- Interactive GUI interface
- Real-time prediction capability
- Visual model performance comparison

---

## Limitations

- Dataset size is limited
- Models may not detect context or sarcasm
- Requires labeled training data
- Performance depends on preprocessing quality

---

## Future Improvements

- Use deep learning models (LSTM, BERT)
- Deploy as a web application
- Use larger datasets
- Improve multi-label classification
- Integrate real-time moderation APIs

---

## Conclusion

This project demonstrates how machine learning can be applied to automatically classify toxic comments in online platforms. By comparing several algorithms, the system helps identify which model performs best for toxicity detection. The GUI interface makes the system easy to use for dataset analysis and prediction.

---

## Author

College Project – Toxic Comment Classification Using Machine Learning
