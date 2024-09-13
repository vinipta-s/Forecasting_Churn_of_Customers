**Prompt**: The telecom operator Interconnect would like to be able to forecast their churn of clients. If it's discovered that a user is planning to leave, they will be offered promotional codes and special plan options. Interconnect's marketing team has collected some of their client's personal data, including information about their plans and contracts.

**This project's focus was on building a machine learning model that can forecast client churn with a AUC-ROC score above 0.85 and achieved 0.9 AUC-ROC and 0.8+ accuracy on the testset with CatBoostClassifier.**

**Project structure:**
1. Libraries
2. Load Data
3. Clean Data
   * Merge data sets
   * Replace Nulls
   * Feature engineering: 'tenure', 'year_start', 'churn'
4. Data Visualization: How the features impact churn.
5. Final Data preparation
  1. Feature engineering: base_charges
  2. Label encoding categorical features
  3. data spliting
  4. Normalize charges by scaling
  5. upsample data
7. Models:
   * LogisticRegression
   * RandomForestClassifier 
   * CatBoostClassifier
   * KNeighborsClassifier
   * VotingClassifier
9. CatBoostClassifier had the highest evaluation scores with a 0.9 AUC-ROC and 0.8+ accuracy on the testset. 


**Datasets**:
  contract.csv — contract information
  personal.csv — the client's personal data
  internet.csv — information about Internet services
  phone.csv — information about telephone services
