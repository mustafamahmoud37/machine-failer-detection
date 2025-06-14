# Machine-Failure-Detection

## overview

- Data loading and exploration

- Data preprocessing

- Model training using Random Forest

- Model evaluation with accuracy, precision, recall, and confusion matrices

- Final conclusions and insights for operational improvement

## Dataset

**Dataset Description**
-The dataset used in this project comes from a predictive maintenance scenario and includes sensor readings from industrial machines. The primary goal is to predict machine failures based on operating conditions.

- Files:
train.csv: Contains historical data with machine failures.

test.csv: Contains data without failure labels, used for inference or competition-style submission.

sample_submission.csv: Sample format for test predictions.

- Dataset Size:
Training set: 136,429 rows × 14 columns

Test set: 90,954 rows × 13 columns

- Features:
Column Name	Description
id	Unique row identifier
Product ID	Identifier for each machine/product
Type	Machine type (L, M, or H)
Air temperature [K]	Ambient temperature around the machine
Process temperature [K]	Internal processing temperature
Rotational speed [rpm]	Machine's operating speed
Torque [Nm]	Load applied to the machine
Tool wear [min]	Amount of wear on the cutting tool

- Target Labels:
Machine failure: Binary label (1 if any failure occurred, 0 otherwise)

Subcomponents of failure (all binary):

TWF: Tool Wear Failure

HDF: Heat Dissipation Failure

PWF: Power Failure

OSF: Overstrain Failure

RNF: Random Failure

## Machine Learning Techniques
- **The notebook applies several ML techniques such as**:

- Supervised learning models (Random Forest)

- Data scaling and normalization

- Train-test splitting and cross-validation

- Performance metrics visualization

## Results
- Random Forest Training Accuracy: 0.999883639207071
- Random Forest Validation Accuracy: 0.9994600934596839
- Mean cross-validation score: 0.9995568987417383
