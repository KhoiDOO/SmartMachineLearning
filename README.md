# SmartLog

Structure of history

- train_case_0:
  - param_dict
  - fold_data
    - fold_0:
    - confusion_matrix:
      - TP : int
      - FP : int
      - TN : int
      - FN : int
    - overall_analysis:
      - accuracy : float64
      - balanced_accuracy : float64
      - sensitivity : float64
      - specificity : float64
      - precision : float64
      - f1-score : float64
    - deep_analysis
      - negative_predictive_value : float64
      - false_negative_rate : float64
      - false_positive_rate : float64
      - false_discovery_rate : float64
      - false_omission_rate : float64
      - positive_likelihood_ratio : float64
      - negative_likelihood_ratio : float64
      - prevalence_threshold : float64
      - threat_score : float64
      - prevalence : float64
      - matthews_correlation_coefficient : float64
      - fowlkes_mallows_index : float64
      - informedness : float64
      - markedness : float64
      - diagnostic_odds_ratio : float64
    - ROC_CURVE : dict
      - tpr: dict
        - class1 : [tpr_values]
        - class2 : [tpr_values]
      - fpr: dict
      - thresh_holds : dict
      - fpr_micro_avg : numpy array
      - tpr_micro_avg : numpy array
      - fpr_macro_avg : numpy array
      - tpr_macro_avg : numpy array
    - AUC_SCORE
      - roc_auc_macro : float64
      - roc_auc_micro : float64
      - roc_auc_weighted : float64
    - Classification_Report
  - fold_1
  - fold_n
- train_case_1
- train_case_n
