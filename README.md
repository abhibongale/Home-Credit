# Home Credit: Credit Risk Model Stability
The goal of this repository is to predict which clients are more likely to default on their loans

## Description
 The absence of a credit history might mean a lot of things, including young age or a preference for cash. 
 Without traditional data, someone with little to no credit history is likely to be denied. Consumer finance providers must accurately determine which clients can repay a loan and which cannot and data is key. If data science could help better predict one’s repayment capabilities, loans might become more accessible to those who may benefit from them the most.

Currently, consumer finance providers use various statistical and machine learning methods to predict loan risk. These models are generally called scorecards. In the real world, clients' behaviors change constantly, so every scorecard must be updated regularly, which takes time. The scorecard's stability in the future is critical, as a sudden drop in performance means that loans will be issued to worse clients on average. The core of the issue is that loan providers aren't able to spot potential problems any sooner than the first due dates of those loans are observable. Given the time it takes to redevelop, validate, and implement the scorecard, stability is highly desirable. There is a trade-off between the stability of the model and its performance, and a balance must be reached before deployment.
Founded in 1997, competition host Home Credit is an international consumer finance provider focusing on responsible lending primarily to people with little or no credit history. Home Credit broadens financial inclusion for the unbanked population by creating a positive and safe borrowing experience.


## Evaluation
www.kaggle.com/competitions/home-credit-credit-risk-model-stability/overview/evaluation

## Scoring
1. Innovation (40%): Analyzes credit stability over time, specifically focusing on the competition evaluation metric beyond just feature selection. e.g. High average gini, non-decreasing performance over time, small oscillations
2. Quality (20%): Any tables, figures, and/or code samples are high quality (e.g. information-dense, easy-to-understand, and informative)
3. Clarity (20%): The overall composition is articulate, concise, accurate, and easy-to-understand.
4. Generalization (20%): The implementation of stability as a metric can be applied to non-competition datasets.
