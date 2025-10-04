# MLOps Challenges

This repository contains a series of practical MLOps challenges designed to help you learn and apply best practices for machine learning operations. The project covers experimentation, model training, testing, deployment, and automation using modern tools and workflows.

## Project Structure

```
├── _build.yml                # Build configuration
├── _config.yml               # Project configuration
├── index.md                  # Project overview
├── pytest.ini                # Pytest configuration
├── requirements.txt          # Python dependencies
├── documentation/            # Step-by-step guides and documentation
│   ├── 00-script.md
│   ├── 01-aml-job.md
│   ├── 02-github-actions.md
│   ├── 03-trigger-workflow.md
│   ├── 04-unit-test-linting.md
│   ├── 05-environments.md
│   ├── 06-deploy-model.md
│   └── media/
│       └── 00-01-github-secret.png
├── experimentation/          # Notebooks and dev data
│   ├── train-classification-model.ipynb
│   └── data/
│       └── diabetes-dev.csv
├── production/               # Production data
│   └── data/
│       └── diabetes-prod.csv
├── src/                      # Source code
│   ├── job.yml               # Job configuration
│   └── model/
│       └── train.py          # Model training script
├── tests/                    # Unit tests and test datasets
│   ├── __init__.py
│   ├── test_train.py
│   └── datasets/
│       ├── first.csv
│       ├── foo.py
│       └── second.csv
```

## Getting Started

1. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
2. **Experimentation**
   - Use the notebook in `experimentation/train-classification-model.ipynb` to explore and train models.
   - Dev data is in `experimentation/data/diabetes-dev.csv`.
3. **Model Training**
   - Main training script: `src/model/train.py`
   - Job configuration: `src/job.yml`
4. **Testing**
   - Run unit tests with pytest:
     ```bash
     pytest
     ```
   - Test scripts and datasets are in `tests/`.
5. **Deployment & Automation**
   - See `documentation/` for guides on deploying models, setting up CI/CD, and using GitHub Actions.

## Documentation

Comprehensive guides are available in the `documentation/` folder, covering:
- Running scripts and jobs
- Azure Machine Learning integration
- Setting up GitHub Actions workflows
- Triggering workflows
- Unit testing and linting
- Managing environments
- Deploying models

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements, bug fixes, or new challenges.

## License

This project is licensed under the MIT License.
