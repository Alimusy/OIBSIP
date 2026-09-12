# Oasis Infobyte Internship Projects

Four data science tasks completed during the Oasis Infobyte internship, each a
self-contained notebook.

| Notebook | Task | Approach | Result |
|---|---|---|---|
| [Iris.ipynb](Iris.ipynb) | Classify iris species from petal and sepal measurements | Logistic Regression | Clean separation, the classic starter problem |
| [Car_price.ipynb](Car_price.ipynb) | Predict used car selling price | Random Forest Regressor | R² 0.96 |
| [Sales_Prediction.ipynb](Sales_Prediction.ipynb) | Predict sales from advertising spend across TV, radio and newspaper | Linear Regression | R² 0.86 |
| [Unemployment.ipynb](Unemployment.ipynb) | Analyse unemployment in India through the Covid period | Exploratory data analysis and time series visualisation | Sharp spike visible in the April to June 2020 window |

## Open it

Every notebook runs in the browser, no setup:

- Iris classification [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alimusy/OIBSIP/blob/main/Iris.ipynb)
- Car price prediction [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alimusy/OIBSIP/blob/main/Car_price.ipynb)
- Sales prediction [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alimusy/OIBSIP/blob/main/Sales_Prediction.ipynb)
- Unemployment analysis [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alimusy/OIBSIP/blob/main/Unemployment.ipynb)

## Running them

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook
```

Each notebook loads its own dataset and runs top to bottom.

## What I took from it

The car price and sales tasks are both regression, but they behave nothing
alike. Car price has strong non-linear interactions between age, fuel type and
transmission that a linear model cannot reach, which is why Random Forest
lands at 0.96 there. Advertising spend is close to linear by construction, so
the simpler model is not just adequate, it is the right call.
