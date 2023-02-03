---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

2022
===
**Prediction of inter-chain distance maps of protein complexes with 2D attention-based deep neural networks**  
<u>Zhiye Guo</u>, Jian Liu, Jeffrey Skolnick, Jianlin Cheng  
*Nature Communications 13 (1), 6963*  
<details><summary>ABSTRACT</summary> 
Residue-residue distance information is useful for predicting tertiary structures of protein monomers or quaternary structures of protein complexes. Many deep learning methods have been developed to predict intra-chain residue-residue distances of monomers accurately, but few methods can accurately predict inter-chain residue-residue distances of complexes. We develop a deep learning method CDPred (i.e., Complex Distance Prediction) based on the 2D attention-powered residual network to address the gap. Tested on two homodimer datasets, CDPred achieves the precision of 60.94% and 42.93% for top L/5 inter-chain contact predictions (L: length of the monomer in homodimer), respectively, substantially higher than DeepHomo’s 37.40% and 23.08% and GLINTER’s 48.09% and 36.74%. Tested on the two heterodimer datasets, the top Ls/5 inter-chain contact prediction precision (Ls: length of the shorter monomer in heterodimer) of CDPred is 47.59% and 22.87% respectively, surpassing GLINTER’s 23.24% and 13.49%. Moreover, the prediction of CDPred is complementary with that of AlphaFold2-multimer.
</details>

<a href='https://www.nature.com/articles/s41467-022-34600-2' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href='https://github.com/BioinfoMachineLearning/CDPred' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a> 

**Multi-head attention-based U-Nets for predicting protein domain boundaries using 1D sequence features and 2D distance maps**  
Sajid Mahmud, <u>Zhiye Guo</u>, Farhan Quadir, Jian Liu, Jianlin Cheng  
*BMC bioinformatics 23 (1), 283*  
<details><summary>ABSTRACT</summary> 
The information about the domain architecture of proteins is useful for studying protein structure and function. However, accurate prediction of protein domain boundaries (i.e., sequence regions separating two domains) from sequence remains a significant challenge. In this work, we develop a deep learning method based on multi-head U-Nets (called DistDom) to predict protein domain boundaries utilizing 1D sequence features and predicted 2D inter-residue distance map as input. The 1D features contain the evolutionary and physicochemical information of protein sequences, whereas the 2D distance map includes the structural information of proteins that was rarely used in domain boundary prediction before. The 1D and 2D features are processed by the 1D and 2D U-Nets respectively to generate hidden features. The hidden features are then used by the multi-head attention to predict the probability of each residue of a protein being in a domain boundary, leveraging both local and global information in the features. The residue-level domain boundary predictions can be used to classify proteins as single-domain or multi-domain proteins. It classifies the CASP14 single-domain and multi-domain targets at the accuracy of 75.9%, 13.28% more accurate than the state-of-the-art method. Tested on the CASP14 multi-domain protein targets with expert annotated domain boundaries, the average per-target F1 measure score of the domain boundary prediction by DistDom is 0.263, 29.56% higher than the state-of-the-art method.
</details>

<a href='https://link.springer.com/article/10.1186/s12859-022-04829-1' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href='https://github.com/jianlin-cheng/DistDom' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a> 


**Distance‐based reconstruction of protein quaternary structures from inter‐chain contacts**  
Elham Soltanikazemi, Farhan Quadir, Raj S Roy, <u>Zhiye Guo</u>, Jianlin Cheng  
*Proteins: Structure, Function, and Bioinformatics 90 (3), 720-731*  
<details><summary>ABSTRACT</summary> 
Predicting the quaternary structure of protein complex is an important problem. Inter-chain residue-residue contact prediction can provide useful information to guide the ab initio reconstruction of quaternary structures. However, few methods have been developed to build quaternary structures from predicted inter-chain contacts. Here, we develop the first method based on gradient descent optimization (GD) to build quaternary structures of protein dimers utilizing inter-chain contacts as distance restraints. We evaluate GD on several datasets of homodimers and heterodimers using true/predicted contacts and monomer structures as input. GD consistently performs better than both simulated annealing and Markov Chain Monte Carlo simulation. Starting from an arbitrarily quaternary structure randomly initialized from the tertiary structures of protein chains and using true inter-chain contacts as input, GD can reconstruct high-quality structural models for homodimers and heterodimers with average TM-score ranging from 0.92 to 0.99 and average interface root mean square distance from 0.72 Å to 1.64 Å. On a dataset of 115 homodimers, using predicted inter-chain contacts as restraints, the average TM-score of the structural models built by GD is 0.76. For 46% of the homodimers, high-quality structural models with TM-score ≥ 0.9 are reconstructed from predicted contacts. There is a strong correlation between the quality of the reconstructed models and the precision and recall of predicted contacts. Only a moderate precision or recall of inter-chain contact prediction is needed to build good structural models for most homodimers. Moreover, GD improves the quality of quaternary structures predicted by AlphaFold2 on a Critical Assessment of Techniques for Protein Structure Prediction–Critical Assessments of Predictions of Interactions dataset.
</details>

