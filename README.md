# Obesity Levels Estimation & Decision Tree Analysis

This repository contains a complete machine learning pipeline and analysis for estimating obesity levels based on eating habits and physical condition using a Decision Tree classifier.

---

## Project Structure
```text
D:.
│   LICENSE
│   obesity_decision_tree.ipynb
│   README.md
│   requirements.txt
│
+---data
│       estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition.zip
│
+---other_examples
│       HeartDisease .docx
│       Truck_10_Brands.docx
│       Truck_22_Brands.docx
│
\---results
        Accuracy_with_vs_without_Hight_and_Weight.png
        Accuracy_with_vs_without_Hight_and_Weight_Table.png
        Confusion_Matrix_For_Depth=16.png
        Confusion_Matrix_For_Depth=16_With_Weight_and_Hight.png
        Features_Importance_For_Depth=16.png
        Test_Accuracy,Precision,Recall,F1_vs_Depth.png
        tree_final.pdf
        tree_final.png
```
---

## Dataset Overview
- Source: UCI Machine Learning Repository (Dataset ID: 544)
- Instances: 2,111 records
- Features: 14 attributes including demographic information, eating habits (e.g., FAVC, FCVC, NCP, CAEC, CH2O), and physical condition metrics (e.g., Age, Gender, SCC, FAF, TUE, CALC, MTRANS). Note that Height and Weight are dropped by default to prevent data leakage and test behavioral prediction capabilities.
- Target: NObeyesdad (Multi-class classification ranging from Insufficient Weight to Obesity Type III).

---

## Installation & Requirements

To run the project locally or replicate the analysis, ensure you have Python installed along with the required libraries.

1. Clone the repository or download the project folder.
2. Install dependencies:
   pip install -r requirements.txt
   *(Alternatively, the notebook installs ucimlrepo dynamically if run inside Google Colab).*

---

## How to Run

### Option 1: Google Colab (Recommended)
1. Open Google Colab.
2. Upload or open the obesity_decision_tree.ipynb notebook.
3. Run the cells sequentially. The script will automatically fetch the dataset via ucimlrepo, pre-process the data, sweep through different tree depths, evaluate performance metrics, and generate the visualizations.

### Option 2: Local Jupyter Notebook
1. Navigate to the project root directory in your terminal.
2. Start Jupyter Notebook:
   jupyter notebook
3. Open obesity_decision_tree.ipynb and execute the cells.

---

## Key Features & Methodology
- Data Preprocessing: Handles categorical variables using one-hot encoding (pd.get_dummies), splits data into training and stratified test sets (80/20 split), and drops direct biometric identifiers (Height, Weight) to focus purely on lifestyle and behavioral habits.
- Depth Sweeping: Iterates through tree depths (from 1 to max depth) to monitor train/test accuracy, precision, recall, and macro F1-score.
- Evaluation & Visualization: Generates confusion matrices, classification reports, feature importance graphs, and exports the final decision tree structure (tree_final.pdf / tree_final.png).

---

## License
Please check the LICENSE file for details regarding usage and permissions.# Obesity-Risk-DecisionTree-Classifier
# Obesity-Risk-DecisionTree-Classifier
