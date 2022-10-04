# MSANA-Online-Data-Stream-Analytics-And-Concept-Drift-Adaptation

This repository contains the code for the paper entitled "**[A Multi-Stage Automated Online Network Data Stream Analytics Framework for IIoT Systems]()**" published in **IEEE Transactions on Industrial Informatics** (Q1, IF: 11.648).  
Authors: Li Yang and Abdallah Shami  
Organization: The Optimized Computing and Communications (OC2) Lab, ECE Department, Western University

In this work, we propose a comprehensive online learning framework for data stream analytics and concept drift adaptation in dynamic environments.  
Two other **tutorial code** for **concept drift, online machine learning, and data stream analytics** can be found in: [PWPAE-Concept-Drift-Detection-and-Adaptation](https://github.com/Western-OC2-Lab/PWPAE-Concept-Drift-Detection-and-Adaptation) and [OASW-Concept-Drift-Detection-and-Adaptation](https://github.com/Western-OC2-Lab/OASW-Concept-Drift-Detection-and-Adaptation)

## Abstract of The Paper
Industry 5.0 aims at maximizing the collaboration between humans and machines. Machines are capable of automating repetitive jobs, while humans handle creative tasks. As a critical component of Industrial Internet of Things (IIoT) systems for service delivery, network data stream analytics often encounter concept drift issues due to dynamic IIoT environments, causing performance degradation and automation difficulties. In this paper, we propose a novel Multi-Stage Automated Network Analytics (MSANA) framework for concept drift adaptation in IIoT systems, consisting of dynamic data pre-processing, the proposed Drift-based Dynamic Feature Selection (DD-FS) method, dynamic model learning & selection, and the proposed Window-based Performance Weighted Probability Averaging Ensemble (W-PWPAE) model. It is a complete automated data stream analytics framework that enables automatic, effective, and efficient data analytics for IIoT systems in Industry 5.0. Experimental results on two public IoT datasets demonstrate that the proposed framework outperforms state-of-the-art methods for IIoT data stream analytics. 

## Implementation 

### AutoML Pipeline and Procedures
<p align="center">
<img src="https://github.com/Western-OC2-Lab/MSANA-Online-Data-Stream-Analytics-And-Concept-Drift-Adaptation/blob/main/System_Overview.jpg" width="600" />
</p>

1. Dynamic Data Pre-Processing
   * Data Balancing
   * Data Normalization
2. Dynamic Feature Engineering
   * Drift-based Dynamic Feature Selection
3. Based Model Learning and Selection
   * Online Base Model Learning
   * Dynamic Model Selection
4. Online Ensemble Model Development
   * Online Model Ensemble
   * Concept Drift Detection

### Online Learning/Concept Drift Adaptation Algorithms  
* Adaptive Random Forest (ARF) with ADWIN drift detector
* Adaptive Random Forest (ARF) with EDDM drift detector
* Streaming Random Patches (SRP)
* Extremely Fast Decision Tree (EFDT)
* K-Nearest Neighbors (KNN) classifier with ADWIN change detector (KNN-ADWIN)
* Self Adapting Memory (SAM) KNN model (SAM-KNN)
* Online Passive-Aggressive (OPA)
* Leveraging Bagging (LB)
* Performance Weighted Probability Averaging Ensemble (PWPAE)
  * Proposed in the previous work
* Window-based Performance Weighted Probability Averaging Ensemble (W-PWPAE)
  * Proposed

### Drift Detection Algorithms
* Adaptive Windowing (ADWIN)
* Early Drift Detection Method (EDDM)

### Dataset 
1. CICIDS2017 dataset, a popular network traffic dataset for intrusion detection problems
   * Publicly available at: https://www.unb.ca/cic/datasets/ids-2017.html  

2. IoTID20 dataset, a novel IoT botnet dataset
   * Publicly available at: https://sites.google.com/view/iot-network-intrusion-dataset/home

### Code  
* [TII-MSANA-CICIDS2017.ipynb](https://github.com/Western-OC2-Lab/MSANA-Online-Data-Stream-Analytics-And-Concept-Drift-Adaptation/blob/main/TII-MSANA-CICIDS2017.ipynb): code for the sampled CICIDS2017 dataset.  
* [TII-MSANA-IoTID20.ipynb](https://github.com/Western-OC2-Lab/MSANA-Online-Data-Stream-Analytics-And-Concept-Drift-Adaptation/blob/main/TII-MSANA-IoTID20.ipynb): code for the sampled IoTID20 dataset.

### Requirements & Libraries  
* Python 3.6+
* [Scikit-learn](https://scikit-learn.org/stable/)  
* [LightGBM](https://lightgbm.readthedocs.io/en/latest/)
* [River](https://riverml.xyz/dev/)

## Contact-Info
Please feel free to contact me for any questions or cooperation opportunities. I'd be happy to help.
* Email: [liyanghart@gmail.com](mailto:liyanghart@gmail.com)
* GitHub: [LiYangHart](https://github.com/LiYangHart) and [Western OC2 Lab](https://github.com/Western-OC2-Lab/)
* LinkedIn: [Li Yang](https://www.linkedin.com/in/li-yang-phd-65a190176/)  
* Google Scholar: [Li Yang](https://scholar.google.com.eg/citations?user=XEfM7bIAAAAJ&hl=en) and [OC2 Lab](https://scholar.google.com.eg/citations?user=oiebNboAAAAJ&hl=en)

## Citation
If you find this repository useful in your research, please cite this article as:  

L. Yang and A. Shami, “A Multi-Stage Automated Online Network Data Stream Analytics Framework for IIoT Systems,” *IEEE Transactions on Industrial Informatics*, 2022.  

```
@article{YANG20221818,
title = "A Multi-Stage Automated Online Network Data Stream Analytics Framework for IIoT Systems",
author = "Li Yang and Abdallah Shami",
journal = "IEEE Transactions on Industrial Informatics",
pages = {1-10},
year = "2022",
}
