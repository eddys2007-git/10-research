# Interpretable Deep Learning for REIT Return Forecasting: A Comparative Study of LSTM, TVP–VAR, and SHAP-Based Explanations

This repository provides the data, code, and summary outputs supporting the empirical analysis presented in the accompanying manuscript "Interpretable Deep Learning for REIT Return Forecasting: A Comparative Study of LSTM, TVP–VAR, and SHAP-Based Explanations". The materials are organized to facilitate transparency, reproducibility, and independent verification of the main experimental results.

## Repository Structure

The repository contains three compressed archives:

### `dataset.zip`

This archive includes all datasets used in the study. It contains daily market price series and derived variables required for feature construction and crash labeling. The data are provided in a processed format consistent with the preprocessing steps described in Section 2 of the manuscript, including log-return transformation and alignment across assets.

### `scripts.zip`

This archive contains the full set of Python scripts used for data preprocessing, feature engineering, model training, evaluation, robustness testing, and interpretability analysis. The scripts implement the methodological pipeline described in the paper, including drawdown-based crash labeling, Random Forest classification, threshold calibration, robustness experiments, and SHAP-based feature attribution. File names and function structures are documented within the scripts to reflect their role in the analysis pipeline.

### `summary_results.zip`

This archive includes summary outputs generated from the experiments, such as performance metrics, robustness evaluation results, and aggregated statistics used to produce the main tables and figures reported in the manuscript. These files are provided to allow readers to quickly inspect the empirical outcomes without rerunning the full experimental workflow.

## Reproducibility Notes

All experiments were conducted using Python. The scripts are designed to be executed sequentially following the logical order of the research framework described in the paper. Random seeds were fixed where applicable to ensure result stability. Due to differences in hardware and software environments, minor numerical variations may occur, but the qualitative findings should remain unchanged.

## Usage

To reproduce the analysis:

1. Extract `dataset.zip` and place the contents in a local data directory.
2. Extract `scripts.zip` and follow the execution order indicated in the script headers.
3. Generated outputs can be compared against the files provided in `summary_results.zip`.

Detailed instructions and parameter settings are documented directly within the scripts.

## License and Disclaimer

The materials are provided for academic and research purposes only. Users are responsible for ensuring appropriate use of the data and code in accordance with applicable data and licensing requirements. The authors make no warranties regarding suitability for commercial applications.

## Citation

If you use this repository in your research, please cite the corresponding paper.
