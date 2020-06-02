# Fully Connected Neural Network

## Model Architecture
<p align="center">
  <img src="https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/FCNN%20architecture.PNG">
</p>

+ **Input features** - Angle theta, Angle phi, and Mask
+ **Outputs** - 1/pT, Bending angles, Pattern Straigntness, and Binary Classification ( i.e. >25 GeV or <25 GeV)
+ **Loss functions** - MSE, MSE, MSE and Focal Loss (as it can handle class imbalances)
+ **Feature Preprocessing** - <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Standardization to Angle theta and Angle phi<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Linear scaling between zero and one to Bending angles, Pattern Straigntness<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Filling Empty/Missing values with zeroes
+ **Validation and Out of Fold Predictions** - 10 even-random-splits of data | 8 for training | 1 for validation | 1 for out-of-fold-predictions | [(detailed image)](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/validation_scheme.png)

## Results and Comparision

+ **1/pT Distribution**

True | LightGBM | FCNN
--- | --- | ---
![True dist](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/raw/master/images/dist-True.png) | ![LightGBM dist](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/dist-LightGBM.png) | ![FCNN dist](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/dist-batchnorm.png)

+ **Classification Report - Regression Head**

LightGBM | FCNN
![Classification Report LightGBM](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/LightGBM%20classification%20Report.PNG) | ![Classification Report FCNN](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/FCNN%20classification%20report%20regression%20head%20dropout.PNG)

+ **Classification Report FCNN - Classification Head**
<p align="center">
  <img src="https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/FCNN%20classification%20report%20classification%20head%20batchnorm.PNG">
</p>

### Comparision - Rate and Efficiency
Rate Ratio | Efficiencies for pT>25 GeV
--- | ---
![Rate Ratio](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/Rate%20ratio%20FCNN-LightGBM.png) | ![Efficiencies](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/Efficiency-LightGBM-FCNN.png)
