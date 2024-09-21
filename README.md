# SpaceX Falcon 9 First Stage Landing Prediction and Data Analysis

## Project Overview

This project aims to predict the success of Falcon 9 first stage rocket landings and analyze the key factors influencing landing outcomes. Using a combination of exploratory data analysis (EDA), SQL queries, interactive data visualization, and machine learning, we explore the historical launch data from SpaceX to derive insights and build predictive models.

### Key Objectives
1. **Exploratory Data Analysis**: Visualize and identify patterns in the data related to flight number, payload mass, orbit type, and launch success rate.
2. **SQL Queries**: Analyze the SpaceX dataset stored in a database using SQL queries to extract key insights.
3. **Data Collection and Web Scraping**: Gather data on launch outcomes, rocket types, and payloads using SpaceX’s API and web scraping techniques.
4. **Geospatial Analysis**: Use Folium to map SpaceX launch sites and analyze their proximities to key geographical features.
5. **Machine Learning**: Build a machine learning pipeline to predict the success of future landings using models like Logistic Regression, SVM, Decision Trees, and KNN.

### Tools & Libraries
- **Python**: Main programming language for data analysis, visualization, and modeling.
- **Pandas, NumPy**: Data manipulation and processing.
- **Matplotlib, Seaborn**: Data visualization for EDA.
- **Folium**: Geospatial analysis and visualization.
- **SQLAlchemy, SQLite**: SQL database interaction and query execution.
- **Scikit-learn**: Machine learning algorithms and evaluation.
- **Plotly Dash**: For creating interactive dashboards (future extension).

### Components of the Project
1. **Exploratory Data Analysis (EDA)**:
   - Performed initial analysis to understand how factors like flight number, payload mass, and orbit type impact landing success.
   - Visualized trends over time, including launch success rates per year.
   
2. **SQL Data Analysis**:
   - Loaded SpaceX data into a SQLite database.
   - Executed SQL queries to extract insights such as total payload mass, successful launches, and average payload per booster version.
   
3. **Web Scraping & Data Collection**:
   - Used SpaceX API to collect additional data on launches and rockets.
   - Scraped revenue and stock data for analysis and integration with launch data.

4. **Geospatial Analysis with Folium**:
   - Mapped the coordinates of SpaceX launch sites.
   - Visualized the success and failure outcomes of launches at each site.
   - Calculated distances between launch sites and key geographical features like coastlines and cities.

5. **Machine Learning**:
   - Built and tuned several models (Logistic Regression, SVM, Decision Trees, KNN) to predict the success of Falcon 9 first stage landings.
   - Achieved high test accuracy using hyperparameter tuning with GridSearchCV.

### Results & Insights
- **Best Machine Learning Model**: Logistic Regression and SVM performed equally well with a test accuracy of 83.3%.
- **Key Factors for Success**: Flight number, payload mass, and orbit type significantly influence landing outcomes.
- **Geospatial Insights**: Launch sites close to coastlines have better success rates, potentially due to lower risk in controlled landings.
  
### Future Work
- **Dashboard Development**: Build an interactive dashboard using Plotly Dash to monitor and visualize SpaceX launches.
- **Model Improvement**: Explore additional machine learning models like Gradient Boosting or XGBoost to improve prediction accuracy.
- **Real-time Data Integration**: Incorporate real-time data from SpaceX API for continuous model updates and insights.

### How to Run
1. Clone the repository and install the required dependencies using `pip install -r requirements.txt`.
2. Run the Jupyter notebooks for each component:
   - `EDA.ipynb`: Perform exploratory data analysis.
   - `SQL_Analysis.ipynb`: Analyze data using SQL queries.
   - `Machine_Learning_Prediction.ipynb`: Build and evaluate machine learning models.
   - `Geospatial_Analysis.ipynb`: Visualize launch sites and proximity analysis with Folium.
3. Optionally, extend the project by creating interactive dashboards using Plotly Dash.

### Data Sources
- [SpaceX API](https://api.spacexdata.com/): For rocket and launch data.
- [Public SpaceX Datasets](https://www.kaggle.com/spacex/spacex-launch-data): For historical launch records.
