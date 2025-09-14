# Credit Risk Score Calculator

This project estimates a credit risk score from user financial/behavioral information. Feature engineering and modeling use scikit-learn, with a baseline LinearRegression model. A simple Streamlit UI lets you input features and see the predicted default probability, credit score, and a rating.

## Description

What’s inside:

- ```prediction_helper.py``` — loads the trained model, preprocesses inputs, and returns ```(probability, credit_score, rating)```.

- ```main.py``` — Streamlit app with inputs for age, income, loan details, delinquencies, utilization, etc.
It also displays a computed Loan-to-Income Ratio (for reference).

- ```artifacts/``` — stores your trained model file (e.g., ```model_data.joblib```).

Note: UI fields **Delinquency Ratio** and **Credit Utilization Ratio** are entered as **percent values (0–100)** in the app.

## Getting Started

### Dependencies

**Python:** 3.10+

**Python packages:** ```streamlit, scikit-learn, pandas, numpy, joblib
(install via requirements.txt)```

### Installing
```
git clone https://github.com/<your-username>/credit-risk-score.git
cd credit-risk-score

python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS / Linux
source .venv/bin/activate

pip install -r requirements.txt
```
Place your trained model (e.g., ```model_data.joblib```) in ```artifacts/``` and make sure ```prediction_helper.py``` points to that path.

### Executing program

Run the Streamlit app:

```
streamlit run main.py
```
Then open the URL shown in the terminal (usually http://localhost:8501
), fill the form, and click **“Calculate Risk”** to see:

- **Default Probability** (e.g., 23.5%)

- **Credit Score** (numeric score)

- **Rating** (e.g., ```A / B / C``` or similar, depending on your helper logic)

## Help

Port already in use (8501)
```
# macOS/Linux
lsof -i :8501
kill -9 <PID>
# Windows
netstat -ano | findstr :8501
taskkill /PID <PID> /F
```
Model file not found
- Confirm the model exists at ```artifacts/model_data.joblib``` (or update the path used in ```prediction_helper.py```).


## Acknowledgments

**This project was curated by**: 
* https://codebasics.io/
* https://www.linkedin.com/in/dhavalsays/
