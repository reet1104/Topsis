# Topsis
This repository contains a Python implementation of the Technique for Order Preference by Similarity to Ideal Solution (TOPSIS), a multi-criteria decision-making (MCDM) method. TOPSIS is used to rank and evaluate alternatives based on multiple criteria, considering both their closeness to an ideal solution and their distance from a nadir (worst-case) solution.

Features
Accepts input data from a CSV file for analysis.
Normalizes numerical data using vector normalization.
Applies user-defined weights and impacts (+ for benefit criteria, - for cost criteria) to compute the weighted normalized decision matrix.
Calculates ideal and anti-ideal solutions and their respective distances for each alternative.
Computes the TOPSIS score and assigns ranks to alternatives.
Outputs results including TOPSIS scores and ranks in a CSV file.
Usage
Prepare the input CSV file containing numerical data for evaluation.
Run the script with the following command:
bash
Copy
Edit
python 102203210.py <input_file> <weights> <impacts> <output_file>
<input_file>: Path to the input CSV file.
<weights>: Comma-separated list of weights for each criterion (e.g., 0.2,0.2,0.2,0.2,0.2).
<impacts>: Comma-separated list of impacts for each criterion (+ for benefit, - for cost).
<output_file>: Path to save the output CSV file containing results.
Example
bash
Copy
Edit
python 102203210.py data.csv "0.2,0.2,0.2,0.2,0.2" "+,+,-,+,+" result.csv
Requirements
Python 3.x
Pandas
NumPy
SciPy
Install dependencies using:

bash
Copy
Edit
pip install pandas numpy scipy
Output
The output CSV file includes:

The original data.
Calculated TOPSIS scores for each alternative.
Ranks based on the TOPSIS scores.

