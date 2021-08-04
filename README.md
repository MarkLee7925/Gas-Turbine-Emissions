# Gas Turbine Emissions

In this project, the objective is to predict the trends of several greenhouse gases, namely Carbon Monoxide (CO) and Nitrogen Oxides (NOx), in a gas turbine and their effects on its overall energy yield. This turbine was located in the northwestern region of Turkey. The results of this project can be used to determine the overall efficiency and environmental effects of greenhouse gases caused.

## Dataset

The data contains 36,733 instances of 11 sensor measurements aggregated over one hour collected over a five-year period between 2011 and 2015. The original raw dataset can be obtained from the UCI Machine Learning Repository (see References). A brief description of each measurement can be found in the "gas_turbine_features.txt" file located in the "data" folder as well as all datasets. For convenience, all five datasets were manually merged into one file (gt_2011-15.csv) in order to predict the overall trends for five years. Alternatively, this project can also used to predict the results for each year.

## Results

This project utilized three standard Machine Learning Regression models and one Deep Neural Network model. The k-fold cross-validated training (CV) and testing/validation (Val.) results for each optimized standard model are presented below:

<table border = "1">
  <thead>
    <th colspan = "5">Final Regression Scores</th>
  </thead>
  <tbody>
    <tr>
      <td><b>Model</b></td>
      <td colspan='2'><b>R^2</b></td>
      <td colspan='2'><b>RMSE</b></td>
    </tr>
    <tr>
      <td><b></b></td>
      <td><b>CV</b></td>
      <td><b>Val.</b></td>
      <td><b>CV</b></td>
      <td><b>Val.</b></td>
    </tr> 
    <tr>
      <td><b>Linear Regression (LR)</b></td>
      <td>0.996</td>
      <td>0.996</td>
      <td>0.952</td>
      <td>1.000</td>
    </tr>
    <tr>
      <td><b>Decision Tree (DT)</b></td>
      <td>0.997</td>
      <td>0.997</td>
      <td>0.891</td>
      <td>0.896</td>
    </tr>
    <tr>
      <td><b>LightGBM (LGB)</b></td>
      <td>0.998</td>
      <td>0.998</td>
      <td>0.708</td>
      <td>0.761</td>
    </tr>
  </tbody>
</table>

For the Neural Network model, the results vary slightly due to the random nature of Deep Learning. Shown below are some sample results:

<table border = "1">
  <thead>
    <th colspan = "3">Sample Neural Network Regression Scores</th>
  </thead>
  <tbody>
    <tr>
      <td><b>Mean Absolute Error (MAE)</b></td>
      <td>0.580</td>
    </tr>
    <tr>
      <td><b>Mean Square Error (MSE)</b></td>
      <td>0.560</td>
    </tr>
    <tr>
      <td><b>Root Mean Square Error (RMSE)</b></td>
      <td>0.748</td>
    </tr>
    <tr>
      <td><b>R^2 Score</b></td>
      <td>0.998</td>
    </tr>
  </tbody>
</table>

## References:

- https://archive.ics.uci.edu/ml/datasets/Gas+Turbine+CO+and+NOx+Emission+Data+Set
- Heysem KAYA, Pınar TÜFEKCİ and Erdinç UZUN. 'Predicting CO and NOx emissions from gas turbines: novel data and a benchmark PEMS', Turkish Journal of Electrical Engineering & Computer Sciences, vol. 27, 2019, pp. 4783-4796, [Web Link]. Weblink: [Web Link]
