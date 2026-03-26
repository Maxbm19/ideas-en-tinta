# Referencias: Métricas para Clasificación Desbalanceada

## Artículos y papers académicos

- [The Precision-Recall Plot Is More Informative than the ROC Plot When Evaluating Binary Classifiers on Imbalanced Datasets](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0118432) — Saito & Rehmsmeier (2015), PLOS ONE. Paper fundacional que demuestra por qué PR-AUC supera a ROC-AUC en datos desbalanceados.
- [The Precision-Recall Plot — PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC4349800/) — Texto completo en PubMed Central.
- [ROC curve accurately assesses imbalanced datasets](https://www.sciencedirect.com/science/article/pii/S2666389924001090) — ScienceDirect (2024), perspectiva contraria sobre ROC.

## Documentación oficial scikit-learn

- [roc_auc_score](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.roc_auc_score.html) — API reference.
- [precision_recall_curve](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_recall_curve.html) — API reference.
- [average_precision_score](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.average_precision_score.html) — AP score (área bajo curva PR).
- [auc](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.auc.html) — Función genérica para calcular AUC.
- [Precision-Recall example plots](https://scikit-learn.org/stable/auto_examples/model_selection/plot_precision_recall.html) — Ejemplo oficial con visualizaciones.

## Blogs y guías técnicas

- [ROC vs PRC](https://beverly-wang0005.medium.com/roc-vs-prc-6cd30d287a4b) — Beverly Wang, Medium: explicación accesible de por qué ROC no es apropiada para datos muy desbalanceados y cuándo combinar PRC con F1 y Cohen's Kappa.
- [ROC AUC vs Precision-Recall for Imbalanced Data](https://machinelearningmastery.com/roc-auc-vs-precision-recall-for-imbalanced-data/) — MachineLearningMastery: comparación práctica con código.
- [How and Why I Switched from ROC to PR Curve](https://juandelacalle.medium.com/how-and-why-i-switched-from-the-roc-curve-to-the-precision-recall-curve-to-analyze-my-imbalanced-6171da91c6b8) — Medium: experiencia práctica en producción.
- [Precision-Recall Curve, a Different View](https://sinyi-chou.github.io/classification-pr-curve/) — Sin Yi Chou: visualizaciones detalladas.
- [The Complete Guide to AUC and Average Precision](https://glassboxmedicine.com/2020/07/14/the-complete-guide-to-auc-and-average-precision-simulations-and-visualizations/) — Glass Box Medicine: simulaciones y visualizaciones.
- [What Is PR AUC?](https://arize.com/blog/what-is-pr-auc/) — Arize AI: explicación orientada a MLOps.

## F1 Score

- [How can the F1-score help with class imbalance?](https://sebastianraschka.com/faq/docs/computing-the-f1-score.html) — Sebastian Raschka, PhD.
- [The Ultimate F1 Score Guide for Imbalanced Classes](https://www.numberanalytics.com/blog/f1-score-imbalanced-classes-guide) — Number Analytics.
- [F1 Score in Machine Learning Explained](https://encord.com/blog/f1-score-in-machine-learning/) — Encord Blog.

## Google ML Crash Course

- [Classification: ROC and AUC](https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc) — Google Developers.

## Dataset de ejemplo

- [Credit Card Fraud Detection — Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) — 284,807 transacciones, 492 fraudes (0.172%). Dataset estándar para benchmarking de métricas en desbalanceo extremo.
- [Credit Fraud: Dealing with Imbalanced Datasets](https://www.kaggle.com/code/janiobachmann/credit-fraud-dealing-with-imbalanced-datasets) — Notebook de referencia en Kaggle.
- [Imbalanced Classification with the Credit Card Fraud Dataset](https://machinelearningmastery.com/imbalanced-classification-with-the-fraudulent-credit-card-transactions-dataset/) — MachineLearningMastery: tutorial completo.
