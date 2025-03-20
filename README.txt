Author: Muhammad Zohaib Khan 
Email: zohaibkhanzohaibi2003@gmail.com
Date: 20-03-2025

PII Masking using LLMs

Project Overview

This project focuses on masking Personally Identifiable Information (PII) such as names and emails using transformer models and Large Language Models (LLMs). The pipeline includes data processing, model training, and evaluation, with a reproducible notebook for testing the trained model.

Project Structure

📂 internship_task/
│-- 📂 Internship_task_data/                 	 # Dataset in JSON format
│-- 📂 results/                                 # for model training checkpoints,  it is not added to zip file due to its size > 1gb
│-- 📂 saved_model3/                            # saved model after fine tuning
│-- 📜 report.pdf                               # Report and documentation
│-- 📜 01_data_processing_adding_emails.ipynb   # Adding emails to the data
│-- 📜 02_few further checkups.ipynb            # Double-checking data integrity
│-- 📜 03_model_training.ipynb                  # Training transformer model and evaluating model performance
│-- 📜 04_masking_pipeline.ipynb                # Script to test trained model
│-- 📜 05_Zero_shot_PII_masking_Using_LLM.ipynb # Zero-shot PII masking using LLM
│-- 📜 email_added_data.json                    # Processed dataset with emails added, created after 01.
│-- 📜 README.md                                # Project documentation

Run the Reproducible Notebook:
Open 04_masking_pipeline.ipynb in Jupyter Notebook or Google Colab to test the trained model.
change the example input sequence as per your choice and run.

Process Breakdown

Step 1: Preprocess raw data and add emails (01_data_processing_adding_emails.ipynb).

Step 2: Validate the processed dataset (02_few further checkups.ipynb).

Step 3: Train a transformer model for PII detection (03_model_training.ipynb).

Step 4: Use 04_masking_pipeline.ipynb to test the trained model on random texts.

Step 5: Implement zero-shot PII masking with a smaller LLM (05_Zero_shot_PII_masking_Using_LLM.ipynb).

Model Training and Evaluation

Uses a transformer-based model for entity recognition and masking.

Evaluates model performance using precision, recall, FNR, FPR and F1-score.

Testing the Model

The 04_masking_pipeline.ipynb notebook is the a testing script.

Load the trained model from saved_models3/ and test it on new text samples.




Author: Muhammad Zohaib Khan 
Email: zohaibkhanzohaibi2003@gmail.com
Date: 19-03-2025

