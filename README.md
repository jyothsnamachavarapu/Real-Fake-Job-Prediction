# Real/Fake Job Posting Prediction

## Abstract
This project aims to address the growing challenge of fraudulent job postings on online platforms. Using a dataset of 18,000 job descriptions (800 labeled as fraudulent), we employ machine learning models like Random Forest, LSTM, SVM, and XGBoost. To handle class imbalance, techniques like SMOTE and ADASYN are applied. The SVM model achieved the highest accuracy (99%), while LSTM excelled in identifying fraudulent postings. The project includes a deployed Streamlit application for real-time predictions, enhancing safety and trust in job platforms.

---

## Key Features
- **Dataset**: Kaggle dataset with 18,000 job descriptions, including text and metadata.
- **Models**: Random Forest, LSTM, SVM, and XGBoost.
- **Techniques**: SMOTE, ADASYN, TF-IDF, and target encoding.
- **Performance**: 
  - **SVM**: Best overall (Accuracy: 99%, F1-Score: 0.85).
  - **LSTM**: Highest recall for fraudulent cases (87%).
  - **Random Forest**: Balanced detection (F1-Score: 0.81).
  - **XGBoost**: Best recall for fraud detection (92%).
- **Deployment**: Streamlit web app for real-time prediction.

---

## Methodology
1. **Data Preprocessing**:
   - Text standardization, tokenization, stop-word removal, and TF-IDF vectorization.
   - Metadata encoding using target encoding.
   - Missing values handled via mode/mean imputation.

2. **Class Imbalance Management**:
   - SMOTE and ADASYN applied to address minority class underrepresentation.

3. **Model Evaluation**:
   - Metrics: Accuracy, Precision, Recall, F1-Score, and Confusion Matrix.
   - SVM and LSTM prioritized for fraud detection; Random Forest provided balanced results.

---

## Results
| Model          | Accuracy | Class 0 F1 | Class 1 F1 |
|----------------|----------|------------|------------|
| Random Forest  | 98.32%   | 0.99       | 0.81       |
| LSTM           | 97%      | 0.99       | 0.77       |
| SVM            | 99%      | 0.99       | 0.85       |
| XGBoost        | 89%      | 0.94       | 0.45       |

- **SVM**: Best balanced performance.
- **LSTM**: Best for high recall in detecting fraudulent listings.
- **XGBoost**: Best for maximizing fraud detection recall.

---

## Deployment
- A Streamlit application is deployed to provide real-time predictions of job posting legitimacy. Users can upload job descriptions and metadata for instant classification.

---

## Authors
- **Yaswanth Reddy Yarrabandla**: Data preprocessing, model implementation.
- **Lakshmi Jyothsna Machavarapu**: NLP techniques, dataset curation.
- **Tushar Vantaram**: Model selection, documentation.
- **Bhavana Tumkunta**: Dataset preparation, project presentations.

---

## References
1. Anita, S. et al. (2021). "Fake Job Detection and Analysis Using Machine Learning and Deep Learning Algorithms."
2. Vidros, S. et al. (2017). "Automatic Detection of Online Recruitment Frauds."
3. Chawla, N. et al. (2002). "SMOTE: Synthetic Minority Over-sampling Technique."
4. Bahdanau, D. et al. (2015). "Neural Machine Translation by Jointly Learning to Align and Translate."

For a complete list of references, see the [report](./Final_report.pdf).

---

## Future Work
- Enhance model scalability with real-time data pipelines.
- Explore ensemble techniques and hybrid architectures.
- Extend the model's capabilities for multilingual datasets.

---

## License
This project is licensed under the MIT License. See `LICENSE` for more details.
