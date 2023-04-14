# Appendix 
Summarizes concepts from the notebook.

---

## **Group Measures**

| Count Type | Column Name |
| --- | --- |
| False Positive Count | 'fp' |
| False Negative Count | 'fn' |
| True Negative Count | 'tn' |
| True Positive Count | 'tp' |
| Predicted Positive Count | 'pp' |
| Predicted Negative Count | 'pn' |
| Count of Negative Labels in Group | 'group_label_neg' |
| Count of Positive Labels in Group | 'group_label_pos' | 
| Group Size | 'group_size'|
| Total Entities | 'total_entities' |

---

## **Absolute Metrics**

| Metric | Column Name |
| --- | --- |
| True Positive Rate | 'tpr' |
| True Negative Rate | 'tnr' |
| False Omission Rate | 'for' |
| False Discovery Rate | 'fdr' |
| False Positive Rate | 'fpr' |
| False Negative Rate | 'fnr' |
| Negative Predictive Value | 'npv' |
| Precision | 'precision' |
| Predicted Positive Ratio$_k$ | 'ppr' |
| Predicted Positive Ratio$_g$ | 'pprev' |
| Group Prevalence | 'prev' |

### **False Negative Rate**

The fraction of false negatives of a group within the labeled positives of the group:

$$FNR_g = \frac{FN_g}{LP_g} = Pr(\hat{Y}=0—Y=1,A=a_i)$$

### **Equality of Opportunity** (i.e. True Positive rate Parity)

The protected and unprotected groups should have equal true positive rates (i.e. same rate of positive outcome, assuming the people in the groups qualify for the outcome):

$$TPR_g = \frac{TP_g}{LP_g} = Pr(\hat{Y}=1—Y=1,A=a_i)$$

---

## **Disparities**

| Metric | Column Name |
| --- | --- |
| True Positive Rate Disparity | 'tpr_disaprity' |
| True Negative Rate Disparity | 'tnr_disparity' |
| False Omission Rate Disparity | 'for_disparity' |
| False Discovery Rate Disparity | 'fdr_disparity' |
| False Positive Rate Disparity | 'fpr_disparity' |
| False NegativeRat Disparitye | 'fnr_disparity' |
| Negative Predictive Value Disparity | 'npv_disparity' |
| Precision Disparity | 'precision_disparity' |
| Predicted Positive Ratio$_k$ Disparity | 'ppr_disparity' |
| Predicted Positive Ratio$_g$ Disparity | 'pprev_disparity' |

---

## **Parities**

| Parity | Column Name |
| --- | --- |
| True Positive Rate Parity | ‘TPR Parity’ |
| True Negative Rate Parity | ‘TNR Parity’ |
| False Omission Rate Parity | ‘FOR Parity’ | 
| False Discovery Rate Parity | ‘FDR Parity’ |
| False Positive Rate Parity | ‘FPR Parity’ |
| False Negative Rate Parity | ‘FNR Parity’ |
| Negative Predictive Value Parity | ‘NPV Parity’ |
| Precision Parity | ‘Precision Parity’ |
| Predicted Positive Ratio_k Parity | ‘Statistical Parity’ |
| Predicted Positive Ratio_g Parity | ‘Impact Parity’ |

| Column Name | Description |
| --- | --- |
| Type I Parity | Fairness in both FDR Parity and FPR Parity |
| Type II Parity | Fairness in both FOR Parity and FNR Parity |
| Equalized Odds | Fairness in both FPR Parity and TPR Parity |
| Unsupervised Fairness | Fairness in both Statistical Parity and Impact Parity|
| Supervised Fairness | Fairness in both Type I and Type II Parity |
| Overall Fairness | Fairness across all parities for all attributes |

---

## **Disparity Tolerance**

$$ \tau ≤ DisparityMeasure_{group_i} ≤ \frac{1}{\tau} $$

$$ 0.8 ≤ DisparityMeasure_{group_i} ≤ \frac{1}{0.8} = 1.25 $$