<a href='https://onlinelibrary.wiley.com/doi/full/10.1002/prot.26269' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href='https://github.com/jianlin-cheng/DeepComplex2' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a> 

**Improving protein tertiary structure prediction by deep learning and distance prediction in CASP14**  
Jian Liu, Tianqi Wu, <u>Zhiye Guo</u>, Jie Hou, Jianlin Cheng  
*Proteins: Structure, Function, and Bioinformatics 90 (1), 58-72*    
<details><summary>ABSTRACT</summary> 
Substantial progresses in protein structure prediction have been made by utilizing deep-learning and residue-residue distance prediction since CASP13. Inspired by the advances, we improve our CASP14 MULTICOM protein structure prediction system by incorporating three new components: (a) a new deep learning-based protein inter-residue distance predictor to improve template-free (ab initio) tertiary structure prediction, (b) an enhanced template-based tertiary structure prediction method, and (c) distance-based model quality assessment methods empowered by deep learning. In the 2020 CASP14 experiment, MULTICOM predictor was ranked seventh out of 146 predictors in tertiary structure prediction and ranked third out of 136 predictors in inter-domain structure prediction. The results demonstrate that the template-free modeling based on deep learning and residue-residue distance prediction can predict the correct topology for almost all template-based modeling targets and a majority of hard targets (template-free targets or targets whose templates cannot be recognized), which is a significant improvement over the CASP13 MULTICOM predictor. Moreover, the template-free modeling performs better than the template-based modeling on not only hard targets but also the targets that have homologous templates. The performance of the template-free modeling largely depends on the accuracy of distance prediction closely related to the quality of multiple sequence alignments. The structural model quality assessment works well on targets for which enough good models can be predicted, but it may perform poorly when only a few good models are predicted for a hard target and the distribution of model quality scores is highly skewed. MULTICOM is available at https://github.com/jianlin-cheng/MULTICOM_Human_CASP14/tree/CASP14_DeepRank3 and https://github.com/multicom-toolbox/multicom/tree/multicom_v2.0.
</details>

<a href='https://onlinelibrary.wiley.com/doi/full/10.1002/prot.26186' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href='https://github.com/multicom-toolbox/multicom/tree/multicom_v2.0' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a> 

2021
===

**Improving deep learning-based protein distance prediction in CASP14**  
<u>Zhiye Guo</u>*, Tianqi Wu*, Jian Liu, Jie Hou, Jianlin Cheng     
*Bioinformatics 37 (19), 3190-3196*      
<details><summary>ABSTRACT</summary> 
<strong>Motivation</strong>

Accurate prediction of residue–residue distances is important for protein structure prediction. We developed several protein distance predictors based on a deep learning distance prediction method and blindly tested them in the 14th Critical Assessment of Protein Structure Prediction (CASP14). The prediction method uses deep residual neural networks with the channel-wise attention mechanism to classify the distance between every two residues into multiple distance intervals. The input features for the deep learning method include co-evolutionary features as well as other sequence-based features derived from multiple sequence alignments (MSAs). Three alignment methods are used with multiple protein sequence/profile databases to generate MSAs for input feature generation. Based on different configurations and training strategies of the deep learning method, five MULTICOM distance predictors were created to participate in the CASP14 experiment.

<strong>Results</strong>  
Benchmarked on 37 hard CASP14 domains, the best performing MULTICOM predictor is ranked 5th out of 30 automated CASP14 distance prediction servers in terms of precision of top L/5 long-range contact predictions [i.e. classifying distances between two residues into two categories: in contact (<8 Angstrom) and not in contact otherwise] and performs better than the best CASP13 distance prediction method. The best performing MULTICOM predictor is also ranked 6th among automated server predictors in classifying inter-residue distances into 10 distance intervals defined by CASP14 according to the precision of distance classification. The results show that the quality and depth of MSAs depend on alignment methods and sequence databases and have a significant impact on the accuracy of distance prediction. Using larger training datasets and multiple complementary features improves prediction accuracy. However, the number of effective sequences in MSAs is only a weak indicator of the quality of MSAs and the accuracy of predicted distance maps. In contrast, there is a strong correlation between the accuracy of contact/distance predictions and the average probability of the predicted contacts, which can therefore be more effectively used to estimate the confidence of distance predictions and select predicted distance maps. 
</details>

