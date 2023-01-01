# MSANA-Online-Data-Stream-Analytics-And-Concept-Drift-Adaptation

This repository contains the code for the paper entitled "**[A Multi-Stage Automated Online Network Data Stream Analytics Framework for IIoT Systems](https://arxiv.org/pdf/2210.01985.pdf)**" published in **IEEE Transactions on Industrial Informatics** (Q1, IF: 11.648), doi: [10.1109/TII.2022.3212003](https://ieeexplore.ieee.org/document/9910406).  
Authors: Li Yang and Abdallah Shami  
Organization: The Optimized Computing and Communications (OC2) Lab, ECE Department, Western University

In this work, we propose a comprehensive online learning framework for data stream analytics and concept drift adaptation in dynamic environments.  
Two other **tutorial code** for **concept drift, online machine learning, and data stream analytics** can be found in: [PWPAE-Concept-Drift-Detection-and-Adaptation](https://github.com/Western-OC2-Lab/PWPAE-Concept-Drift-Detection-and-Adaptation) and [OASW-Concept-Drift-Detection-and-Adaptation](https://github.com/Western-OC2-Lab/OASW-Concept-Drift-Detection-and-Adaptation)

## Paper Link
[Open access version on arXiv](https://arxiv.org/pdf/2210.01985.pdf)  
[Published version on IEEE](https://ieeexplore.ieee.org/document/9910406)  

## Abstract of The Paper
Industry 5.0 aims at maximizing the collaboration between humans and machines. Machines are capable of automating repetitive jobs, while humans handle creative tasks. As a critical component of Industrial Internet of Things (IIoT) systems for service delivery, network data stream analytics often encounter concept drift issues due to dynamic IIoT environments, causing performance degradation and automation difficulties. In this paper, we propose a novel Multi-Stage Automated Network Analytics (MSANA) framework for concept drift adaptation in IIoT systems, consisting of dynamic data pre-processing, the proposed Drift-based Dynamic Feature Selection (DD-FS) method, dynamic model learning & selection, and the proposed Window-based Performance Weighted Probability Averaging Ensemble (W-PWPAE) model. It is a complete automated data stream analytics framework that enables automatic, effective, and efficient data analytics for IIoT systems in Industry 5.0. Experimental results on two public IoT datasets demonstrate that the proposed framework outperforms state-of-the-art methods for IIoT data stream analytics. 

## Concept Drift
In non-stationary and dynamical environments, such as IoT environments, the distribution of input data often changes over time, known as concept drift. The occurrence of concept drift will result in the performance degradation of the current trained data analytics model. Traditional offline machine learning (ML) models cannot deal with concept drift, making it necessary to develop online adaptive analytics models that can adapt to the predictable and unpredictable changes in data streams. 

To address concept drift, effective methods should be able to detect concept drift and adapt to the changes accordingly. Therefore, concept drift detection and adaptation are the two major steps for online learning on data streams.

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
* Adaptive Random Forest (ARF) with ADWIN drift detector (ARF-ADWIN)
* Adaptive Random Forest (ARF) with EDDM drift detector (ARF-EDDM)
* Streaming Random Patches (SRP)
* Extremely Fast Decision Tree (EFDT)
* K-Nearest Neighbors (KNN) classifier with ADWIN change detector (KNN-ADWIN)
* Self Adapting Memory (SAM) KNN model (SAM-KNN)
* Online Passive-Aggressive (OPA)
* Leveraging Bagging (LB)
* Performance Weighted Probability Averaging Ensemble (PWPAE)
  * Proposed in the [previous work](https://github.com/Western-OC2-Lab/PWPAE-Concept-Drift-Detection-and-Adaptation)
* Window-based Performance Weighted Probability Averaging Ensemble (W-PWPAE)
  * Proposed in this work

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
* [River](https://riverml.xyz/dev/)

## Contact-Info
Please feel free to contact me for any questions or cooperation opportunities. I'd be happy to help.
* Email: [liyanghart@gmail.com](mailto:liyanghart@gmail.com)
* GitHub: [LiYangHart](https://github.com/LiYangHart) and [Western OC2 Lab](https://github.com/Western-OC2-Lab/)
* LinkedIn: [Li Yang](https://www.linkedin.com/in/li-yang-phd-65a190176/)  
* Google Scholar: [Li Yang](https://scholar.google.com.eg/citations?user=XEfM7bIAAAAJ&hl=en) and [OC2 Lab](https://scholar.google.com.eg/citations?user=oiebNboAAAAJ&hl=en)

## Citation
If you find this repository useful in your research, please cite this article as:  

L. Yang and A. Shami, “A Multi-Stage Automated Online Network Data Stream Analytics Framework for IIoT Systems,” *IEEE Transactions on Industrial Informatics*, vol. 19, no. 2, pp. 2107-2116, Feb. 2023, doi: 10.1109/TII.2022.3212003.  

```
@ARTICLE{9910406,
  author={Yang, Li and Shami, Abdallah},
  journal={IEEE Transactions on Industrial Informatics}, 
  title={A Multi-Stage Automated Online Network Data Stream Analytics Framework for IIoT Systems}, 
  year={2023},
  volume={19},
  number={2},
  pages={2107-2116},
  doi={10.1109/TII.2022.3212003}}
```
