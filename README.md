# AUC-decomposition---Taiwan-dataset
In credit risk modeling, metrics such as AUC and Gini are widely used, yet several misconceptions persist—for example, how they are influenced by the false positive rate. But what do these measures actually capture, and how can they be applied more effectively in model validation?

A study by Agus Sudjianto and Alice L. introduced the idea of breaking down AUC into within-cluster and between-cluster components to improve validation practices. Building on their framework, I extended this concept to the Gini index (also known as Accuracy Ratio or Somers’ D).

Instead of relying solely on a single overall score, decomposing AUC/Gini provides insights into where a model consistently struggles or creates imbalances across groups. This perspective supports better monitoring, calibration, and fairness assessments.

The code you will find is inspired by this work: https://github.com/asudjianto-xml/AUC-Decomposition and the paper cited below.

The paper: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5386496

ABSTRACT: 
The Area Under the ROC Curve (AUC) is a widely used performance metric for binary classifiers. However, as a global ranking statistic, the AUC aggregates model behavior over the entire dataset, masking localized weaknesses in specific subpopulations. In high-stakes applications such as credit approval and fraud detection, these weaknesses can lead to financial risk or operational failures. In this paper, we introduce a formal decomposition of global AUC into intra- and inter-cluster components. This allows practitioners to evaluate classifier performance within and across clusters of data, enabling granular diagnostics and subgroup analysis. We also compare the AUC with additive performance metrics such as the Brier score and log loss, which support decomposability and direct attribution. Our framework enhances model development and validation practice by providing additional insights to detect model weakness for model risk management.
