# AI Compliance Demonstration: GDPR Right to Explanation

**Name:** Denniz Garza
**Topic/Regulation Chosen:** GDPR "Right to Explanation" & PII Protection (HIPAA-style)

---

## Summary of the Principle/Regulation

This demonstration addresses the GDPR "Right to Explanation," which requires organizations to provide meaningful explanations for automated decisions affecting individuals. In a medical AI context, patients have a right to understand why a model predicts their health risk. Additionally, HIPAA requires the protection of sensitive patient information (PII), illustrating the need for careful data handling and anonymization.

---

## Technical Explanation of the Code Demonstration

1. A synthetic medical dataset is generated, including a sensitive feature `sex`.  
2. A Random Forest Classifier predicts the target variable (simulated disease outcome).  
3. **Feature Importance** is calculated using permutation importance to explain model predictions, including the sensitive feature.  
4. The sensitive feature is removed, the model is retrained, and predictions are compared to demonstrate anonymization impact.

---

## Real-World Consequence

- If healthcare AI systems fail to explain predictions, they violate GDPR Art. 22, which can result in fines up to 4% of global revenue.  
- Failure to protect PII (e.g., `sex`) risks HIPAA violations, which may lead to penalties up to $50,000 per record.  
- This demonstration shows both the **explainability** and **PII mitigation** trade-offs in AI deployment.

---

## Mitigation & Best Practices

- Remove or anonymize personal identifiers before training.
- Implement fairness-aware learning algorithms.
- Use SHAP, LIME, or interpretML to document and explain feature influence.
- Maintain model cards or compliance documentation for audit readiness.

---

## Youtube Link
https://youtu.be/tLZFjIXgj9U