<a href='https://academic.oup.com/bioinformatics/article/37/19/3190/6271413' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href=' https://github.com/multicom-toolbox/deepdist' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a> 


**MULTICOM2 open-source protein structure prediction system powered by deep learning and distance prediction**  
Tianqi Wu, Jian Liu, <u>Zhiye Guo</u>, Jie Hou, Jianlin Cheng    
*Scientific reports 11 (1), 13155*      
<details><summary>ABSTRACT</summary> 
Protein structure prediction is an important problem in bioinformatics and has been studied for decades. However, there are still few open-source comprehensive protein structure prediction packages publicly available in the field. In this paper, we present our latest open-source protein tertiary structure prediction system—MULTICOM2, an integration of template-based modeling (TBM) and template-free modeling (FM) methods. The template-based modeling uses sequence alignment tools with deep multiple sequence alignments to search for structural templates, which are much faster and more accurate than MULTICOM1. The template-free (ab initio or de novo) modeling uses the inter-residue distances predicted by DeepDist to reconstruct tertiary structure models without using any known structure as template. In the blind CASP14 experiment, the average TM-score of the models predicted by our server predictor based on the MULTICOM2 system is 0.720 for 58 TBM (regular) domains and 0.514 for 38 FM and FM/TBM (hard) domains, indicating that MULTICOM2 is capable of predicting good tertiary structures across the board. It can predict the correct fold for 76 CASP14 domains (95% regular domains and 55% hard domains) if only one prediction is made for a domain. The success rate is increased to 3% for both regular and hard domains if five predictions are made per domain. Moreover, the prediction accuracy of the pure template-free structure modeling method on both TBM and FM targets is very close to the combination of template-based and template-free modeling methods. This demonstrates that the distance-based template-free modeling method powered by deep learning can largely replace the traditional template-based modeling method even on TBM targets that TBM methods used to dominate and therefore provides a uniform structure modeling approach to any protein. Finally, on the 38 CASP14 FM and FM/TBM hard domains, MULTICOM2 server predictors (MULTICOM-HYBRID, MULTICOM-DEEP, MULTICOM-DIST) were ranked among the top 20 automated server predictors in the CASP14 experiment. After combining multiple predictors from the same research group as one entry, MULTICOM-HYBRID was ranked no. 5. The source code of MULTICOM2 is freely available at https://github.com/multicom-toolbox/multicom/tree/multicom_v2.0.
</details>

<a href='https://www.nature.com/articles/s41598-021-92395-6' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href=' https://github.com/multicom-toolbox/multicom/tree/multicom_v2.0' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a> 


**DeepDist: real-value inter-residue distance prediction with deep residual convolutional network**  
Tianqi Wu*, <u>Zhiye Guo</u>*, Jie Hou, Jianlin Cheng   
*BMC bioinformatics 22, 1-17*    
<details><summary>ABSTRACT</summary> 
<strong>Background</strong>

Driven by deep learning, inter-residue contact/distance prediction has been significantly improved and substantially enhanced ab initio protein structure prediction. Currently, most of the distance prediction methods classify inter-residue distances into multiple distance intervals instead of directly predicting real-value distances. The output of the former has to be converted into real-value distances to be used in tertiary structure prediction.

<strong>Results</strong>  
To explore the potentials of predicting real-value inter-residue distances, we develop a multi-task deep learning distance predictor (DeepDist) based on new residual convolutional network architectures to simultaneously predict real-value inter-residue distances and classify them into multiple distance intervals. Tested on 43 CASP13 hard domains, DeepDist achieves comparable performance in real-value distance prediction and multi-class distance prediction. The average mean square error (MSE) of DeepDist’s real-value distance prediction is 0.896 Å2 when filtering out the predicted distance ≥ 16 Å, which is lower than 1.003 Å2 of DeepDist’s multi-class distance prediction. When distance predictions are converted into contact predictions at 8 Å threshold (the standard threshold in the field), the precision of top L/5 and L/2 contact predictions of DeepDist’s multi-class distance prediction is 79.3% and 66.1%, respectively, higher than 78.6% and 64.5% of its real-value distance prediction and the best results in the CASP13 experiment.
</details>

