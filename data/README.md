# Data

## Source

This project uses data from the Kaggle **IEEE-CIS Fraud Detection** competition.

Competition page:

https://www.kaggle.com/competitions/ieee-fraud-detection

The dataset contains anonymized e-commerce transaction and identity information
provided for the competition by Vesta Corporation.

## Files Used

Only the labelled training data are required for this project:

- `train_transaction.csv`
- `train_identity.csv`

The competition test files are not used because this project evaluates model
performance through chronological splits of the labelled training data rather
than through a Kaggle competition submission.

## Data Access

The competition data are not distributed with this repository.

To reproduce the notebooks:

1. Create or sign in to a Kaggle account.
2. Open the IEEE-CIS Fraud Detection competition and accept its rules.
3. Generate a Kaggle API token from your Kaggle account settings.
4. In Google Colab, add the token as a secret named `KAGGLE_API_TOKEN`.
5. Grant the notebook access to that secret.
6. Run the notebook from the beginning.

The notebooks use the official Kaggle CLI to download the required files
programmatically.

The API token is read from Colab Secrets and is never stored in the notebooks
or committed to this repository.

## Repository Data Directory

The local directory is intentionally structured as:

```text
data/
├── README.md
└── raw/
    └── .gitkeep