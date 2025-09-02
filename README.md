# AI-Powered Email Classification for Asset Management Companies  

This repository contains the implementation and research artifacts for a thesis project on **automating customer email handling in Asset Management Companies (AMCs)** using **machine learning and natural language processing (NLP)**. The solution focuses on hierarchical email classification and entity extraction, integrated into customer service workflows.  

## 📌 Features  
- **Hierarchical Classification (4 Levels):**  
  - Type → Area → Sub Area → Child Sub Area  
- **Transformer-based Models:**  
  - Fine-tuned BERT classifiers for intent detection  
  - Named Entity Recognition (NER) for extracting structured fields (e.g., folio numbers, transaction IDs, dates)  
- **Model Evaluation:**  
  - Achieved Macro F1-score of **0.89** (Type) and **0.95** (Child Sub Area)  
  - Weighted F1-scores of **0.94** and **0.98**  
- **Explainability:**  
  - SHAP analysis for model interpretability  
- **Synthetic + Realistic Dataset:**  
  - Custom-built dataset simulating AMC email traffic  

## 📂 Repository Structure  
```bash
├── data/                      # Datasets (synthetic + CSV files)
├── notebooks/                 # Jupyter notebooks with model pipeline
│   ├── Email_Classification_Cleaned.ipynb
├── models/                    # Trained model artifacts (if stored)
├── src/                       # Utility scripts (preprocessing, training, evaluation)
├── requirements.txt           # Dependencies
├── README.md                  # Project overview (this file)
└── LICENSE                    # License file
```

## ⚙️ Installation  
1. Clone this repository:  
   ```bash
   git clone https://github.com/hrithik-singh07/AI-Email-Classification-Information-Retrival-Model.git
   cd AI-Email-Classification-Information-Retrival-Model
   ```
2. Create a virtual environment and install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage  
1. Open the cleaned notebook:  
   ```bash
   jupyter notebook notebooks/Email_Classification_Cleaned.ipynb
   ```  
2. Run all cells to:  
   - Load dataset  
   - Preprocess and tokenize text  
   - Train and evaluate models  
   - Visualize results  

## 📊 Results  
- **Top-Level Classification (Type):** Macro F1 = 0.89  
- **Fine-Grained (Child Sub Area):** Macro F1 = 0.95  
- **Interpretability:** SHAP confirmed domain-specific feature importance  

## 📖 Thesis Reference  
This repository supports the thesis:  
*“Automating Email Classification and Entity Extraction in Asset Management Companies using Transformer-based NLP Models”*  

## 🙏 Acknowledgements  
- OpenAI **ChatGPT** was used for commenting, documentation, and code refactoring support.  
- NLTK, Scikit-learn, XGBoost, and SHAP libraries for implementation.  

## 📜 License  
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.  
