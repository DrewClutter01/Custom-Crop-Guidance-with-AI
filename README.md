# Custom-Crop-Guidance-with-AI
![dean-vallance-2rINCqTV76g-unsplash](https://github.com/user-attachments/assets/4420dfbf-7f59-4b8a-bed0-1f6d4f15df56)
The "Custom Crop Guidance with AI" project aims to help farmers maximize their crop yields by understanding crop's specific needs and nutrients. We used the [Crop Recommendation Dataset](https://www.kaggle.com/datasets/varshitanalluri/crop-recommendation-dataset?select=Crop_Recommendation.csv) to gather our data and utilized a Logistic Regression and Random Forest Classifier on the dataset to tackle our problem.

# Business Understanding and Data Understanding
A lack of understanding about environmental conditions and nutrients can be detrimental to farmers' success because different crops require different nutrients​. The data set was entirely composed of numerical data excluding the target variable. Listed below are the variables from the data set.

**Key Factors**: Nitrogen, Phosphorus and Potassium 

**Environmental Variables**: Temperature, Humidity, pH_Value, Rainfall

**Target Variables**: Crop

 
The three primary macronutrients essential to successful crop growth are [Nitrogen, Phosporus and Potassium](https://cropnuts.com/nitrogen-phosphorus-potassium-npk-fertilizers/).
![npk-illustration-720x480](https://github.com/user-attachments/assets/73fd6cf6-3fce-461d-aaee-23c75978e80e)

[Nitrogen](https://www.corteva.ca/en/resources/agronomy-hub/understanding-nitrogen0.html) is important to crops because in most crops it can be the main nutrient to affect yield and plant health. It is also an essential component of the structure of amino acids, proteins, chlorophyll (and more) in crops.

[Phosphorus](https://taurus.ag/importance-of-phosphorus-to-crops/#:~:text=Ten%20ways%20phosphorus%20aids%20in%20plant%20growth%20and,earlier%20maturity%208%20Increases%20disease%20resistance%20More%20items) is a main ingredient in ATP and a central component of DNA & RNA (which are needed to build proteins). It is also required by the plant from the seedling stage through to maturity and has an impact on crop quality and yield.

[Potassium](https://extension.umn.edu/phosphorus-and-potassium/potassium-crop-production) is involved with the enzyme activation within the plant, which also affects the ATP production. In crops it also plays a role in helping regulate the exchange of water vapor, oxygen and carbon dioxide (the opening and closing of the stomata).

[Soil p_H](https://www.nrcs.usda.gov/sites/default/files/2022-11/pH%20-%20Soil%20Health%20Guide_0.pdf) is an important indicator for the suitability of a soil for plant growth. According to the USDA for most crops pH of 6 to 7.5 is optimal. If the pH levels are too high are low, it can lead to a deficiency of nutrients

[Humidity](https://www.pthorticulture.com/en-us/training-center/how-does-humidity-influence-crop-quality) ensures optimal transpiration which is essential for nutrient uptake and effective photosynthesis, ultimately impacting plant growth and crop yield.

[Rainfall](https://www.nicheagriculture.com/how-rainfall-affects-crop-health/) supplies the water necessary for plants to absorb and distribute nutrients essential for their survival and growth. Additionally, it plays a role in reducing soil erosion and enhancing soil fertility.

### Modeling and Evaluation
We recommend for our client to use the logistic regression model. It preformed quite well, 98% accuracy on the dedicated testing data. This model also showcased 100% accuracy achieved in 4 specific clusters, indicating perfect classification for those clusters. Additionally,l ogistic regression models are quicker to train and make predictions than random forest classifiers

### Conclusion 
We recommend that our client use the logistic regression model. It performed quite well, achieving 98% accuracy on the dedicated testing data. This model also showcased 100% accuracy in four specific clusters, indicating perfect classification for those clusters. Additionally, logistic regression models are quicker to train and make predictions than random forest classifiers.


### Repository Navigation
This repository contains four folders: .ipynb_checkpoints, Data, Images, and Notebooks. The Data folder contains the original dataset as well as the clustered dataset. Within the Notebooks folder, you can find eight sub-folders. Each team member has their own sub-folder. Additionally, EDA-Clustering, LogReg, and RandomForest are the sub-folders that contain the code for the clustering justification, logistic regression model, and random forest model, respectively. The EDA done for the dataset can be found in these two folders: Nicole_Salas and Dorothy_Uriri_Akpovwa.

# Final notebok link: https://github.com/DrewClutter01/Custom-Crop-Guidance-with-AI/blob/main/report-notebook.ipynb
# Final Presentation link: https://github.com/DrewClutter01/Custom-Crop-Guidance-with-AI/blob/main/presentation.pdf

# Reproduction instructions
Prerequisties include: Python, Anaconda, Gitbash 

Software dependencies: 
sklearn.cluster - KMeans
sklearn.metrics - silhouette_samples, silhouette_score
matplotlib.cm
sklearn.preprocessing - MinMaxScaler, StandardScaler
sklearn.linear_model - LogisticRegression
sklearn.model_selection - train_test_split
sklearn.metrics - confusion_matrix, ConfusionMatrixDisplay
sklearn.model_selection - train_test_split, GridSearchCV
sklearn.preprocessing - MinMaxScalersklearn.linear_model - LogisticRegression
matplotlib - style
sklearn.tree -  DecisionTreeClassifier
sklearn.ensemble -  BaggingClassifier, RandomForestClassifier

Installation: 
1. Fork the repository 
2. Clone the repository using git clone and insert the copied url from the forking 
3. cd into what has been cloned  
4. Next open jupyter notebook and begin importing the software dependencies

Remember to make sure you have the latest version of all the software dependencies, and use the documentation if needed!
