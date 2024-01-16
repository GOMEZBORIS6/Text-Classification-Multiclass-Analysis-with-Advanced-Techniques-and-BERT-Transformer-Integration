# Text-Classification-Multiclass-Analysis-with-Advanced-Techniques-and-BERT-Transformer-Integration

<img src="E_commerce_classification.png" style="width:100%; height: 400px">

**Overview:**

The primary goal of this project is to categorize e-commerce products into four distinct groups: `Electronics`, `Household`, `Books`, and `Clothing & Accessories`, based on their descriptions available on various e-commerce platforms. The key steps undertaken in this notebook include:

1. Conducted basic **Exploratory Data Analysis**, comparing the distributions of character count, word count, and average word length in product descriptions across different categories.

2. Applied various **text normalization techniques** to enhance the consistency of product descriptions.

3. Utilized **TF-IDF vectorization** on the normalized product descriptions for effective text representation. The baseline performance of several classifiers was compared, and hyperparameter tuning was executed specifically on **SVM Classifier**.

4. Explored an alternative approach by implementing selected text normalization processes, such as converting to lowercase and substituting contractions directly on the raw data of product descriptions. Employed Google's pre-trained **Word2Vec model** on tokens derived from partially normalized descriptions, generating embeddings subsequently converted to compressed sparse row (CSR) format. Baseline performance of various classifiers was assessed, and hyperparameter tuning was conducted on the **XGBoost classifier**.

5. Applied the model with the highest validation accuracy to predict labels for test observations, achieving a notable test accuracy of **0.950378**.

6. Utilized the **Google [BERT](https://github.com/google-research/bert)(Bidirectional Encoder Representations from Transformers)** model through the **Hugging Face Transformers library** in our project. Following the modeling phase and fine-tuning of the model, we achieved an impressive test accuracy, specifically **0.957569.**

**About Dataset**

This is the classification based E-commerce text dataset for **4 categories** - `Electronics`, `Household`, `Books` and `Clothing & Accessories`, which almost cover **80%** of any E-commerce website.

The dataset is in `.csv` format with two columns - the first column is the class name and the second one is the datapoint of that class. The data point is the product and description from the e-commerce website.

The dataset has the following features :

**Data Set Characteristics:** Multivariate

**Number of Instances:** 50425

**Number of classes:** 4

**Area:** Computer science

**Attribute Characteristics:** Real

**Number of Attributes:** 1

**Associated Tasks:** Classification

**Missing Values?** No

Gautam. (2019). E commerce text dataset (version - 2) [Data set]. [Zenodo](https://doi.org/10.5281/zenodo.3355823).
