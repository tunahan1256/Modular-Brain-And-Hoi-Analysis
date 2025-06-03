# From Cross-Modularity to High-Order Interactions: An Information-Theoretic Analysis of the Brain’s Modular Skeleton

This project was built upon the guidance and article suggestions of Prof. Daniele Marinazzo and represents my own implementation and interpretation. It was undertaken out of a desire to understand how basic information-theoretic measures can be used to analyze brain connectivity. The project investigates the modular organization and high-order informational dependencies of the human brain using structural and functional connectivity data.

## 🧠 Project Overview

The goal of this project is to reproduce and extend the findings of Diez et al. (2015) on modular brain organization and explore high-order interactions (HOIs) across brain modules using advanced information-theoretic measures. 

We:
- Clustered structural (SC) and resting-state functional connectivity (rsFC) matrices into 20 modules via hierarchical agglomerative clustering.
- Rearranged connectivity matrices based on these modules, confirming strong structural-functional alignment.
- Extracted representative time series per module using PCA.
- Analyzed statistical properties (normality) of module time series.
- Computed entropies, mutual information, and other information measures.
- Explored high-order interactions via O-information and S-information using both Gaussian Copula (GC) and k-Nearest Neighbors (KNN) estimators.

## 📚 Based On

- **[Diez et al., 2015]**: *A novel brain partition highlights the modular skeleton shared by structure and function.*
- **[HOI Library]**: *High-Performance Estimation of Higher-Order Interactions* by Alexandre Reis et al.

## 🧪 Methods Used

- **Hierarchical clustering** and **cross-modularity optimization** to identify 20 brain modules.
- **Principal Component Analysis (PCA)** for module signal extraction.
- **Information-theoretic measures**:
  - Entropy, Mutual Information, Conditional Mutual Information
  - O-Information, S-Information
  - Total Correlation (TC), Dual Total Correlation (DTC), Shared Information (Sinfo)
- **Estimators**:
  - Gaussian-based analytical estimators
  - Non-parametric KNN and Gaussian Copula-based methods
- **Statistical Testing**:
  - Shapiro-Wilk, Henze-Zirkler tests for normality
  - Variability and dependency characterization


## 🎓 Internship Context

This internship was completed in the research group of **Prof. Daniele Marinazzo** at **Ghent University**. It focused on the analysis of brain connectivity data using tools from information theory. Key goals included:

- Investigating the modular structure of the brain
- Characterizing brain dynamics through entropy and mutual information
- Exploring synergy and redundancy using high-order interactions (HOIs)

This research experience offered valuable insights into the complexity of brain organization and strengthened both analytical and computational skills in a neuroscience context.

## 📖 References

## References

- Basser, P. J., Mattiello, J., & LeBihan, D. (1994). *MR diffusion tensor spectroscopy and imaging*. Biophysical Journal, 66(1), 259–267.  
  [https://doi.org/10.1016/S0006-3495(94)80775-1](https://doi.org/10.1016/S0006-3495(94)80775-1)

- Biswal, B., et al. (1995). *Functional connectivity in the motor cortex of resting human brain using echo-planar MRI*. Magnetic Resonance in Medicine, 34(4), 537–541.  
  [https://doi.org/10.1002/mrm.1910340409](https://doi.org/10.1002/mrm.1910340409)

- Diez, I. et al. (2015). *A novel brain partition highlights the modular skeleton shared by structure and function*. Scientific Reports, 5, 10532.  
  [https://doi.org/10.1038/srep10532](https://doi.org/10.1038/srep10532)

- Friston, K. J., et al. (2003). *Dynamic causal modelling*. NeuroImage, 19(4), 1273–1302.  
  [https://doi.org/10.1016/S1053-8119(03)00202-7](https://doi.org/10.1016/S1053-8119(03)00202-7)

- Honey, C. J. et al. (2009). *Predicting human resting-state functional connectivity from structural connectivity*. PNAS, 106(6), 2035–2040.  
  [https://doi.org/10.1073/pnas.0811168106](https://doi.org/10.1073/pnas.0811168106)

- Meunier, D. et al. (2009). *Hierarchical modularity in human brain functional networks*.  
  [https://doi.org/10.3389/neuro.11.037.2009](https://doi.org/10.3389/neuro.11.037.2009)

- Human Connectome Project Dataset (n.d.). BioCr HCatlas.  
  [https://www.nitrc.org/projects/biocr_hcatlas](https://www.nitrc.org/projects/biocr_hcatlas)

- Reis, A. et al. (2023). *HOI: A Python library for higher-order information theoretic analysis in neuroscience*.  
  [https://brainets.github.io/hoi/](https://brainets.github.io/hoi/)

- Roebroeck, A., Formisano, E., & Goebel, R. (2005). *Mapping directed influence over the brain using Granger causality and fMRI*. NeuroImage, 25(1), 230–242.  
  [https://doi.org/10.1016/j.neuroimage.2004.11.017](https://doi.org/10.1016/j.neuroimage.2004.11.017)

- Sørensen, T. (1948). *A method of establishing groups of equal amplitude in plant sociology based on similarity of species*.  

- Tononi, G., Sporns, O., & Edelman, G. M. (1994). *A measure for brain complexity: Relating functional segregation and integration*. PNAS, 91(11), 5033–5037.  
  [https://doi.org/10.1073/pnas.91.11.5033](https://doi.org/10.1073/pnas.91.11.5033)

- Van Essen, D. C. et al. (2012). *The Human Connectome Project: A data acquisition perspective*. NeuroImage, 62(4), 2222–2231.  
  [https://doi.org/10.1016/j.neuroimage.2012.02.018](https://doi.org/10.1016/j.neuroimage.2012.02.018)


## 🔍 Future Directions

Building on the current findings, future research could incorporate transfer entropy decomposition to capture the directionality and dynamic flow of information between brain modules, enabling a deeper understanding of temporal causality. Feature importance methods like mutual information ranking or recursive feature elimination could help identify key modules or interactions related to individual differences or clinical outcomes, improving model interpretability and prediction.

Adopting standardized parcellation schemes such as Yeo’s 7+2 networks would enhance cross-study comparisons and clarify whether high-order synergistic and redundant patterns are network-specific. Extending analyses to dynamic functional connectivity using sliding-window or hidden Markov models combined with high-order metrics could reveal how information interactions fluctuate over time.

Integrating multimodal data (e.g., EEG/MEG with fMRI) and structural constraints from diffusion imaging may provide a more comprehensive view of neural coding. Finally, applying this framework to clinical populations could identify biomarkers of neurological or psychiatric disorders by detecting abnormal information flow, advancing translational neuroscience.


