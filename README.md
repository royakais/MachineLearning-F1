# MachineLearning-F1

A practical machine-learning project focused on analyzing Formula 1 data through data preparation, exploratory visualization, classification, and regression.

The repository contains the project notebooks, serialized preprocessing objects, trained models, and prediction outputs used throughout the workflow.

## Project workflow

The project is organized as an end-to-end machine-learning pipeline:

1. **Data preprocessing**
   - Load the Formula 1 dataset.
   - Clean and prepare the data for analysis.
   - Encode categorical variables and scale numerical features.
   - Save reusable preprocessing artifacts such as the encoder and scaler.

2. **Data visualization**
   - Explore relationships and patterns in the Formula 1 data.
   - Create visual summaries to support interpretation and feature selection.

3. **Classification**
   - Prepare classification features and targets.
   - Train and evaluate a classification model.
   - Save the trained model and the feature metadata required for reuse.

4. **Regression**
   - Build a regression workflow for numerical predictions.
   - Train and evaluate regression models.
   - Generate and export prediction results for the relevant seasons and positions.

5. **Model artifacts and outputs**
   - Reusable `.pkl` files store preprocessing objects, feature information, and trained models.
   - Excel files contain datasets and generated prediction outputs.

## Repository structure

```text
MachineLearning-F1/
├── Data Preprocessing/
│   ├── preprocessing.ipynb
│   ├── F1_dataset_2024-2026.xlsx
│   ├── ohe.pkl
│   └── scaler.pkl
├── Data Visualization/
│   └── Data visualization v2 (1).ipynb
├── Data Classification/
│   ├── Classification.ipynb
│   ├── classification_features.pkl
│   └── classification_model.pkl
├── Data Regression/
│   ├── regression.ipynb
│   ├── regression_features.pkl
│   ├── regression_model.pkl
│   └── prediction output files
├── Trained Set/
├── Test Set/
└── README.md
```

## Getting started

### 1. Clone the repository

```bash
git clone https://github.com/royakais/MachineLearning-F1.git
cd MachineLearning-F1
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on macOS/Linux:

```bash
source .venv/bin/activate
```

Activate it on Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

### 3. Install the required packages

The notebooks use common Python data-science and machine-learning libraries, including:

- Python 3
- Jupyter Notebook or JupyterLab
- pandas
- NumPy
- Matplotlib
- scikit-learn
- openpyxl, for Excel files

Install them with:

```bash
pip install jupyter pandas numpy matplotlib scikit-learn openpyxl
```

### 4. Run the notebooks in sequence

Open Jupyter from the repository root:

```bash
jupyter notebook
```

Recommended order:

1. `Data Preprocessing/preprocessing.ipynb`
2. `Data Visualization/Data visualization v2 (1).ipynb`
3. `Data Classification/Classification.ipynb`
4. `Data Regression/regression.ipynb`

Run the preprocessing notebook first so that the encoder, scaler, and prepared data are available to later stages.

## Reproducibility notes

- Run notebooks from the repository root when relative paths are used.
- Keep the generated `.pkl` model and preprocessing files together with their corresponding notebooks.
- Review notebook outputs after rerunning them, because model results may change when the dataset or dependencies change.
- The Excel files in the repository represent saved datasets and prediction outputs from the project workflow.

## Contributors

This project was created by:

- Roya Kais
- Amanda Elkik
- Daisy
- Christia
- Christina

Contributions are welcome. Please open an issue before making a substantial change, then submit a pull request describing the update and how it was tested.

## License

No license has been specified for this repository yet. Until a license is added, reuse and redistribution should be treated as restricted by default.
