# recommendation_engine
Recommendation engine for product recommendations on Amazon dataset

In this assignment, we’re creating a recommendation engine for product recommendations on Amazon.com. The dataset we selected contains information about musical instruments.

After performing the exploratory data analysis and doing the required pre-processing steps, we compare the performance of multiple models. The models can be divided into 2 areas:
1.	collaborative filtering recommendation engines
2.	content-based recommendation engines

With collaborative filtering, we fit the following models:
1.	KNN - achieving RMSE of 0.8754
2.	SVD - achieving RMSE of 0.8745
3.	SVD++ - achieving RMSE of 0.8742

With content-based models, we fit the following model:
1.	TF-IDF - achieving RMSE of 3.6176

	Based on the performance, we ended up selecting the SVD model, which ended up getting 0.8578 RMSE on our testing set. The reason we selected it over SVD++, which performed better on the training set, is that SVD took significantly less time to compute (approx. 95% less time than SVD++). While the model performance is certainly important, we also have to consider the time, as once deployed, we would need to make sure that the recommendations are readily available to the users browsing the store.
 

