# LightGBM
+ **Input -** Angle theta, Angle phi, Bending Angle, TimeInfo, RingNumber, Front/Rear hit, Mask, PatternStraightness, Zone, and MedianTheta
+ **Output -** 1/pT
+ **Loss -** MSE
+ **HyperParameters optimized -** Learning Rate, Bagging fraction, Min child Sample, Max Depth, Lambda 1, Lambda 2, Feature fraction and Early Stopping Rounds
+ **Obtained Optimized Values -** 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Learning Rate :  0.27622648017994983
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Bagging fraction : 0.6652163201643659
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Min child Sample : 98
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Max Depth : 39
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Lambda 1 : 0.5572619319129042
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Lambda 2 : 0.4093734644841744
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Feature fraction : 0.7657601467713301
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Early Stopping : 76

## Bayesian Hyperparameter Optimization
<p align="center">
  <img src="https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/LightGBM-SearchSpace-Projections.png">
</p>
<p align="center">
  Projection of Hyperparameter Space onto various axes
</p>