<a href='https://link.springer.com/article/10.1186/s12859-021-03960-9' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href='https://github.com/multicom-toolbox/deepdist' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a> 


**Combination of deep neural network with attention mechanism enhances the explainability of protein contact prediction**  
Chen Chen, Tianqi Wu, <u>Zhiye Guo</u>, Jianlin Cheng   
*Proteins: Structure, Function, and Bioinformatics 89 (6), 697-707*    
<details><summary>ABSTRACT</summary> 
Deep learning has emerged as a revolutionary technology for protein residue-residue contact prediction since the 2012 CASP10 competition. Considerable advancements in the predictive power of the deep learning-based contact predictions have been achieved since then. However, little effort has been put into interpreting the black-box deep learning methods. Algorithms that can interpret the relationship between predicted contact maps and the internal mechanism of the deep learning architectures are needed to explore the essential components of contact inference and improve their explainability. In this study, we present an attention-based convolutional neural network for protein contact prediction, which consists of two attention mechanism-based modules: sequence attention and regional attention. Our benchmark results on the CASP13 free-modeling targets demonstrate that the two attention modules added on top of existing typical deep learning models exhibit a complementary effect that contributes to prediction improvements. More importantly, the inclusion of the attention mechanism provides interpretable patterns that contain useful insights into the key fold-determining residues in proteins. We expect the attention-based model can provide a reliable and practically interpretable technique that helps break the current bottlenecks in explaining deep neural networks for contact prediction. The source code of our method is available at https://github.com/jianlin-cheng/InterpretContactMap.
</details>

<a href='https://onlinelibrary.wiley.com/doi/full/10.1002/prot.26052' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href='https://github.com/jianlin-cheng/InterpretContactMap' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a> 


**Protein model accuracy estimation empowered by deep learning and inter-residue distance prediction in CASP14**  
Xiao Chen*, Jian Liu*, <u>Zhiye Guo</u>*, Tianqi Wu*, Jie Hou*, Jianlin Cheng  
*Scientific Reports 11 (1), 10943*    
<details><summary>ABSTRACT</summary> 
The inter-residue contact prediction and deep learning showed the promise to improve the estimation of protein model accuracy (EMA) in the 13th Critical Assessment of Protein Structure Prediction (CASP13). To further leverage the improved inter-residue distance predictions to enhance EMA, during the 2020 CASP14 experiment, we integrated several new inter-residue distance features with the existing model quality assessment features in several deep learning methods to predict the quality of protein structural models. According to the evaluation of performance in selecting the best model from the models of CASP14 targets, our three multi-model predictors of estimating model accuracy (MULTICOM-CONSTRUCT, MULTICOM-AI, and MULTICOM-CLUSTER) achieve the averaged loss of 0.073, 0.079, and 0.081, respectively, in terms of the global distance test score (GDT-TS). The three methods are ranked first, second, and third out of all 68 CASP14 predictors. MULTICOM-DEEP, the single-model predictor of estimating model accuracy (EMA), is ranked within top 10 among all the single-model EMA methods according to GDT-TS score loss. The results demonstrate that inter-residue distance features are valuable inputs for deep learning to predict the quality of protein structural models. However, larger training datasets and better ways of leveraging inter-residue distance information are needed to fully explore its potentials.
</details>

<a href='https://www.nature.com/articles/s41598-021-90303-6' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  

2020
===

**DNSS2: Improved ab initio protein secondary structure prediction using advanced deep learning architectures**  
<u>Zhiye Guo</u>*, Jie Hou*, Jianlin Cheng   
*Proteins: Structure, Function, and Bioinformatics 89 (2), 207-217*    
<details><summary>ABSTRACT</summary> 
Accurate prediction of protein secondary structure (alpha-helix, beta-strand and coil) is a crucial step for protein inter-residue contact prediction and ab initio tertiary structure prediction. In a previous study, we developed a deep belief network-based protein secondary structure method (DNSS1) and successfully advanced the prediction accuracy beyond 80%. In this work, we developed multiple advanced deep learning architectures (DNSS2) to further improve secondary structure prediction. The major improvements over the DNSS1 method include (a) designing and integrating six advanced one-dimensional deep convolutional/recurrent/residual/memory/fractal/inception networks to predict 3-state and 8-state secondary structure, and (b) using more sensitive profile features inferred from Hidden Markov model (HMM) and multiple sequence alignment (MSA). Most of the deep learning architectures are novel for protein secondary structure prediction. DNSS2 was systematically benchmarked on independent test data sets with eight state-of-art tools and consistently ranked as one of the best methods. Particularly, DNSS2 was tested on the protein targets of 2018 CASP13 experiment and achieved the Q3 score of 81.62%, SOV score of 72.19%, and Q8 score of 73.28%. DNSS2 is freely available at: https://github.com/multicom-toolbox/DNSS2.
</details>

