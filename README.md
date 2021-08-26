# Kaggle_HousingFutureSales
### Link for competition: https://www.kaggle.com/c/house-prices-advanced-regression-techniques/

==============================================================================================  
#### In this notebook, we will explore the famous Boston Housing dataset avaialble through Kaggle for regression task (predicting the future sales of a house). 

This competition is beginner-friendly and is focused on getting your hands dirty in EDA (Exploratory Data Analysis) with various techniques on data inspection, creation, trasnformation and selection. 

We performed simple outlier removal based on trend analysis of the response variable, and then focused on checking sensible variables (especially nominal and ordinal) to perform detailed category-based imputation with pandas groupby and nearest neighbor. 

We extracted the sensible variables by checking color-coded 2d scatter plots to analyze if a categorical variable (color) significantly affects the response variable. 

We also created simplified (chunked) categorical values to reduce the complexity of the input and hence that of the model for a comparison to see if this tradeoff is worthwhile. 

We then also look for possible transformation needed for normality on the response variable (required for linear regression, but not necessary for neural network or svm).

We have experimented with Lasso, Elastic Net, Kernel Ridge, Gradient Boosted Trees, XGB and LGBM (last three all tree-based models). We also included Ensemble Learning (Averaging vs. Stacking) as alternative models anfd that our stacking module (meta-learning) performs the best (given its flexibility and size). 

For further details on EDA, model construction and analysis, please see notebook. 

Components of this notebook are inpisred by common methodoligies implemented in the Kaggle community. 

Happy Kaggle exploration!
====================================================================================================
## Sample plots in notebook on EDA:

### Outlier filtering
<div style="text-align:center"><img src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/outlier_house.png?" data-canonical-src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/outlier_house.png?" width="500" height="350" /></div>


### Housing price over years constructed
<div style="text-align:center"><img src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/Year_based_price_trend.png?" data-canonical-src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/Year_based_price_trend.png?" width="1000" height="450" /></div>

### Categorical variable 3d scatter
<div style="text-align:center"><img src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/variable_selection_cate.png?" data-canonical-src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/variable_selection_cate.png?" width="800" height="600" /></div>

### Variable Transformation
<div style="text-align:center"><img src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/Variable Transformation.png?" data-canonical-src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/Variable Transformation.png?" width="700" height="500" /></div>

### Variable importance plot (RF-based)
<div style="text-align:center"><img src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/RF_Variable_Importance.png?" data-canonical-src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/RF_Variable_Importance.png?" width="500" height="425" /></div>

### Final selected variable R2 plot (ordinal and numerical) with response variable
<div style="text-align:center"><img src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/Final_R2_plot.png?" data-canonical-src="https://github.com/YSun-syptk/Kaggle_HousingFutureSales/blob/main/blob/Final_R2_plot.png?" width="500" height="425" /></div>
