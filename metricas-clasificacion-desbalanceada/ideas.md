Esto viene de

# The Precision-Recall Plot Is More Informative than the ROC Plot When Evaluating Binary Classifiers on Imbalanced Datasets](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0118432


and performance is frequently illustrated with Receiver Operating Characteristics (ROC) plots

any bioinformatics studies develop and evaluate classifiers that are to be applied to strongly imbalanced datasets in which the number of negatives outweighs the number of positives significantly. While ROC plots are visually appealing and provide an overview of a classifier's performance across a wide range of specificities, one can ask whether ROC plots could be misleading when applied in imbalanced classification scenarios

"Max idea : so ROC plots works good for many eccesanrios"

 We show here that the visual interpretability of ROC plots in the context of imbalanced datasets can be deceptive with respect to conclusions about the reliability of classification performance, owing to an intuitive but wrong interpretation of specificity. PRC plots, on the other hand, can provide the viewer with an accurate prediction of future classification performance due to the fact that they evaluate the fraction of true positives among positive predictions.

 "Max idea: deceptive means give the incorrect idea, prc could give a better interpretation because it evaluate the fection of true positives among positive predictions"


 "Max idea : es importante añadir esto " - > "In binary classification, data is divided into two different classes, positives (P) and negatives (N) (see Fig. 1A, left oval). The binary classifier then classifies all data instances as either positive or negative (see Fig. 1A, right oval). This classification produces four types of outcome—two types of correct (or true) classification, true positives (TP) and true negatives (TN), and two types of incorrect (or false) classification, false positives (FP) and false negatives (FN) (see Fig. 1B). A 2x2 table formulated with these four outcomes is called a confusion matrix. All the basic evaluation measures of binary classification are derived from the confusion matrix (see Table 1).


"



Esto igual esta bueno -> "While any such threshold, which divides a dataset into positively and negatively predicted classes, can be reasonable in a particular application, it is not obvious how the right threshold value should be chosen. A powerful solution is to use threshold-free measures such as the ROC and PRC plots." menciona que es mejor usar metodos de evaluacion que no dependan del treshold o treshold free


otra explicacion de curva roc -. "The ROC plot shows the tradeoff between specificity and sensitivity [24]. It is model-wide because it shows pairs of specificity and sensitivity values calculated at all possible threshold scores. In ROC plots, classifiers with random performance show a straight diagonal line from (0, 0) to (1, 1) [24], and this line can be defined as the baseline of ROC. A ROC curve provides a single performance measure called the Area under the ROC curve (AUC) score. AUC is 0.5 for random and 1.0 for perfect classifiers [4]. AUC scores are convenient to compare the performances of multiple classifiers."


es verdad que mide specifity y sencivity que son eso



esto esta excelente para explicar "Un ejemplo concreto: imaginá un dataset de detección de fraude con 100 fraudes y 99,900 transacciones legítimas. Si el modelo genera 500 falsos positivos, eso es catastrófico en la práctica (por cada fraude detectado hay 5 alertas falsas), pero el FPR es solo 500/99,900 ≈ 0.5%. La curva ROC ve eso como un rendimiento excelente."


En resumen: la ROC es "optimista" con datos desbalanceados porque el FPR se atenúa con la cantidad de negativos. La curva PR es más honesta porque mide directamente la calidad de las predicciones positivas sin que la clase mayoritaria distorsione la métrica.