<p>&nbsp;</p>
<h1>Housing Price Prediction using Machine Learning</h1>
<p>This project predicts housing prices using a machine learning model. It includes data preprocessing, feature engineering, model training, and evaluation. The model is built using Python and popular libraries such as <code>scikit-learn</code>, <code>pandas</code>, and <code>matplotlib</code>.</p>
<h2>Table of Contents</h2>
<ul>
<li><a href="#project-overview">Project Overview</a></li>
<li><a href="#dataset">Dataset</a></li>
<li><a href="#features">Features</a></li>
<li><a href="#installation">Installation</a></li>
<li><a href="#usage">Usage</a></li>
<li><a href="#model-evaluation">Model Evaluation</a></li>
<li><a href="#results">Results</a></li>
<li><a href="#contributing">Contributing</a></li>
<li><a href="#license">License</a></li>
</ul>
<h2 id="project-overview">Project Overview</h2>
<p>The goal of this project is to predict housing prices based on various features such as location, number of rooms, population, and more. The model uses a <strong>Gradient Boosting Regressor</strong> and includes advanced techniques like feature engineering, hyperparameter tuning, and cross-validation.</p>
<h2 id="dataset">Dataset</h2>
<p>The dataset used in this project is the <strong>California Housing Dataset</strong>, which contains information about housing districts in California. It includes features such as:</p>
<ul>
<li><code>longitude</code>, <code>latitude</code>: Geographic location of the district.</li>
<li><code>total_rooms</code>: Total number of rooms in the district.</li>
<li><code>total_bedrooms</code>: Total number of bedrooms in the district.</li>
<li><code>population</code>: Population of the district.</li>
<li><code>households</code>: Number of households in the district.</li>
<li><code>median_income</code>: Median income of households in the district.</li>
<li><code>median_house_value</code>: Median house value for households in the district (target variable).</li>
<li><code>ocean_proximity</code>: Proximity to the ocean (categorical feature).</li>
</ul>
<p>The dataset is available <a href="https://raw.githubusercontent.com/ageron/handson-ml2/master/datasets/housing/housing.csv" target="_blank" rel="noopener">here</a>.</p>
<h2 id="features">Features</h2>
<ul>
<li><strong>Feature Engineering</strong>:
<ul>
<li>Added new features: <code>rooms_per_household</code>, <code>bedrooms_per_room</code>, and <code>population_per_household</code>.</li>
</ul>
</li>
<li><strong>Data Preprocessing</strong>:
<ul>
<li>Handled missing values using median imputation.</li>
<li>Standardized numeric features.</li>
<li>Encoded categorical features using One-Hot Encoding.</li>
</ul>
</li>
<li><strong>Model Training</strong>:
<ul>
<li>Used a <strong>Gradient Boosting Regressor</strong> for prediction.</li>
<li>Performed hyperparameter tuning using <strong>GridSearchCV</strong>.</li>
</ul>
</li>
<li><strong>Model Evaluation</strong>:
<ul>
<li>Evaluated the model using <strong>Mean Absolute Error (MAE)</strong> and <strong>R&sup2; Score</strong>.</li>
<li>Visualized feature importance.</li>
</ul>
</li>
</ul>
<h2 id="installation">Installation</h2>
<p>To run this project, you need to install the required Python libraries. You can do this using <code>pip</code>:</p>
<pre><code>pip install pandas numpy scikit-learn matplotlib seaborn joblib</code></pre>
<h2 id="usage">Usage</h2>
<ol>
<li>Clone the repository:
<pre><code>git clone https://github.com/ehsanmns/housing-price-prediction.git
cd housing-price-prediction</code></pre>
</li>
<li>Run the Jupyter Notebook or Python script:
<pre><code>jupyter notebook housing_price_prediction.ipynb</code></pre>
or
<pre><code>python housing_price_prediction.py</code></pre>
</li>
<li>The script will:
<ul>
<li>Load the dataset.</li>
<li>Preprocess the data.</li>
<li>Train the model.</li>
<li>Evaluate the model and display results.</li>
</ul>
</li>
</ol>
<h2 id="model-evaluation">Model Evaluation</h2>
<p>The model was evaluated using the following metrics:</p>
<ul>
<li><strong>Mean Absolute Error (MAE):</strong> <code>$MAE_VALUE</code></li>
<li><strong>R&sup2; Score:</strong> <code>$R2_SCORE</code></li>
</ul>
<h3>Feature Importance</h3>
<p>The most important features for predicting housing prices are:</p>
<ol>
<li><code>median_income</code></li>
<li><code>rooms_per_household</code></li>
<li><code>population_per_household</code></li>
</ol>
<h2 id="results">Results</h2>
<ul>
<li>The model achieved an <strong>R&sup2; Score</strong> of <code>0.83</code>, indicating a good fit to the data.</li>
<li>The <strong>Mean Absolute Error (MAE)</strong> was <code>30528.50</code>, which means the model's predictions are, on average, within <code>$MAE_VALUE</code> dollars of the actual prices.</li>
</ul>
<h2 id="contributing">Contributing</h2>
<p>Contributions are welcome! If you'd like to contribute, please follow these steps:</p>
<ol>
<li>Fork the repository.</li>
<li>Create a new branch (<code>git checkout -b feature/YourFeatureName</code>).</li>
<li>Commit your changes (<code>git commit -m 'Add some feature'</code>).</li>
<li>Push to the branch (<code>git push origin feature/YourFeatureName</code>).</li>
<li>Open a pull request.</li>
</ol>
<p>&nbsp;</p>
