# 📧 Jacob Yim - Phishing Email Detector (Work In Progress) - UPDATED 4/27/25

This project builds a phishing email classification model using a pre-trained DistilBERT model from Hugging Face.  
The model was fine-tuned in Google Colab on a small custom dataset to classify emails as either phishing or legitimate.

🚧 **Work in Progress**  
This project is still under development and will be updated with more data, fine-tuning, and evaluation in the future.

---

## 🔥 Project Overview

- **Model:** DistilBERT (from Hugging Face Transformers)
- **Environment:** Google Colab
- **Task:** Classify email text as either `phishing` (1) or `legitimate` (0)
- **Dataset:** Custom-made sample dataset (currently 31 examples)

---

## 📂 How to Use

> ⚠️ Due to compatibility differences, the `.ipynb` notebook may not render correctly on GitHub.  
> Please **download** the notebook and open it in **Google Colab** or **Jupyter Notebook** to view and run the project properly.

### Steps:
1. Download the `.ipynb` file from this repository.
2. Open it with Google Colab or Jupyter Notebook.
3. Run the cells step-by-step to:
    - Preprocess the email texts (remove HTML, URLs, special characters, etc.)
    - Fine-tune the DistilBERT model
    - Predict phishing/legitimate labels for new emails
    - **(New!)** Allow real-time user input to classify custom email messages

---

## 🛠 Features

- **Data Cleaning:** 
  - Uses BeautifulSoup to remove HTML tags
  - Removes URLs and special characters
  - Converts text to lowercase and standardizes spaces

- **Model Fine-Tuning:** 
  - Fine-tunes DistilBERT using Hugging Face Trainer API
  - Splits dataset into training and test sets (70%/30%)

- **New Email Prediction:** 
  - Classifies new batches of email messages entered in code
  - Provides outputs as "Phishing" or "Legitimate"

- **User Input Email Prediction:** 
  - **(New!)** Allows users to manually type in an email message
  - Classifies user-provided emails as phishing or legitimate in real-time

---

## 🚀 Next Steps

- Expand the dataset with more real-world phishing and legitimate emails
- Further fine-tune the model on larger datasets
- Evaluate the model with precision, recall, F1-score
- Save and load fine-tuned models
- Deploy the model as a simple web application (optional)

---

## 📜 License

This project is released for educational purposes only.
