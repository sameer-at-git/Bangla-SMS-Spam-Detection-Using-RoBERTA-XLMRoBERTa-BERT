# A Comparative Analysis of BERT, RoBERTa, and XLM-RoBERTa for Bengali SMS Multiclass Spam Detection

## Summary of the Research Project
This project focuses on the automatic detection and classification of **spam**, **smishing (phishing via SMS)**, and **normal messages** in the **Bengali language**.  

We used the **Banglabarta dataset** and fine-tuned three state-of-the-art transformer-based models:  
- **BERT**  
- **RoBERTa**  
- **XLM-RoBERTa**  

Our research evaluates their performance on this task and identifies the most effective solution.  

**Key Finding:**  
**XLM-RoBERTa** achieved the best performance, making it the most effective model for Bengali SMS spam detection.

---

## Getting Started

### Prerequisites
You will need a Python environment with the following libraries installed:

- `torch`  
- `transformers`  
- `scikit-learn`  
- `pandas`  
- `numpy`  

Install dependencies using pip:

```bash
pip install torch transformers scikit-learn pandas numpy
```

---

## Repository Structure

```
data/                 # Small sample of the Banglabarta dataset
notebooks/            # Jupyter notebooks for preprocessing, fine-tuning, evaluation
images/               # Plots and tables for visualization
README.md             # Project overview
dataset_resource.md   # Dataset details and citation
```

---

## Usage

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Explore the Notebooks**  
   Open the notebooks in the `notebooks/` folder to see the full workflow.

3. **Download the Full Dataset (Optional)**  
   The `data/` folder contains only a small sample.  
   For full-scale experiments, download the complete dataset from the link in `dataset_resource.md`.

---

## Methodology

1. **Dataset Preparation**  
   - Used the **Banglabarta dataset** of Bengali SMS messages  
   - Created a **balanced subset** to prevent bias across classes (Smishing, Promotional, Normal)  

2. **Preprocessing**  
   - Text normalization  
   - Label encoding  

3. **Model Fine-Tuning**  
   - Fine-tuned three pre-trained transformer models: **BERT, RoBERTa, XLM-RoBERTa**  

4. **Performance Evaluation**  
   - Metrics used: **Accuracy, Precision, Recall, F1-score**

---

## Results and Discussion

| Model          | Accuracy  |
|----------------|-----------|
| **XLM-RoBERTa** | **98.92%** |
| BERT           | 98.20%    |
| RoBERTa        | 94.41%    |

**XLM-RoBERTa** outperformed the others.  
Its multilingual pre-training on 100+ languages gave it an edge in Bengali text classification.  
Meanwhile, **RoBERTa** lagged behind due to being pre-trained on English-only corpora.

---

## Citation
If you use this work, please cite the original research paper.  
Full citation details are provided in **`dataset resource.md`**.
