# COVID-19-SINDY
A smiple demonstration of SINDY (Sparse Identification of Nonlinear Dynamics) to discover a dynamical system from real coronavirus time series data

## Description
SINDY is an algorithm that "combine(s) sparsity-promoting techniques and machine learning with nonlinear dynamical systems to discover governing equations from noisy measurement data". In the jupyter notebook, we retrieve the latest data from [CSSEGISandData
/COVID-19](https://github.com/CSSEGISandData/COVID-19) and trained a regression model that has sparse coefficient while powerful enough to describe the given training data.

We trained the model using 26 data points of recoeds in Hubei, and used it to predict future Japan data. It is interesting that, given only 26 data, the model is able to produce prediction that is similar to [SIR model](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology) commonly used in eppidemiology.

This experiment is conducted on Google colaboratory.[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shaoanlu/COVID-19-SINDY/blob/master/covid-19_SINDY.ipynb)

## Result
### Training data (time series records in Hubei from 22/01/2020 to 16/02/2020)
![](https://github.com/shaoanlu/COVID-19-SINDY/raw/master/imgs/trn.png)

### 30-day prediction in Japan (record on 16/02/2020 as initial condition)
![](https://github.com/shaoanlu/COVID-19-SINDY/raw/master/imgs/pred.png)


## Refernces
1. [Discovering governing equations from data by sparse identification of nonlinear dynamical systems](https://www.pnas.org/content/113/15/3932)
2. [PySINDy](https://github.com/luckystarufo/pySINDy)
