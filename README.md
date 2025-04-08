# Computational Replication of Essential Gene Identification Methods in Targeted Genome Sequencing  
**Niccolò Caselli**  
**30/12/2024**

**University of Florence – School of Engineering**  
**Bachelor’s Degree in Computer Engineering**  

**Project submitted for the final exam of the Artificial Intelligence course – B003725**  

**Professor:**  
Prof. Paolo Frasconi  

**Department:**  
Department of Information Engineering  

---
This project is a computational study aimed at replicating the findings of the research paper "Towards the Identification of Essential Genes Using Targeted Genome Sequencing and Comparative Analysis" by Gustafson et al. (2006). It focuses on evaluating machine learning classifiers for predicting essential genes in _S. cerevisiae_ and _E. coli_, validating the performance and methodology presented in the original work.

## Objective

The primary goal was to assess the accuracy of Naive Bayes and Random Forest classifiers in predicting gene essentiality, based on provided datasets and computational methods. The study emphasizes replicability and compares the results to those presented in the original research.

## Methodology

- **Tools and Libraries**: Python's `scikit-learn` was used for machine learning, alongside `pandas`, `numpy`, and `matplotlib` for data handling and visualization.
- **Dataset**: Gene-specific features and binary labels indicating essentiality were sourced from the supplementary materials of the original paper.
- **Feature Selection**: Features were divided into predefined groups (e.g., SC_GenProt and SC_All) with rankings derived from mutual information maximization (CMIM).
- **Implementation**:
  - **Naive Bayes**: Replicated the original methodology with bootstrapping for model evaluation.
  - **Random Forest**: A comparative classifier using K-fold cross-validation and tailored hyperparameters.
- **Evaluation Metrics**: Positive Predictive Value (PPV) and Area Under the Receiver Operating Characteristic Curve (AUC) were used to assess performance.

## Results

- Naive Bayes closely replicated the original results with slight improvements in some metrics.
- Random Forest demonstrated superior performance but required additional features and optimization.
- Phyletic retention emerged as the most predictive feature, aligning with the findings of Gustafson et al.

## Conclusion

The replication validated the original study's results, demonstrating that computational methods can significantly reduce the experimental workload in essential gene identification. Future improvements could include better hyperparameter optimization and addressing class imbalance through resampling techniques.

## Additional Information

All source code, plots, and results are available on GitHub: [report.pdf](https://github.com/NiccoloCase/essential-genes-identification/blob/main/report.pdf)
