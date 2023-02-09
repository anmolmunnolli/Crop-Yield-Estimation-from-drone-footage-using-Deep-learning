# Crop-Yield-Estimation-from-drone-footage-using-Deep-learning
To accurately predict crop yield in a given land using the drone footage and deep learning techniques at real-time. The predicted values will benefit in estimating yield return, better resource and investment planning, efficient usage of land area and smart farming.
![image](https://user-images.githubusercontent.com/76611893/217705862-cdee424c-11c1-44a9-a4ef-c4fb2c9b908b.png)
![image](https://user-images.githubusercontent.com/76611893/217706019-39349b86-702b-48ae-b264-64087e0069d8.png)

Data Acquisition: The video length is divided into equal sectors. Frames from each sector is considered using a Timeframe defined. Consider a land divided into sectors to detect the amount of crops per sector.

Data cleaning and Transformation will be performed on these frames stored in a google drive folder. Splitting of data will be done as 60%-training, 20%- validation and 20%- testing. ii) Object Detection: Pre-processed frames are sent to the Faster R-CNN model, to identify the total detected boxes of crop produce in the field. The fasterCNN model is trained on existing labeled images of a particular crop

Regression analysis: The number of Total detected boxes in a land is added as an attribute to other parameters like soil type, land area, etc to perform regression analysis. We plan to use 4 regression models: Random Forest Regressor, Gradient Boosting Regressor, Support Vector Regressor and Decision Tree Regressor. The best model is selected depending on the evaluation metrics such as R-Squared (R2).The net crop produce in a given land, considering relevant attributes and detected boxes, is predicted by the regression model

Optimization and Acceptance of results: Statistical analysis such as Standard deviation and variance is performed on the predicted results. If the error rate and the estimation metrics are satisfactory, the results and the model is accepted. Hyperparameter Tuning is performed if the results are unsatisfactory and the model is trained again to yield better results.
