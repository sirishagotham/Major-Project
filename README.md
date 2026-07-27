SMARTER NER
Fine-Grained Telugu Named Entity Recognition using Semi-Supervised Learning and Explainable AI
 Overview

SMARTER NER is a Natural Language Processing (NLP) project developed to recognize named entities from Telugu text, a low-resource language. The project uses a hybrid approach that combines manual annotation and semi-supervised learning to improve entity recognition accuracy. A spaCy-based Named Entity Recognition model is initially trained on labeled data and further enhanced through pseudo-labeling, dataset refinement, and retraining. To improve transparency, Explainable AI using LIME is integrated, allowing users to understand why the model predicts particular entities. A Streamlit-based web application provides a simple interface for real-time Telugu text analysis and visualization of detected entities.

 Problem Statement

Most existing Named Entity Recognition systems are designed for high-resource languages such as English, where large annotated datasets are available. However, Telugu is a low-resource language with limited labeled data, making it difficult to build accurate NER models. Existing systems mainly depend on supervised learning, which requires extensive manual annotation and is both time-consuming and expensive. Furthermore, most NER systems do not provide explanations for their predictions, making them less transparent and difficult to interpret. SMARTER NER addresses these challenges using semi-supervised learning and Explainable AI.

 Objectives
Develop a Named Entity Recognition (NER) system for the Telugu language.
Improve NER performance in low-resource environments using Semi-Supervised Learning.
Increase model accuracy through pseudo-labeling, dataset refinement, and retraining.
Integrate Explainable AI (LIME) to make predictions transparent and interpretable.
Build a user-friendly Streamlit application for real-time entity recognition.
Accurately identify entities such as Person, Location, Organization, and Miscellaneous.
 Key Features
Telugu Named Entity Recognition
Hybrid Learning Approach (Manual Annotation + Semi-Supervised Learning)
Pseudo-label Generation
Dataset Refinement
Model Retraining
Explainable AI using LIME
Real-time Web Application using Streamlit
Entity Visualization
Accurate identification of Person, Location, Organization, and Miscellaneous entities
 Methodology
Step 1: Manual Annotation

A small Telugu dataset is manually annotated with entity labels such as Person, Location, Organization, and Miscellaneous.

Step 2: Model Training

A spaCy-based Named Entity Recognition model is trained using the manually labeled dataset.

Step 3: Pseudo-Labeling

The trained model predicts labels for a large unlabeled Telugu dataset.

Step 4: Dataset Refinement

Low-quality pseudo-labeled samples are filtered to improve the quality of the training dataset.

Step 5: Model Retraining

The model is retrained using both manually labeled data and refined pseudo-labeled data to improve prediction accuracy.

Step 6: Explainable AI

LIME is integrated to explain why the model predicts specific entities.

Step 7: Deployment

The trained model is deployed using Streamlit, where users enter Telugu text and receive entity predictions with visualization and explanations.

 System Architecture
                 Telugu Text Input
                         │
                         ▼
                 Text Preprocessing
                         │
                         ▼
              Manual Annotated Dataset
                         │
                         ▼
                spaCy NER Model Training
                         │
                         ▼
                Pseudo Label Generation
                         │
                         ▼
               Dataset Quality Refinement
                         │
                         ▼
                  Model Retraining
                         │
          ┌──────────────┴──────────────┐
          ▼                             ▼
   Named Entity Prediction       LIME Explainability
          │                             │
          └──────────────┬──────────────┘
                         ▼
          Streamlit Web Application
                         │
                         ▼
     Entity Visualization & Final Output
 Tech Stack
Category	Technology
Programming Language	Python 3.8
NLP Framework	spaCy
Machine Learning	Semi-Supervised Learning
Explainable AI	LIME
Frontend	Streamlit
Visualization	spaCy Displacy
IDE	Visual Studio Code
Version Control	Git & GitHub
Operating System	Windows 7 or above
 Project Structure
SMARTER-NER/
│
├── dataset/
│   ├── labeled_data/
│   ├── unlabeled_data/
│
├── models/
│   ├── trained_spacy_model/
│
├── preprocessing/
│   ├── preprocess.py
│
├── training/
│   ├── train_model.py
│
├── pseudo_labeling/
│   ├── generate_labels.py
│
├── refinement/
│   ├── refine_dataset.py
│
├── explainability/
│   ├── lime_explainer.py
│
├── app.py
├── requirements.txt
├── README.md
└── LICENSE
 Installation and Setup
Clone the Repository
git clone https://github.com/yourusername/SMARTTER-NER.git
Navigate to the Project Directory
cd SMARTTER-NER
Create Virtual Environment
python -m venv venv
Activate Virtual Environment

Windows

venv\Scripts\activate
Install Required Packages
pip install -r requirements.txt
Run the Application
streamlit run app.py
 Model Performance

The SMARTTER NER model achieves improved performance by combining manually labeled data with pseudo-labeled data through Semi-Supervised Learning. Dataset refinement removes low-quality predictions, resulting in better accuracy and more reliable entity recognition. The integration of LIME improves model transparency by explaining prediction results, making the system both accurate and interpretable. (Your PPT does not include numerical metrics such as Accuracy, Precision, Recall, or F1-score.)

 Feature Enhancements (Future Scope)
Support fine-grained entity types such as Events, Products, and Numerical Expressions.
Integrate cross-lingual learning using related Indian languages.
Replace LIME or complement it with SHAP for enhanced explainability.
Develop real-time applications such as chatbots, virtual assistants, and information extraction systems.
Extend support to multiple low-resource Indian languages.
Build more scalable, accurate, and interpretable NER systems.
 Contributors

Project Guide

Dr. V. Venkateshwara Rao (Professor, Ph.D.)

Team Members

CH. Yasaswi
P. Geetha Rani Sri
G. Sri Naga Sirisha
R. J. S. Raju
C. Nandiraju
 License

This project was developed for academic and research purposes as part of the Bachelor of Technology curriculum. It is intended for educational use and research in Natural Language Processing for low-resource languages. If published as an open-source project, it can be released under the MIT License, allowing others to use, modify, and distribute the software with proper attribution.

This version is fully aligned with your uploaded SMARTER NER presentation and does not add unsupported technical details or performance metrics.
