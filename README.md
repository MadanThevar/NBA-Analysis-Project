![NBA Data Analysis](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.pinterest.com%2Fpin%2Fnba-playoffs-basketball-gif-by-nba-find-share-on-giphy--587860557622407818%2F&psig=AOvVaw0T-DLXtxYCJyYNI3D_gQYM&ust=1723856421872000&source=images&cd=vfe&opi=89978449&ved=0CBMQjRxqFwoTCMDamOCn-IcDFQAAAAAdAAAAABAp)

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
   - **🌳Decision Tree Classifier**: The Decision Tree model effectively classifies NBA player positions using key metrics such as assists (AST), rebounds (TRB), field goal attempts (FGA), and field goal percentage (FG%), providing an interpretable method to understand how these performance indicators determine player roles.

## 📈 Graphs and Visualizations

### 🔥 Correlation Heatmap
![image](https://github.com/user-attachments/assets/7efe1d75-484b-4e19-8f5b-35b7cb4f488c)
- **Description**: This heatmap visualizes the correlations between different player statistics. For example, it shows a strong positive correlation between `Field Goal Attempts (FGA)` and `Points Scored (PTS)`, suggesting that players who attempt more shots tend to score more points.

### 📊 Elbow Graph
![image](https://github.com/user-attachments/assets/b625f0c6-dc7d-4f93-a0d3-84bf8d5b65ad)
- **Description**: The elbow graph helps determine the optimal number of clusters for player archetypes. The point where the graph bends (the "elbow") indicates the optimal number of clusters, which we used to group players into categories such as scorers, playmakers, and defenders.

### 🎯 K-Means Clustering - Player Archetypes
![image](https://github.com/user-attachments/assets/151b1ffb-af53-450e-aa1b-c7007b17adeb)
- **Description**: This scatter plot illustrates the results of the K-Means clustering model, grouping players based on their performance stats. Each color represents a different player archetype, providing insights into their roles on the court.

🌳 **Decision Tree Classifier - Visualization**
![image](https://github.com/user-attachments/assets/14358651-d951-4ac0-af2e-79ddd584ac64)
- **Description**: This Decision Tree model is used to classify NBA player positions based on various performance metrics, such as assists, rebounds, field goal attempts, and more. Each node in the tree represents a decision based on one of these metrics, leading to a prediction of the player's position at the leaf nodes.

## 🌟 Key Insights
- **Accurate Predictions**: Linear regression and OLS models provided significant predictive potential for scoring metrics.
- **Player Archetypes**: Clustering analysis revealed distinct player roles, aiding in player evaluation and team composition.
- **OLS Statistics Summary**
<img width="690" alt="Screenshot 2024-08-15 at 20 32 29" src="https://github.com/user-attachments/assets/bb9dba94-db2a-4f0b-9ab9-6af7936fa573">

- The OLS regression shows that each additional field goal attempt increases points scored by approximately 1.08, with an R-squared of 0.46, indicating a moderately strong model.

## 🚀 Applications
- **Player Evaluation**: Use of machine learning models to evaluate player performance and potential.
- **Team Strategy**: Insights from the data can inform team strategies and decision-making.
- **Fan Engagement**: Enhanced understanding of player roles and team dynamics can boost fan engagement and interest.

## 📂 Project Structure
- **/data**: Contains the raw and cleaned datasets used in the analysis.
- **/notebooks**: Jupyter notebooks showcasing the data analysis process and model implementation.
- **/scripts**: Python scripts used for data processing and model training.
- **/outputs**: Final visualizations and analysis reports.
- **/images**: Contains the images of the graphs used in the markdown file.

## 📚 References
- **Final Report**: [Download PDF](./Final%20report%20document.pdf)
- **Working Project HTML**: [View Project](./Final%20working%20project%204%2030%20(1).html)
- **Group Presentation**: [Download PDF](./Group%2020.pdf)

## 🙌 Contributors
- **Sydney Truong**
- **Austin Percy**
- **Madan Thevar**
