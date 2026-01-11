# Otto Group Product Classification Challenge

This project addresses the **Otto Group Product Classification Challenge**, a multiclass classification problem involving anonymized tabular data. The objective is to predict product categories while minimizing **multiclass logarithmic loss**, with an emphasis on probabilistic calibration.

## Project Overview
- **Dataset:** Over 200,000 products described by 93 numerical features  
- **Task:** Supervised multiclass classification (9 classes)  
- **Evaluation Metric:** Multiclass log-loss  
- **Platform:** Kaggle  

## Methodology
A variety of machine learning models were explored, including logistic regression, k-nearest neighbors, random forests, neural networks, and gradient-boosted trees (XGBoost). To leverage the complementary strengths of these models, an **advanced stacking ensemble** was implemented using out-of-fold predictions and a tree-based meta-model.
![Model Pipeline](Final_pipeline.png)

## Results
The final stacking ensemble outperformed all individual base models in terms of log-loss and accuracy. The approach achieved a **Kaggle leaderboard score of 0.42174**, ranking **201 out of 3,559 participants**.

## Limitations
The primary limitation of this project is computational cost. Training the full ensemble requires significant time, which constrained rapid experimentation and occasionally led to session interruptions in the Kaggle environment.

## Key Takeaways
This project provided hands-on experience with ensemble learning, probabilistic modeling, validation strategies, and large-scale tabular data modeling in a competitive setting.

