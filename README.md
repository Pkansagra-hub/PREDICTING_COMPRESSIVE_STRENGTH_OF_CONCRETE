# PREDICTING_COMPRESSIVE_STRENGTH_OF_CONCRETE
Predicting compressive strength of concrete from multivariate dataset.

Concrete is widely used in construction all over the world. It is produced from different components such as water, cement and so on.
For __quality control and as a measure of performance, 28-day compressive strength test is mandatory__ for design and construction code requirements
__The Compressive Strength of Concrete determines the quality of Concrete.__This is generally determined by a standard crushing test on a concrete cylinder.
This requires engineers to build small concrete cubes with different combinations of raw materials and test these cylinders for strength variations with a change in each raw material.
The test is based on standard compression which is very complicated, time consuming and subject to experimental error.
More importantly, __if the concrete fails the test after such a long wait, there might be no way to effect an adjustment since it is already placed.__

Therefore, estimation of compressive strength well before 28 day is highly desired and widely practiced since it offers many advantages.

1. It allows advanced scheduling of operations such as prestressing and formwork removal resulting in improved efficiency.

2. It also enhances quality control as structures become more durable due to avoidance of excessive loading at early age.

Many methods exist to predict and estimate concrete strength well before 28 days.Prominent among them is the Abrahams Law which is a linear equation relating concrete strength and its water to cement ratio. In reality, __the relationship between concrete strength and its constituents material is highly nonlinear__ and as such relation as __Abrahams law fail to adequately represent this complex relationship__ and fall short in generalizing to previously unseen data.


However, artificial intelligence has proven itself to be a versatile tool in learning complex patterns and is widely used in various fields for classification and regression.
_Hence, a widely proposed method is the use of artificial neural network (ANN) in concrete strength prediction and the most widely deployed ANN network is the back propagation network_.__Hence, a widely proposed method is the use of artificial neural network (ANN) in concrete strength prediction and the most widely deployed ANN network is the back propagation network.However, back propagation networks suffered from local minima resulting in instability in the developed model. The convergence to local minima results from the optimization objective of ANN which is multimodal in nature. This instability manifest itself in the fact that different sets of training data produce different models impacting on the ability of the developed model in generalizing to previously unseen data.__

__However,SVM is a very efficient and stable algorithm which is now being applied in many fields. It exhibit good generalization performance in real-world scenarios where it often outperform many other techniques used in predictions and classifications. Its sound and solid mathematical foundation ensured its adaptation and optimization to varying data analysis problems__

# 1. Problem Statement
Predicting Compressive Strength of Concrete given its age and quantitative measurements of ingredients.

# 2. Data Description
Data is obtained from UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/Concrete+Compressive+Strength

Number of instances - 1030
Number of Attributes - 9
Attribute breakdown - 8 quantitative inputs, 1 quantitative output

## Attribute information
* Inputs
  * Cement
  * Blast Furnace Slag
  * Fly Ash
  * Water
  * Superplasticizer
  * Coarse Aggregate
  * Fine Aggregate
   (All above features measured in kg/$m^3$)
  * Age (in days)
* Output
  * Concrete Compressive Strength (Mpa)
# 3. Modelling and Evaluation

## Algorithms used
* Linear regression
* Lasso regression
* Ridge regression
* Decision Trees
* Random Forests
* Metric - Since the target variable is a continuous variable, regression evaluation metric RMSE (Root Mean Squared Error) and R2 Score (Coefficient of Determination) have been used.
