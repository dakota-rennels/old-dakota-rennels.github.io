## Oklahoma State Data Platform

**Project description:** OMES Data-Driven Services has undertaken an initative to create a State Data Platform to provide transparency, security, and accountability of state data while supporting state agencies with various tools, software, infastructure, and services. The main goal of the platform is to connect state agencies who offer services to the public such as: food benefits, school programs, licensing programs, and mental healh; with a platform for seemless data sharing between state agencies. This hub-and-spoke model is will allow the State of Oklahoma to work together to improve the lives of Oklahomans by improving programs through more detailed analytics, while ensuring all information is protected and secure. For a bit more of an introduction into the initative, please watch the following video:
[![OMES collaborates with state agencies to utilize data and drive service efficiencies for Oklahomans](/images/Youtube_Thumbnail_SDP.png)](https://youtu.be/ZNxmbjxT_Uo "OMES collaborates with state agencies to utilize data and drive service efficiencies for Oklahomans")

### 1. Perform descriptive statistics and EDA on provided data.

Initial analysis on the dataset was performed to confirm the correct data types were assigned to variables, confirm no missing data in the dataset, and verify the correct target variable for classification and prediction, respectively.

<html>
<body>

<h2>Descriptive Statistics</h2>

<table style="width:100%">
  <tr>
    <th>Variable</th>	
    <th>Missing</th>
    <th>Count</th>
    <th>Minimum</th>
    <th>Maximum</th>
    <th>Mean</th>
    <th>Standard Deviation</th>
    <th>Skewness</th>
  </tr>
  <tr>
    <td>damt</td>
    <td>0</td>
    <td>6002</td>
    <td>0</td>
    <td>27</td>
    <td>7.209</td>
    <td>7.3612</td>
    <td>0.11698</td>
  </tr>
   <tr>
    <td>donr</td>
    <td>0</td>
    <td>6002</td>
    <td>0</td>
    <td>1</td>
    <td>0.499</td>
    <td>0.5</td>
    <td>0.00467</td>
  </tr>
  <tr>
    <td>gifa</td>
    <td>0</td>
    <td>6002</td>
    <td>1.89</td>
    <td>72.27</td>
    <td>11.678</td>
    <td>6.5281</td>
    <td>1.74146</td>
  </tr>
  <tr>
    <td>gifdol</td>
    <td>0</td>
    <td>6002</td>
    <td>23</td>
    <td>1974</td>
    <td>115.8</td>
    <td>86.538</td>
    <td>6.09138</td>
  </tr>
  <tr>
    <td>gifl</td>
    <td>0</td>
    <td>6002</td>
    <td>3</td>
    <td>642</td>
    <td>22.981</td>
    <td>29.3964</td>
    <td>7.18035</td>
  </tr>
  <tr>
    <td>gifr</td>
    <td>0</td>
    <td>6002</td>
    <td>1</td>
    <td>173</td>
    <td>15.654</td>
    <td>12.4246</td>
    <td>2.67345</td>
  </tr>
  <tr>
    <td>hv</td>
    <td>0</td>
    <td>6002</td>
    <td>51</td>
    <td>710</td>
    <td>183.905</td>
    <td>72.7705</td>
    <td>1.4889</td>
  </tr>
  <tr>
    <td>inc</td>
    <td>0</td>
    <td>6002</td>
    <td>1</td>
    <td>7</td>
    <td>3.939</td>
    <td>1.4019</td>
    <td>-0.01495</td>
  </tr>
  <tr>
    <td>incavg</td>
	<td>0</td>	
	<td>6002</td>
	<td>14</td>
	<td>287</td>
	<td>56.789</td>
	<td>24.833</td>
	<td>1.85779</td>
  </tr>
  <tr>
    <td>incmed</td>
	<td>0</td>	
	<td>6002</td>
	<td>3</td>	
	<td>287</td>
	<td>43.949</td>
	<td>24.6644</td>
	<td>2.00492</td>
  </tr>
  <tr>
    <td>kids</td>
	<td>0</td>	
	<td>6002</td>
	<td>0</td>	
	<td>5</td>
	<td>1.584</td>
	<td>1.4125</td>
	<td>0.39406</td>
  </tr>
  <tr>
    <td>lag</td>
	<td>0</td>	
	<td>6002</td>
	<td>1</td>	
	<td>34</td>
	<td>6.319</td>
	<td>3.6414</td>
	<td>2.41056</td>
  </tr>
  <tr>
    <td>low</td>
	<td>0</td>	
	<td>6002</td>
	<td>0</td>
	<td>87</td>
	<td>13.885</td>
	<td>13.1046</td>	
	<td>1.35139</td>
  </tr>
  <tr>
    <td>mdon</td>
	<td>0</td>	
	<td>6002</td>
	<td>5</td>	
	<td>40</td>
	<td>18.789</td>
	<td>5.5963</td>
	<td>1.1176</td>
  </tr>
  <tr>
    <td>npro</td>
	<td>0</td>	
	<td>6002</td>
	<td>2</td>	
	<td>164</td>
	<td>61.354</td>
	<td>30.3052</td>
	<td>0.28319</td>
  </tr>
  <tr>
    <td>ownd</td>
	<td>0</td>	
	<td>6002</td>	
	<td>0</td>
	<td>1</td>
	<td>0.885</td>
	<td>0.3196</td>
	<td>-2.40714</td>
  </tr>
  <tr>
    <td>sex</td>
	<td>0</td>
	<td>6002</td>
	<td>0</td>
	<td>1</td>
	<td>0.608</td>
	<td>0.4883</td>
	<td>-0.44168</td>
  </tr>
  <tr>
    <td>wlth</td>
	<td>0</td>	
	<td>6002</td>
	<td>0</td>	
	<td>9</td>	
	<td>7.023</td>	
	<td>2.331</td>	
	<td>-1.46091</td>
  </tr>
</table>
</body>
</html>

### 2. Build and run classification models.
The models were assessed on its overall accuracy (misclassification rate) while observing sensitivity and specificity of the models. donr was the variable used to identify a donor. It is marked '1' if the individual donated and '0' if they did not donate. Four main types of models were tested: Naive Bayesian, Neural Network, Tree-based, and KNN. 

### 3. Build and run prediction models.
The models were assessed on its overall accuracy (misclassification rate) while observing sensitivity and average squared error of the models. damt was the variable used to identify the predicted amount a donor will donate. Four main types of models were tested: Polynomial Linear Regression, Tree-based Regressor, and Neural Network.

### 4. Provide a summary of analysis and detail limitations.

The Neural Networks in both the classification and prediction models provided the best models for deployment. Using the models, an estimated 76% improvement in cost effectiveness is estimated. The estimated percent is based on the estimated donation amount from each predicted donor. Limitaions in the data consist of limited records to train and test the model while more variables could have been analyzed to fine tune a more accurate model. More detailed location data was withheld from the data team that could have been beneficial to regional analysis and donation prediction. Using the new data from the upcoming marketing campaign will detail how accurate the predicting power of the model is and can be used to fine tune the model for future usage.

For more details see [Report via PDF](/SAS/Nonprofit_marketing_report.pdf).
