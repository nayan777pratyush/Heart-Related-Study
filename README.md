
Or in Colab, the major packages are preinstalled; just upload `heart.csv` when prompted.

---

## How to run

1. Open the notebook in Google Colab:
   - Click "Open in Colab" badge at the top of the notebook (or use the Colab link shown in the notebook).
   - Upload `heart.csv` when prompted and run the cells sequentially.

2. Run locally:
   - Place `heart.csv` in the same directory as the notebook.
   - Start Jupyter:
     ```
     jupyter notebook R23EF192_Assignment_1.ipynb
     ```
   - Run the notebook cells in order.

3. Command-line run (to export or run non-interactively):
   - You can execute the notebook via nbconvert / papermill to produce an executed notebook or HTML report.

---

## Notebook structure (high-level)

- Environment check & file upload (handles Colab and local)
- Imports and plotting configuration
- Data load, preview and shape printing
- Exploratory Data Analysis: histograms, correlations, pairplots, class balance checks
- Preprocessing: imputers, scalers, categorical encoding if needed
- Train / validation split
- Model training: Logistic Regression, Decision Tree, Random Forest, SVM, KNN
- Model evaluation and comparison (accuracy, precision, recall, F1, confusion matrix)
- Visualizations for insights and model results

---

## Evaluation metrics reported

- Accuracy
- Precision
- Recall (Sensitivity)
- F1-score
- Confusion matrix

---

## Tips & notes

- Ensure `heart.csv` is the correct dataset (Kaggle/UCI heart disease CSV). Column encodings can differ between sources — verify `thal` and `ca` encodings if you encounter inconsistent values.
- For reproducibility, set random seeds (e.g., in train_test_split and model constructors).
- Consider cross-validation and hyperparameter search (GridSearchCV / RandomizedSearchCV) if you want more robust model selection.
- If class imbalance is present, consider stratified splits and metrics beyond accuracy (precision/recall, ROC AUC).

---

## License & Attribution

Please attribute the original dataset source (Kaggle / UCI) if you use the heart disease data. This README/template is provided as-is; include an appropriate license for your project if required (MIT, Apache 2.0, etc.).

---

## Contact

GitHub: @nayan777pratyush

If you'd like, I can:
- Convert this into a README.md file and create a commit for you,
- Add badges (Colab, Python version, license),
- Or generate a short abstract to include at the top for a report.
