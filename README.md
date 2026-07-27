SMARTER NER

Fine-Grained Telugu Named Entity Recognition using Semi-Supervised Learning and Explainable AI

Overview

SMARTER NER is a Natural Language Processing (NLP) project designed to recognize named entities from Telugu text, which is a low-resource language. The project uses a hybrid approach that combines manual annotation and semi-supervised learning to improve entity recognition accuracy. A spaCy-based NER model is trained using labeled data and further enhanced through pseudo-labeling, dataset refinement, and retraining. Explainable AI (LIME) is integrated to make the model's predictions transparent and interpretable. A Streamlit-based web application allows users to enter Telugu text and view recognized entities in real time. 



Problem Statement

Most existing Named Entity Recognition (NER) systems are developed for high-resource languages such as English, where large annotated datasets are available. Telugu, being a low-resource language, has limited labeled data, which affects the performance of traditional NER models. Existing systems mainly rely on supervised learning, requiring extensive manual annotation, which is time-consuming and expensive. Additionally, they lack explainability, making it difficult to understand how predictions are generated. SMARTTER NER addresses these challenges using semi-supervised learning and Explainable AI. 


Objectives

* Develop a Named Entity Recognition (NER) system for the Telugu language.
* Improve NER performance using Semi-Supervised Learning.
* Enhance model accuracy through pseudo-labeling, dataset refinement, and retraining.
* Provide explainability using LIME.
* Build a user-friendly Streamlit web application.
* Accurately identify entities such as Person, Location, Organization, and Miscellaneous. 


Key Features

* Telugu Named Entity Recognition.
* Hybrid learning using manual annotation and semi-supervised learning.
* Pseudo-label generation for unlabeled data.
* Dataset refinement to improve prediction quality.
* Model retraining for better accuracy.
* Explainable AI using LIME.
* Streamlit-based interactive web application.
* Real-time entity recognition and visualization.
* Supports Person, Location, Organization, and Miscellaneous entity detection.  


Methodology

1. **Manual Annotation:** A small Telugu dataset is manually labeled with entity categories such as Person, Location, Organization, and Miscellaneous.

2. **Model Training:** A spaCy-based NER model is trained using the manually annotated dataset.

3. **Pseudo-Labeling:** The trained model predicts labels for a larger unlabeled Telugu dataset.

4. **Dataset Refinement:** Low-quality pseudo-labeled data is filtered to improve the dataset quality.

5. **Model Retraining:** The refined dataset is combined with labeled data to retrain the model and improve performance.

6. **Explainable AI:** LIME is integrated to explain the model's predictions.

7. **Deployment:** The trained model is deployed through a Streamlit web application for real-time Telugu text analysis. 


System Architecture

The SMARTTER NER system follows a sequential workflow. Telugu text entered by the user is first preprocessed. The preprocessed text is then passed to the spaCy-based NER model, which has been trained using manually annotated data and improved through pseudo-labeling and dataset refinement. The model identifies named entities such as Person, Location, Organization, and Miscellaneous. LIME is then used to explain the model's predictions, and the final results are displayed through a Streamlit web interface with entity visualization.  


Tech Stack

| Category             | Technology               |   |
| -------------------- | ------------------------ | - |
| Programming Language | Python 3.8               |   |
| NLP Library          | spaCy                    |   |
| Machine Learning     | Semi-Supervised Learning |   |
| Explainable AI       | LIME                     |   |
| Web Framework        | Streamlit                |   |
| Visualization        | spaCy Displacy           |   |
| IDE                  | Visual Studio Code       |   |
| Version Control      | Git & GitHub             |   |
| Operating System     | Windows 7 or above       |   |


Project Structure

```text
SMARTTER-NER/
│
├── dataset/
├── preprocessing/
├── models/
├── training/
├── pseudo_labeling/
├── refinement/
├── explainability/
├── app.py
├── requirements.txt
├── README.md
└── LICENSE

## 9. Installation and Setup

### Clone the Repository

```bash
git clone https://github.com/yourusername/SMARTTER-NER.git
```

### Navigate to the Project Folder

```bash
cd SMARTTER-NER
```

### Create a Virtual Environment

```bash
python -m venv venv
```

### Activate the Virtual Environment (Windows)

```bash
venv\Scripts\activate
```

### Install Required Packages

```bash
pip install -r requirements.txt
```

### Run the Application

```bash
streamlit run app.py
```

Model Performance

The SMARTTER NER model improves entity recognition by combining manually labeled data with pseudo-labeled data through Semi-Supervised Learning. Dataset refinement removes low-quality predictions, increasing the overall reliability of the model. LIME provides explanations for model predictions, making the system transparent and interpretable. The presentation does not provide numerical evaluation metrics such as Accuracy, Precision, Recall, or F1-score. 


Feature Enhancements

* Support additional fine-grained entity types such as Events, Products, and Numerical Expressions.
* Integrate cross-lingual learning with related Indian languages.
* Enhance explainability using SHAP.
* Develop real-time applications such as chatbots and virtual assistants.
* Extend support to multiple low-resource Indian languages.
* Build more scalable and accurate NER systems. 


Contributors

**Project Guide**

* Dr. V. Venkateshwara Rao

**Team Members**

* CH. Yasaswi
* P. Geetha Rani Sri
* G. Sri Naga Sirisha
* R. J. S. Raju
* C. Nandiraju 


License

This project was developed for academic and research purposes as part of the Bachelor of Technology curriculum. It is intended for educational and research use in Natural Language Processing for low-resource languages. If released as an open-source project, it can be licensed under the MIT License to allow reuse, modification, and distribution with proper attribution.