<a href='https://onlinelibrary.wiley.com/doi/abs/10.1002/prot.26007' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href='https://github.com/multicom-toolbox/DNSS2' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a>  


**Deep ranking in template-free protein structure prediction**  
Xiao Chen, Nasrin Akhter, <u>Zhiye Guo</u>, Tianqi Wu, Jie Hou, Amarda Shehu, Jianlin Cheng  
*Proceedings of the 11th ACM international conference on bioinformatics, computational biology and health informatics*    
<details><summary>ABSTRACT</summary> 
The road to the discovery of the biological activities of a protein molecule in the cell goes through knowledge of its three-dimensional, biologically-active structure(s). Current evidence suggests significant regions of the protein universe are inaccessible by either wet-laboratory structure determination or homology modeling. While great progress has been made by computational approaches in elucidating dark regions of the proteome, inherent challenges remain. In this paper, we advance research on addressing one such a challenge known as model (quality) assessment. In essence, the task involves discriminating relevant structure(s) among many computed for a protein of interest. We propose a method based on deep learning and evaluate it on tertiary structures computed by a popular de-novo platform on benchmark datasets. The method uses novel protein residue-residue distance features, improved residue-residue contacts, together with other features, such as energies and model topology similarity, to estimate the quality of protein models. A detailed evaluation shows that the proposed method outperforms related ones and advances the state of the art in model assessment.
</details>

<a href='https://dl.acm.org/doi/abs/10.1145/3388440.3412469' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a> 


**The MULTICOM protein structure prediction server empowered by deep learning and contact distance prediction**  
Jie Hou, Tianqi Wu, <u>Zhiye Guo</u>, Farhan Quadir, Jianlin Cheng  
*Protein structure prediction, 13-26*     
<details><summary>ABSTRACT</summary> 
Prediction of the three-dimensional (3D) structure of a protein from its sequence is important for studying its biological function. With the advancement in deep learning contact distance prediction and residue–residue coevolutionary analysis, significant progress has been made in both template-based and template-free protein structure prediction in the last several years. Here, we provide a practical guide for our latest MULTICOM protein structure prediction system built on top of the latest advances, which was rigorously tested in the 2018 CASP13 experiment. Its specific functionalities include: (1) prediction of 1D structural features (secondary structure, solvent accessibility, disordered regions) and 2D interresidue contacts; (2) domain boundary prediction; (3) template-based (or homology) 3D structure modeling; (4) contact distance-driven ab initio 3D structure modeling; and (5) large-scale protein quality assessment enhanced by deep learning and predicted contacts. The MULTICOM web server (http://sysbio.rnet.missouri.edu/multicom_cluster/) presents all the 1D, 2D, and 3D prediction results and quality assessment to users via user-friendly web interfaces and e-mails. The source code of the MULTICOM package is also available at https://github.com/multicom-toolbox/multicom.
</details>

<a href='https://link.springer.com/protocol/10.1007/978-1-0716-0708-4_2' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a>  <a href='https://github.com/multicom-toolbox/multicom' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/CODE-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00FFB2'/></a>  

2017
===

**Resistance welding spot defect detection with convolutional neural networks**  
Zhiye Guo, Shaofeng Ye, Yiju Wang, Chun Lin  
*Computer Vision Systems: 11th International Conference, ICVS 2017*     
<details><summary>ABSTRACT</summary> 
A convolutional neural network based method is proposed in this paper to classify the images of resistance welding spot. The features of resistance wielding spots are very complex and diverse, which made it difficult to separate the good ones and the bad ones using hard threshold. Several types of convolutional neural networks with different depths and layer nodes are built to learn the features of welding spot. 10 thousand labeled images are used for training and 3 hundred images are used to test the network. As a result, we get a 99.01% accuracy on test images, which is 97.70% better than human inspection.
</details>

<a href='https://link.springer.com/chapter/10.1007/978-3-319-68345-4_15' target="_blank"><img alt='LINK' src='https://img.shields.io/badge/PAPER_LINK-100000?style=for-the-badge&logo=LINK&logoColor=9A8787&labelColor=0072EE&color=00B2FF'/></a> 

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
