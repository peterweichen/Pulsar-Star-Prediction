# Pulsar-Star-Prediction
Pulsar Star Prediction in SAS

## Introduction

This report develops a model trying to predict the likelihood of one observation being Pulsar star. The dataset was collected during the High Time Resolution Universe Survey and describes characteristics of a sample of pulsar star candidates. We build a regression model to identify potential pulsar star in the universe. Each candidate could be potentially identified as a real pulsar without additional information. However, according to the publisher, in practice, “almost all detections are caused by radio frequency interference (RFI) and noise, making legitimate signals hard to find” and rendering outcomes of True Negative classification. Therefore, this report targets at assisting in accurately predicting real pulsar stars using analytical constructed model. Besides, this would be able to help facilitate rapid analysis significantly by automatically labeling pulsar candidates.


## Data

The dataset was obtained from [Kaggle](https://www.kaggle.com/). It is a community to hold data science competitions, where publishers provide their data in an accessible format. The particular dataset we use is designed for “Predicting a Pulsar Star” project last updated on 2018-05-09. (https://www.kaggle.com/pavanraj159/predicting-a-pulsar-star) It describes a sample of pulsar candidates collected during the High Time Resolution Universe Survey. Pulsars are a rare type of Neutron star that produce radio emission detectable on Earth.  

Overall, this dataset contains 16,259 spurious examples caused by RFI/noise (negative examples), and 1,639 real pulsar examples(positive examples). The observations would be 17,898 in total.  

There are 9 variables within, including eight continuous variables and one categorial variable. The first four continuous variable are simple statistics drawn from integrated pulse profile. This describe a longitude-resolved version of the signal that has been averaged in both time and frequency, which is used to detect a real pulsar star.  

The remaining four continuous variables were obtained from the DM-SNR curve. (DM represents the "dispersion measure" and increases with distance and electron density between Earth and pulsar; SNR stands for the signal-to-noise ratio, increasing with integration time. Both are good indicators to distinguish pulsar from other kinds of stars.) The dependent variable here we use is the categorial variable “target_class,” denoting whether the observation is predicted as a pulsar star, with (1) for pulsar star, and (0) for not a star. There are no missing values observed in this dataset. 

