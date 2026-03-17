<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/hanshang/CLR_vs_CDF_transformation">
    <img src="MQ.png" alt="Logo" width="400" height="400">
    <img src="City.png" alt="Logo" width="400" height="200">
  </a>

<h3 align="center">Forecasting age distribution of deaths across countries: Life expectancy and annuity valuation</h3>

</div>

# Forecasting age distribution of deaths across countries: Life expectancy and annuity valuation
Multi-country comparison of life-table death counts (dx) between the centered log-ratio and cumulative distribution function transformations

<!-- ABOUT THE PROJECT -->
## Abstract

<p align="justify">
For modeling and forecasting the age distribution of death counts, we revisit two \textit{one-to-one} mapping transformations, namely the cumulative distribution function and the centered log-ratio in compositional data analysis. Between the two transformations, the cumulative distribution function provides a scale-free way to visualize the gender gap and cross-country heterogeneity in the probability of dying between sexes and countries. Drawing on age-specific period life-table death counts from 24 countries in the Human Mortality Database (2025), we assess and compare the point and interval forecast accuracy of the two transformations, using the same forecasting method. Enhancing the forecast accuracy of period life-table death counts holds significant value for demographers, who rely on such forecasts to estimate survival probabilities and life expectancy, and for actuaries, who use them to price annuities across various entry ages and maturities.
<br />
</p>

### Main Results
The R script files in the `R Code` folder should be used in the following order:
1. load_package.R: load R packages
2. transformation.R: CLR and CDF transformations
3. data.zip: unzip the data folder containing the age distribution of death counts from the 24 countries in the Human Mortality Database
4. read_data.R: read data files
5. point_forecast_compar.R: point forecast comparison based on the Kullback-Leibler and Jensen-Shannon divergences
6. interval_forecast_compar_PI_80.R: interval forecast comparison based on the coverage probability difference between the nominal and empirical coverage probabilities and mean interval score at the 80% nominal coverage probability.
7. interval_forecast_compar_PI_95.R: interval forecast comparison based on the coverage probability difference between the nominal and empirical coverage probabilities and mean interval score at the 95% nominal coverage probability.
8. annuity_calculation.R: based on the 50-years-ahead out-of-sample point forecasts, we determine the annuity prices for various entry ages and maturities.
9. annuity_calculation_interval_PI_80.R: based on the 50-years-ahead out-of-sample interval forecasts at the 80% nominal coverage probability, we determine the lower and upper bounds of the annuity prices for various entry ages and maturities.
10. annuity_calculation_interval_PI_95.R: based on the 50-years-ahead out-of-sample interval forecasts at the 95% nominal coverage probability, we determine the lower and upper bounds of the annuity prices for various entry ages and maturities.
11. save_function.R: R function for saving figures

## Contact
arXiv link: [https://arxiv.org/abs/2507.04303](https://arxiv.org/abs/2507.04303)

Han Lin Shang - hanlin.shang@mq.edu.au

Steven Haberman - s.haberman@citystgeorges.ac.uk

<br />
    <a href="https://github.com/hanshang/CLR_vs_CDF_transformation"><strong>Explore R code »</strong></a>
<br />
