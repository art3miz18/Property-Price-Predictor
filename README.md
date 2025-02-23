
# Real Estate Valuation Analysis and Visualization

This repository contains the source code, analysis notebooks, and documentation for a project focused on predicting real estate valuations using regression analysis. The project includes data cleaning, exploratory data analysis (EDA), feature engineering, model building, and visualization. A Gradio interface is also provided to allow interactive exploration of the analysis.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation and Setup](#installation-and-setup)content\Real_estate_valuation_data_set.xlsx
- [Usage](#usage)
- [Gradio Interface](#gradio-interface)
- [Results and Visualizations](#results-and-visualizations)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The aim of this project is to build a refined regression model for predicting house prices (per unit area) using historical transaction data from Sindian District, New Taipei City, Taiwan. The analysis covers:
- Data cleaning and preparation
- Exploratory data analysis (EDA)
- Feature engineering and transformation
- Regression model building and diagnostics
- Visualization of key insights

An interactive Gradio interface is provided to make it easy for users to upload datasets and view analysis outputs.

## Dataset
The project uses the **Real Estate Valuation Data Set** from the UCI Machine Learning Repository. The dataset includes:
- **X0 (No.)**: Row identifier
- **X1 (Transaction Date)**: Transaction date (e.g., March 2013)
- **X2 (House Age)**: Age of the house in years
- **X3 (Distance to Nearest MRT Station)**: Distance in meters
- **X4 (Number of Convenience Stores)**: Count of convenience stores in the vicinity
- **X5 (Latitude)**: Geographical latitude (in degrees)
- **X6 (Longitude)**: Geographical longitude (in degrees)
- **Y (House Price of Unit Area)**: Target variable

## Project Structure
```
Real_Estate_Valuation/
│
├── data/
│   ├── Real_Estate_Valuation_Data_Set.xlsx   # Original dataset
│   └── dataset_preprocessed.csv               # Preprocessed dataset (if applicable)
│
├── notebooks/
│   ├── EDA_regression_01.ipynb                # Jupyter Notebook with full analysis
│   └── Visualizations.ipynb                   # Additional visualizations and interactive plots
│
├── gradio_app/
│   ├── app.py                                 # Gradio interface for interactive analysis
│   └── requirements.txt                       # Dependencies for the Gradio app
│
├── report/
│   └── Final-Project-Report-Team-1.pdf          # Final technical report
│
├── README.md                                  # This file
└── requirements.txt                           # Main project dependencies
```

## Installation and Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/Real_Estate_Valuation.git
   cd Real_Estate_Valuation
   ```

2. **Set Up a Virtual Environment:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # For Windows: venv\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   For the Gradio interface, install additional dependencies from `gradio_app/requirements.txt` if needed.

## Usage

### Running the Jupyter Notebooks
Navigate to the `notebooks/` directory and launch Jupyter Notebook:
```bash
jupyter notebook
```
Open and run the notebooks to perform EDA, model building, and visualization.

### Launching the Gradio Interface
To start the interactive Gradio interface:
```bash
cd gradio_app
python app.py
```
This will launch a local web server where you can upload your dataset, trigger the analysis, and view interactive visualizations.

## Gradio Interface
The Gradio interface allows users to:
- Upload a CSV dataset.
- Automatically process the dataset (including cleaning, feature transformation, and regression analysis).
- View interactive graphs such as scatter plots, heatmaps, and regression diagnostics.
- See a text summary of model performance metrics (e.g., R² and RMSE).

## Results and Visualizations
Key visualizations included in the project:
- **Histograms and Boxplots:** For initial data distribution analysis.
- **Pairplots:** To visualize relationships between variables.
- **Correlation Heatmaps:** To identify multicollinearity.
- **Regression Diagnostic Plots:** To evaluate model performance.
- **PCA Visualizations:** For combined geographical feature representation.

## Contributing
Contributions are welcome! Please fork the repository and submit pull requests for enhancements or bug fixes.

## License
This project is licensed under the [MIT License](LICENSE).
