# AUC-decomposition---Taiwan-dataset
In credit risk modeling, metrics such as AUC and Gini are widely used, yet several misconceptions persist—for example, how they are influenced by the false positive rate. But what do these measures actually capture, and how can they be applied more effectively in model validation?

A study by Agus Sudjianto and Alice L. introduced the idea of breaking down AUC into within-cluster and between-cluster components to improve validation practices. Building on their framework, I extended this concept to the Gini index (also known as Accuracy Ratio or Somers’ D).

Instead of relying solely on a single overall score, decomposing AUC/Gini provides insights into where a model consistently struggles or creates imbalances across groups. This perspective supports better monitoring, calibration, and fairness assessments.

The code you will find is inspired from this work: https://github.com/asudjianto-xml/AUC-Decomposition and the paper cited below.

The paper: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5386496

