# Fully Connected Neural Network

## Model Architecture
![Architecture](https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/FCNN%20architecture.PNG)

+ **Input features** - Angle theta, Angle phi, and Mask
+ **Outputs** - 1/pT, Bending angles, Pattern Straigntness, and Binary Classification ( i.e. >25 GeV or <25 GeV)
+ **Loss functions** - MSE, MSE, MSE and Focal Loss (as it can handle class imbalances)
+ **Feature Preprocessing** - <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ##Standardization## - Angle theta and Angle phi<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Linear scaling from Min to Max between zero and one - Bending angles, Pattern Straigntness<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Missing values - zero
