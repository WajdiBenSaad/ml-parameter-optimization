# ml-parameter-optimization
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://twitter.com/wajdi_bs)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://twitter.com/wajdi_bs) [![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://twitter.com/wajdi_bs)  [![Open Source Love png1](https://badges.frapsoft.com/os/v1/open-source.png?v=103)](https://twitter.com/wajdi_bs)


Hyperparameter optimization for machine learning algorithms

## Getting started

### Prerequisites

Make sure you have up-to-date versions installed of:

  - lightgbm
  - numpy
  - pandas
  - scikit-learn
  - scipy
  - xgboost

### Installation

Clone the repository in your local workspace:

```
git clone https://github.com/arnaudvl/ml-parameter-optimization
```

## Functionality

There are 3 modules in mlopt that can be used for hyperparameter tuning: lgb_tune, sklearn_tune and xgb_tune.

sklearn_tune covers the adaboost, k-nearest neighbour, logistic regression, random forest and support vecor machine algorithms. Calling the function tune_params starts the tuning process using gridsearch.

The lightgbm (lgb_tune) and xgboost (xgb_tune) algorithms cannot efficiently be tuned using gridsearch given the large amount of hyperparameters. As a result, the parameters are tuned iteritavely. See the example for a full explanation.
