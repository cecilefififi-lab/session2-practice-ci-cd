# CI/CD with GitHub Actions

This project demonstrates a complete CI/CD pipeline using GitHub Actions for automated linear model training and releases.

## How it works

1. When `training_data.csv` is modified and pushed to `main`, the pipeline:
   - Trains a new linear regression model
   - Pushes the model to the `release` branch
   - Creates a GitHub Release

## Files

- `training_data.csv` - Training dataset (YearsExperience, Salary)
- `train_model.py` - Python script that trains the linear model
- `requirements.txt` - Python dependencies
- `.github/workflows/ci-cd.yml` - GitHub Actions workflow