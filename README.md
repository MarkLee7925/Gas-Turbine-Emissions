# Gas Turbine Emissions

Carbon emissions have always been a major concern for the environment and in our society. The rise of global warming and increased awareness of climate change have been major issues in the past several years. In this project, the objective is to predict the trends of several gas turbine sensor measurements, namely Carbon Monoxide (CO) and Nitrogen Oxides (NOx), and their effects on its overall energy yield. This turbine was located in the northwestern region of Turkey. The results of this project can be used to determine the overall efficiency and environmental effects of greenhouse gases caused.

## Dataset

The data contains 36,733 instances of 11 sensor measurements aggregated over one hour collected over a five-year period between 2011 and 2015. The original raw dataset can be obtained from the UCI Machine Learning Repository (see References). A brief description of each measurement can be found in the "gas_turbine_features.txt" file located in the "data" folder as well as all datasets. 

For convenience, all five datasets were manually merged into one .csv file (gt_2011-15.csv) in order to predict the overall trends for five years. Alternatively, this project can also used to predict the results for each year.

## Models

Data visualization techniques were employed to showcase the correlation and trends of the data features and how they relate to the overall energy yield (the dependent variable). Furthermore, the K-Means clustering algorithm (for unsupervised learning) was employed to help the viewer better understand certain data patterns and features by grouping them into clusters.

This project utilized the following models.

- Logistic Regresion (LR)
- Decision Tree (DT)
- LightGBM (LGB)
- Deep Neural Network (DNN)

## References:

- https://archive.ics.uci.edu/ml/datasets/Gas+Turbine+CO+and+NOx+Emission+Data+Set
- Heysem KAYA, Pınar TÜFEKCİ and Erdinç UZUN. 'Predicting CO and NOx emissions from gas turbines: novel data and a benchmark PEMS', Turkish Journal of Electrical Engineering & Computer Sciences, vol. 27, 2019, pp. 4783-4796, [Web Link]. Weblink: [Web Link]
