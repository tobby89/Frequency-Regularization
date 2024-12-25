# Enhancing Gestational Age and Delivery Date Estimation with Frequency Regularization

## Overview

This project explores robust methods for gestational age estimation from fetal fMRI data using frequency regularization. The aim is to improve the accuracy and reliability of gestational age and delivery date predictions, which are critical for prenatal care and reducing maternal mortality rates.

## Motivation

Globally, maternal mortality rates remain high, with unforeseen childbirth being a significant contributor. Accurate estimation of gestational age and delivery dates can significantly mitigate these risks, especially in emergency scenarios. This research focuses on incorporating frequency regularization techniques into existing machine learning models to enhance prediction robustness and segmentation accuracy.

## Approach

### Dataset
The study uses an open-source dataset from [fetal-fMRI - OpenNeuro](https://openneuro.org/), containing 160 cases with 925 volumes of 3D image data.

### Methodology
1. **Preprocessing:** 
   - Detection of fetal brain regions using a pretrained model from prior studies.
   - Ground truth creation for segmentation tasks.
2. **Frequency Regularization:**
   - Parameters manipulated in the frequency domain to suppress irrelevant high-frequency components using zigzag patterns.
   - Reconstruction of spatial tensors via the inverse discrete cosine transform (IDCT).
3. **Evaluation Metrics:**
   - Dice Score comparison between the baseline and enhanced methods.

### Results
- Dice Score improved from **0.3348** to **0.9439** after applying frequency regularization.
- Enhanced segmentation quality, improving the reliability of gestational age predictions and delivery date estimations.

## Key Findings
- The proposed approach demonstrated a **181.95% improvement** in segmentation accuracy.
- Frequency regularization proved effective in reducing parameter redundancy while maintaining high performance.

## Conclusion
This project highlights the potential of frequency regularization to enhance machine learning models in medical imaging. Future work will focus on expanding the dataset and exploring additional robustness improvements.

## References
1. Vahedifard et al., *Artificial Intelligence in Fetal Resting-State Functional MRI Brain Segmentation*, 2023.
2. Huang et al., *Frequency Regularization for Improving Adversarial Robustness*, 2022.
3. [Complete reference list in the paper](#).

## Citation
If you use this code or approach, please cite the original paper:
> Tobias et al., *Robustness Enhancement in fMRI Gestational Age and Delivery Date Estimation with Frequency Regularization*, University of Alberta.