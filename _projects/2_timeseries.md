---
layout: page
title: Resource-aware benchmarking of classical and deep time-series forecasters
description: Accuracy, deployment cost and noise robustness across five domains — and why the most accurate model is often none of the ones you would deploy.
img: assets/img/timeseries.png
importance: 2
category: research experience
---

**Course research project, National University of Singapore · January – May 2025** · [Code](https://github.com/jiaozijun666/DL-for-time-series-forecasting)

{% include figure.liquid loading="eager" path="assets/img/timeseries.png" class="img-fluid rounded z-depth-1" alt="Study diagram: five domain datasets, two classical and four deep forecasters, evaluated on accuracy, scalability, generalization and robustness." %}
<div class="caption">Five domains, six forecasters, four evaluation axes.</div>

**Study design:** Six forecasters — Prophet, LightGBM, DLinear, LSTM, Transformer and DARNN — benchmarked on five univariate series drawn from energy consumption, air quality, manufacturing productivity, urban traffic and biomedical gait. Each series gets its own preprocessing pipeline: imputation, winsorisation, calendar and event features, and train-set-only scaling to prevent leakage.

**Evaluation beyond error:** Every model–dataset pair is scored on four axes rather than one: forecast error (MAE, RMSE, MAPE, sMAPE), decision-relevant accuracy (directional and threshold accuracy), deployment cost (training time, peak memory, early stopping), and noise robustness — the change in MAE under additive Gaussian perturbation at σ = 0.05.

**Finding:** Peak memory varied by roughly three orders of magnitude across models, from tens of gigabytes for the attention-based recurrent model down to tens of megabytes for the linear and gradient-boosting baselines. The most accurate model on a given series was frequently neither the cheapest nor the most noise-stable: LightGBM degraded by up to 63% in MAE under perturbation on the smallest series, while the recurrent models stayed within 1.2%, and several deep models fell below 0.50 directional accuracy on that same series. The conclusion is that forecaster selection should be posed against deployment constraints, not as error minimisation alone.

**Individual contribution:** Focused on the Prophet and Transformer components of the benchmark, including preprocessing, model implementation, experiment configuration, and evaluation of forecasting accuracy and robustness across multiple time-series datasets.

**Methods:** Prophet · LightGBM · DLinear · LSTM · Transformer · DARNN · perturbation-based robustness testing
