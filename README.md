# Dictionary-Learning-Augmented-Cosmic-Ray-Detection
For any queries, please contact at ee19resch01008@iith.ac.in

# Abstract
In this work, we propose a novel Dictionary Learning (DL) based framework to detect Cosmic Ray (CR) hits that contaminate the astronomical images obtained through optical photometric surveys. The unique and distinguishable spatial signatures of CR hits compared to other actual astrophysical sources in the image motivated us to characterize the CR patches uniquely via their sparse representations obtained from a learned dictionary. Specifically, the dictionary is trained on images acquired from the Dark Energy Camera (DECam) observations. Next, the learned dictionary is used to represent the CR and Non-CR patches (e.g., each patch is with $11 \times 11$ pixel resolution) extracted from the original images. A Machine Learning (ML) classifier is then trained to classify the CR and Non-CR patches. Empirically, we demonstrate that the proposed DL-based method can detect the CR hits at patch level and provide approximately $83\%$ detection rates at 0.1 $\%$ false positives on the DECam test data with Random Forest (RF) algorithm.Further, we used the coarse segmentation maps obtained from the classifier output to guide the deep-learning-based CR segmentation models. The coarse maps are fed through a separate channel along with the contaminated image to detect the CR-induced pixels more accurately. We evaluated the performance of proposed DL-guided deep segmentation models over the baseline on test data from DECam. We demonstrate that the proposed method provides additional guidance to the baseline models in terms of faster convergence rate and improves CR detection performance by $2\%$ in the case of shallow models. 

# Publication
This work is accepted to the "30 th European Signal Processing Conference", EUSIPCO - 2022.

# Acknowledgment
We considered our codes mainly from the following sources.
1. https://github.com/profjsb/deepCR (deepCR)
2. https://github.com/nel215/ksvd (Approximate K-SVD)
