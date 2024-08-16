![NBA Data Analysis](https://github.com/MadanThevar/NBA-Analysis-Project/blob/main/bull1-ezgif.com-webp-to-gif-converter.gif?raw=true)

# 🏀 NBA Statistics Analysis Project

## 📄 Overview
This project explores the application of **machine learning** and **data visualization** techniques to analyze NBA player statistics. Our analysis aims to predict player performance, provide insights into team strategies, and enhance decision-making processes within the NBA.

## 📊 Dataset Information
- **Source**: Data was scraped from [Basketball Reference](https://www.basketball-reference.com/leagues/NBA_2024_totals.html), including statistics on points per game, rebounds, field goals, and more for the 2024 NBA season.
- **Data Cleaning**: The data was meticulously cleaned to ensure accuracy, focusing on player performance metrics and team outcomes.

## 🔍 Methodology
1. **Data Collection and Cleaning**:
   - Collected extensive data covering all NBA players and teams.
   - Organized data into structured data frames, filtering outliers to refine the dataset.
   
2. **Exploratory Data Analysis (EDA)**:
   - **Correlation Heatmap**: Visualized relationships between various player statistics using Seaborn and Matplotlib.
   - **Elbow Graph**: Determined optimal player archetypes, such as scorers and defenders, for clustering analysis.
   
3. **Machine Learning Models**:
   - **📈 Linear Regression**: Predicted points scored based on field goal attempts, achieving a significant R-squared value of 0.460.
   - **🌲 Random Forest Classifier**: Classified player positions with an accuracy of 42.86%, based on game data and player metrics.
   - **🎯 K-Means Clustering**: Grouped players into archetypes using key features like points and assists, providing insights into player roles.
   - **🌳 Decision Tree Classifier**: The Decision Tree model effectively classifies NBA player positions using key metrics such as assists (AST), rebounds (TRB), field goal attempts (FGA), and field goal percentage (FG%), providing an interpretable method to understand how these performance indicators determine player roles.
   - **📊 SVM Model**: A Support Vector Machine (SVM) model was also trained to classify player positions, leveraging its strength in handling high-dimensional spaces and providing a robust classification boundary.

## 📈 Graphs and Visualizations

### 🔥 Correlation Heatmap
![image](https://github.com/user-attachments/assets/7efe1d75-484b-4e19-8f5b-35b7cb4f488c)
- **Description**: This heatmap visualizes the correlations between different player statistics. For example, it shows a strong positive correlation between `Field Goal Attempts (FGA)` and `Points Scored (PTS)`, suggesting that players who attempt more shots tend to score more points.

### 📊 Elbow Graph
![image](https://github.com/user-attachments/assets/b625f0c6-dc7d-4f93-a0d3-84bf8d5b65ad)
- **Description**: The elbow graph helps determine the optimal number of clusters for player archetypes. The point where the graph bends (the "elbow") indicates the optimal number of clusters, which we used to group players into categories such as scorers, playmakers, and defenders.

### 📈 Linear Regression Model - Scatter Plot
![image](https://github.com/user-attachments/assets/a965f9db-7112-476a-b960-01d6c169f988)
- **Description**:  The model's performance shows a reasonable alignment with this line, indicating that it can moderately predict points scored based on input features like Field Goal Attempts (FGA).

### 🔍 SVM Model - Classification Boundary
![image](https://github.com/user-attachments/assets/2d6546a1-4505-47be-8b16-863b922340ba)
- **Description**: This graph shows the relationship between the actual points scored by NBA players and the points predicted by the Support Vector Regression (SVR) model. The red dashed line represents the ideal scenario where the predicted points would exactly match the actual points.

### 🎯 K-Means Clustering - Player Archetypes
![image](https://github.com/user-attachments/assets/151b1ffb-af53-450e-aa1b-c7007b17adeb)
- **Description**: This scatter plot illustrates the results of the K-Means clustering model, grouping players based on their performance stats. Each color represents a different player archetype, providing insights into their roles on the court.

### 🌳 Decision Tree Classifier - Visualization
![image](https://github.com/user-attachments/assets/14358651-d951-4ac0-af2e-79ddd584ac64)
- **Description**: This Decision Tree model is used to classify NBA player positions based on various performance metrics, such as assists, rebounds, field goal attempts, and more. Each node in the tree represents a decision based on one of these metrics, leading to a prediction of the player's position at the leaf nodes.

## 🌟 Key Insights
- **Accurate Predictions**: Linear regression and OLS models provided significant predictive potential for scoring metrics.
- **Player Archetypes**: Clustering analysis revealed distinct player roles, aiding in player evaluation and team composition.
- **OLS Statistics Summary**
<img width="690" alt="Screenshot 2024-08-15 at 20 32 29" src="https://github.com/user-attachments/assets/bb9dba94-db2a-4f0b-9ab9-6af7936fa573">

- The OLS regression shows that each additional field goal attempt increases points scored by approximately 1.08, with an R-squared of 0.46, indicating a moderately strong model.

## 🔑 Key Takeaways
1. **Linear Regression Performance**: The Linear Regression model is effective for capturing the linear relationship between field goal attempts and points scored, making it a suitable choice for basic predictions.
2. **Complexity vs. Performance**: More complex models like SVR and Decision Trees may introduce unnecessary complexity for this dataset, as simpler models like Linear Regression perform comparably well.
3. **Clustering Insights**: K-Means clustering effectively grouped players into archetypes, providing valuable insights into player roles and team composition.
4. **Model Interpretability**: Simpler models like Linear Regression and Decision Trees offer better interpretability, which is essential for understanding and explaining predictions.
5. **Data Quality**: The accuracy of all models heavily depends on the quality and completeness of the dataset. Proper data cleaning and preprocessing are crucial for reliable predictions.

## 🚀 Room for Improvements
1. **Feature Engineering**: Introducing additional features such as advanced shooting metrics, defensive stats, or player efficiency ratings to enhance model predictions.
2. **Model Tuning**: Fine-tuning hyperparameters for complex models like SVR and Decision Trees to improve their performance and reduce overfitting.
3. **Ensemble Methods**: Using ensemble methods like Random Forests or Gradient Boosting to combine the strengths of multiple models and achieve better predictive accuracy.
4. **Cross-Validation**: Implementing cross-validation techniques to better assess model performance and generalize predictions to new data.
5. **Handling Non-Linearity**: Exploring non-linear models or polynomial regression to better capture potential non-linear relationships in the data.

## 📈 Applications
- **Player Evaluation**: By applying machine learning models such as Decision Trees, SVMs, and Linear Regression, teams can accurately evaluate player performance and potential, enabling data-driven decisions in scouting and roster management.
- **Team Strategy**: Leveraging clustering methods like K-Means allows teams to identify player archetypes, which can be crucial for tailoring game strategies and optimizing team composition. 
- **Model Optimization**: To further improve model accuracy and robustness, techniques like hyperparameter tuning, feature selection, and ensemble methods (e.g., Random Forest) could be employed.
- **Advanced Analytics**: Incorporating additional player metrics, such as advanced shooting metrics or defensive statistics, could provide a more holistic view of player performance and improve model predictions.
- **Fan Engagement**: Enhanced understanding of player roles and team dynamics can boost fan engagement and interest, with data-driven insights being used to create interactive fan experiences and media content.

## 📂 Project Structure
- **/data**: Contains the raw and cleaned datasets used in the analysis.
- **/notebooks**: Jupyter notebooks showcasing the data analysis process and model implementation.
- **/scripts**: Python scripts used for data processing and model training.

## 🙌 Contributors
- **Sydney Truong**
- **Austin Percy**
- **Madan Thevar**
