---
permalink: /
title: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Education
====
* M.Sc. in Data Science for Sustainability, National University of Singapore, Singapore, 2024 - 2025
* B.Sc. in Mathematical Sciences, University of Southampton, UK, 2021 - 2024
* Summer Institute in Beginners for Data Science, University of Hong Kong, Hong Kong SAR, 2023

Projects
====
* [AI Agents for Financial Trading](https://github.com/nusduck/QF5214_2025_G7_StockAgent)
  * An LLM-Driven Multi-Agent system for stock prediction and investment recommendation.
  * Multi agent design: fundamental agent, technical agent, sentiment agent, synthesis agent, planner for task routing, adjudicator for consistency and confidence checks
  * Data integration: market and fundamentals, news and reports, social sentiment, on the fly technical indicators including MA, RSI, MACD, Bollinger, ATR, ROC
  * Reliability: unified input and output contract, step level logs for prompts and tool IO, rate limit aware caching, retries and timeouts
  * Decisions and evaluation: signal fusion by scores, thresholds, or voting, backtests and reports for return, drawdown, win rate, factor exposure, scalable to multiple assets and frequencies
  * Productization: modular pipeline, config driven runs, front end friendly outputs for dashboards and demos, easy A/B comparisons

* [Automated ESG data Extraction and Performance Analytics](https://github.com/ariahuang314/groupproject)
  * An ESG analytics system using OCR, ESG-BERT, NER, and an LLM agent to extract KPIs from reports/news and benchmark companies.
  * End to end pipeline: PDF OCR, layout aware chunking, table parsing, NER for metrics and units, normalization, company and period resolution, topic and scope tagging, ontology mapping, deduplication
  * Models and rules: ESG BERT for section and sentence classification, NER plus patterns for numbers and units, LLM agent for normalization and taxonomy alignment
  * Data quality: confidence scoring, human in the loop review for low confidence items, step level logging for traceability
  * Analytics: coverage, consistency, and trend scores per company, sector benchmarks, simple dashboard for query and comparison
  * Reproducibility: pinned environments, Makefile and CI, seeds and caching to reduce variance

* [Deep Learning for Time Series Forecasting](https://github.com/jiaozijun666/DL-for-time-series-forecasting)
  * A modular toolkit that implements classical and deep models for time series forecasting with reproducible experiments and reports.
  * Models included: LGBM, Prophet, DLinear, LSTM, DARNN, Transformer
  * Datasets used in our study: air quality, energy, gait, metro traffic, productivity
  * Experiment flow: data prep and splits, config driven training, metric reporting and result export
  * Reproducibility: requirements file, fixed seeds, scripted runs and saved results
  * Evaluation: standard forecasting metrics and side by side comparisons across models

* [Machine Learning in Quantum Many-Body Physics (undergraduate thesis)](https://drive.google.com/file/d/13TPwP0Q4bkb2IvXgZR-k4CTegbUgCSc3/view?usp=drive_link)
  * Applying machine learning to represent and solve quantum many-body systems, focusing on neural-network quantum states, restricted Boltzmann machines, and tensor networks.
  * Topics: neural-network quantum states, RBM wavefunctions, tensor networks including MPS and PEPS, variational optimization, imaginary time evolution, quantum geometric metrics
  * Goals: learn ground-state wavefunctions, estimate energies, capture entanglement structure, compare RBM and tensor-network representations, discuss area-law versus volume-law behavior
  * Methods: variational ansatz with RBM and stochastic reconfiguration, layout of MPS and PEPS with SVD based contractions, iPEPS and iPEPO for imaginary time evolution, evaluation via relative energy error and fidelity
  * Findings: NQS can achieve controllable accuracy for ground-state energy with error scaling tied to hidden-unit density, and RBM states can emulate tensor-network states while allowing volume-law entanglement at larger sizes

Resume
====
[Latest CV](https://drive.google.com/file/d/1p65xDsLY66W1NKIsIvLm3sz0smJq-51S/view?usp=drive_link)
