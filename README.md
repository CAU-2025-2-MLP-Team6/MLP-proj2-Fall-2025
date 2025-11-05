# MLP-proj2-Fall-2025
CAU Machine Learning Project Class - Term Project 2 Repository

# Descriptions

## Proj2_MLP_Fall.ipynb
This code runs in Colab and covers the entire process of the project.
You must use the T4 GPU runtime environment.
A Kaggle API Token is required for convenient access to the Competition data. In the very first cell, you obtain the Kaggle API Token and download the training data by inputting the `kaggle.json` file.

## Proj2_MLP_Fall_baseline.ipynb
This code is for submission to the Kaggle Competition and covers the baseline model construction process corresponding to Step 1.
You must use the P100 GPU runtime environment.
The Competition's training data must be added as an input in the Kaggle notebook before submission.

## Proj2_MLP_Fall_final.ipynb
This code is for submission to the Kaggle Competition and covers the final model construction process.
Dependencies are required to use models like MiniLM-L6-v2 and DeBERTa-v3-small. In addition to adding the Competition data as input, you must also add the following datasets: [MiniLM-L6-v2](https://www.kaggle.com/datasets/shinomoriaoshi/sentencetransformersallminilml6v2) and [DeBERTa-v3-small](https://www.kaggle.com/datasets/miwojc/debertav3small).
Furthermore, a new dataset must be created and added which contains the `wheels_dir` folder, generated using the command `!pip download sentence-transformers transformers peft accelerate datasets -d wheels_dir`. This dataset is used for pip local installation in the first block of the code.

## csv files
The files `step_1_submission.csv`, `step_2_submission.csv`, `step_3_deberta_lora_submission.csv`, `step_3_lgb_submission.csv` contain the results of the models created through their respective steps. The `submission.csv` file contains the final model's results.