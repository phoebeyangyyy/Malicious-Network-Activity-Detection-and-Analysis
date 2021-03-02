# Malicious Network Activity Detection and Analysis

**Summary:**

In this project, I developed an Intrusion Detection System(IDS) to identify normal interactions and various types of attacks. Conduct exploratory data analysis like turn the target variable to feature with binary values by encoding the 22 kinds of attacks into one group called "abnormal" and removed highly correlated features and missing values, etc.

Futhermore, I built a Random Forest model and fine-tune the model parameters through the grid search to find optimal hyperparameter. Several metrics have been designed to measure the effectiveness of IDS. I choose the ranking metrics to include confusion matrix, and Area under the ROC curve (AUC). Those are good metrics that represent the ability of the system to distinguish between intrusive and non-intrusive activities. The evaluation results are too good to be true. A overfitting problem occures because of the imbalanced dataset.

Last but not least, I analyzied top factors that give rise to malicious attacks to gain access or cause destruction to the network."dst_bytes" is the top1 factor to monitor a network or systems for malicious activity or policy violations.

**Drawbacks:**

It is not enough to deal with the imbalanced data just using cross-validation. I can use the SMOTE method for addressing imbalanced datasets and oversample the minority class.
Not only measure the effectiveness, but the efficiency should also be considered as a metric to the given model for this measure deals with the resources needed to be allocated to the system including CPU cycles and main memory.
More models could be tried to achieve better accuracy when distinguishing between the various types of attacks and normal interactions.
