# Credit Risk Score Calculator

This project estimates a credit risk score from user financial/behavioral information. Feature engineering and modeling use scikit-learn, with a baseline LinearRegression model. A simple Streamlit UI lets you input features and see the predicted default probability, credit score, and a rating.

## Description

What’s inside:

prediction_helper.py — loads the trained model, preprocesses inputs, and returns (probability, credit_score, rating).

main.py — Streamlit app with inputs for age, income, loan details, delinquencies, utilization, etc.
It also displays a computed Loan-to-Income Ratio (for reference).

artifacts/ — stores your trained model file (e.g., model_data.joblib).

Note: UI fields Delinquency Ratio and Credit Utilization Ratio are entered as percent values (0–100) in the app.

## Getting Started

### Dependencies

Python: 3.10.12 

runtime

Packages: scikit-learn, pandas, numpy, joblib (plus xgboost and streamlit if you plan to use them later). See requirements.txt for exact versions.

### Installing

git clone https://github.com/<your-username>/credit-risk-score.git
cd credit-risk-score

python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS / Linux
source .venv/bin/activate

pip install -r requirements.txt


### Executing program

* How to run the program
* Step-by-step bullets
```
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)

## Version History

* 0.2
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.1
    * Initial Release

## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* [awesome-readme](https://github.com/matiassingers/awesome-readme)
* [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* [dbader](https://github.com/dbader/readme-template)
* [zenorocha](https://gist.github.com/zenorocha/4526327)
* [fvcproductions](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46)
