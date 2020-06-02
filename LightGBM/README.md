# LightGBM
+ **Input -** Angle theta, Angle phi, Bending Angle, TimeInfo, RingNumber, Front/Rear hit, Mask, PatternStraightness, Zone, and MedianTheta
+ **Output -** 1/pT
+ **Loss -** MSE
+ **HyperParameters optimized -** Learning Rate, Bagging fraction, Min child Sample, Max Depth, Lambda 1, Lambda 2, Feature fraction and Early Stopping Rounds
+ **Obtained Optimized Values -** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Learning Rate :  0.27622648017994983<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Bagging fraction : 0.6652163201643659<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Min child Sample : 98<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Max Depth : 39<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Lambda 1 : 0.5572619319129042<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Lambda 2 : 0.4093734644841744<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Feature fraction : 0.7657601467713301<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Early Stopping : 76
+ **Projection of Hyperparameter Space (Constructed during Bayesian HyperParameter Search) onto various axes -**
<p align="right">
  <img src="https://github.com/PRATEEKKUMARAGNIHOTRI/CMS-trigger/blob/master/images/LightGBM-SearchSpace-Projections.png">
</p>
