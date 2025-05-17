# DI725_project

This is the main code base of the project of DI725 course. To execute the proposed method, [fine-tuning-paligemma-with-riscm-custom-tokenizer.ipynb](fine-tuning-paligemma-with-riscm-custom-tokenizer.ipynb) notebook should be exevuted on Colab environment. Since the training process requires large RAM usage, executing this file on the local environment may cause execution errors.

To execute the notebook properly, following keys should be defined and should be accessible from the notebook in Colab session.
- DATA_PATH: The path of RISCM folder
  - DATA_PATH
    - resized
      - *.jpg
    - captions.csv
- HF_TOKEN: Huggingface API token
- KAGGLE_USERNAME: Username of the Kaggle account (should habe been consented to the license for PaliGemma and Paligemma 2 models)
- KAGGLE_KEY: Kaggle API Key of the account
- WANDB_KEY: Weights & Biases account API key (will be used during training)

> NOTE:
> This notebook will download [modified-big-vision](https://github.com/ErenNarin/modified-big-vision) repository from GitHub to local environment. This repository is based on Google's [big-vision](https://github.com/google-research/big_vision) repository. This base repository modified to use suggested training and evaluation techniques. So, it is essential to use modified repository instead of the original one, to use suggested approaches.