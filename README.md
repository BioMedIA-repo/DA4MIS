# BioMedIA👩‍💻.
* **[New], We are reformatting the codebase to support the 5-fold cross-validation and randomly select labeled cases, the reformatted methods in this [Branch](https://github.com/HiLab-git/SSL4MIS/tree/cross_val_dev)**. 
* Recently, semi-supervised image segmentation has become a hot topic in medical image computing, unfortunately, there are only a few open-source codes and datasets, since the privacy policy and others. For easy evaluation and fair comparison, we are trying to build a semi-supervised medical image segmentation benchmark to boost the semi-supervised learning research in the medical image computing community. **If you are interested, you can push your implementations or ideas to this repo or contact [me](https://luoxd1996.github.io/) at any time**.  
* This repo has re-implemented these semi-supervised methods (with some modifications for semi-supervised medical image segmentation, more details please refer to these original works): (1) [Mean Teacher](https://papers.nips.cc/paper/6719-mean-teachers-are-better-role-models-weight-averaged-consistency-targets-improve-semi-supervised-deep-learning-results.pdf); (2) [Entropy Minimization](https://openaccess.thecvf.com/content_CVPR_2019/papers/Vu_ADVENT_Adversarial_Entropy_Minimization_for_Domain_Adaptation_in_Semantic_Segmentation_CVPR_2019_paper.pdf); (3) [Deep Adversarial Networks](https://link.springer.com/chapter/10.1007/978-3-319-66179-7_47); (4) [Uncertainty Aware Mean Teacher](https://arxiv.org/pdf/1907.07034.pdf); (5) [Interpolation Consistency Training](https://arxiv.org/pdf/1903.03825.pdf); (6) [Uncertainty Rectified Pyramid Consistency](https://arxiv.org/pdf/2012.07042.pdf); (7) [Cross Pseudo Supervision](https://arxiv.org/abs/2106.01226); (8) [Cross Consistency Training](https://openaccess.thecvf.com/content_CVPR_2020/papers/Ouali_Semi-Supervised_Semantic_Segmentation_With_Cross-Consistency_Training_CVPR_2020_paper.pdf); (9) [Deep Co-Training](https://openaccess.thecvf.com/content_ECCV_2018/papers/Siyuan_Qiao_Deep_Co-Training_for_ECCV_2018_paper.pdf); (10) [Cross Teaching between CNN and Transformer](https://arxiv.org/pdf/2112.04894.pdf); (11) [FixMatch](https://arxiv.org/abs/2001.07685); (12) [Regularized Dropout](https://proceedings.neurips.cc/paper/2021/file/5a66b9200f29ac3fa0ae244cc2a51b39-Paper.pdf). In addition, several backbones networks (both 2D and 3D) are also supported in this repo, such as **UNet, nnUNet, VNet, AttentionUNet, ENet, Swin-UNet, etc**. 
# 123456
* This project was originally developed for our previous works. Now and future, we are still working on extending it to be more user-friendly and support more approaches to further boost and ease this topic research. **If you use this codebase in your research, please cite the following works**:
  11111111111
```shell
  @article{jin2024inter,
  title={Inter-and intra-uncertainty based feature aggregation model for semi-supervised histopathology image segmentation},
  author={Jin, Qiangguo and Cui, Hui and Sun, Changming and Song, Yang and Zheng, Jiangbin and Cao, Leilei and Wei, Leyi and Su, Ran},
  journal={Expert Systems with Applications},
  volume={238},
  pages={122093},
  year={2024},
  publisher={Elsevier}
}

@inproceedings{jin2022semi,
  title={Semi-supervised histological image segmentation via hierarchical consistency enforcement},
  author={Jin, Qiangguo and Cui, Hui and Sun, Changming and Zheng, Jiangbin and Wei, Leyi and Fang, Zhenyu and Meng, Zhaopeng and Su, Ran},
  booktitle={International Conference on Medical Image Computing and Computer-Assisted Intervention},
  pages={3--13},
  year={2022},
  organization={Springer}
}

  ```
  
## Literature reviews of semi-supervised learning approach for medical image segmentation (**SSL4MIS**).
|Date|The First and Last Authors|Title|Code|Reference|
|---|---|---|---|---|
|2023-07|H. Wang and X. Li|DHC: Dual-debiased Heterogeneous Co-training Framework for Class-imbalanced Semi-supervised Medical Image Segmentation|[Code](https://github.com/xmed-lab/DHC)|[MICCAI2023](https://arxiv.org/pdf/2307.11960.pdf)|
|2023-07|Q. Wei and Y. Zhou|Consistency-guided Meta-Learning for Bootstrapping Semi-Supervised Medical Image Segmentation|[Code](https://github.com/aijinrjinr/MLB-Seg)|[MICCAI2023](https://arxiv.org/pdf/2307.11604.pdf)|
|2023-07|H. Peiris and M. Harandi|Uncertainty-guided dual-views for semi-supervised volumetric medical image segmentation|[Code](https://github.com/himashi92/Co-BioNet)|[Nature Machine Intelligence](https://www.nature.com/articles/s42256-023-00682-w)|
|2023-07|S. Gao and S. Zhang|Correlation-Aware Mutual Learning for Semi-supervised Medical Image Segmentation|[Code](https://github.com/Herschel555/CAML)|[MICCAI2023](https://arxiv.org/pdf/2307.06312.pdf)|
|2023-07|Z. Xu and R. Tong|Ambiguity-selective consistency regularization for mean-teacher semi-supervised medical image segmentation|[Code](https://github.com/lemoshu/AC-MT)|[MedIA2023](https://www.sciencedirect.com/science/article/pii/S1361841523001408)|
|2023-06|P. Liu and G. Zheng|C3PS: Context-aware Conditional Cross Pseudo Supervision for Semi-supervised Medical Image Segmentation|None|[Arxiv](https://arxiv.org/pdf/2306.08275.pdf)|
|2023-05|Z. Zhang and Z. Jiao|Cross-supervised Dual Classifiers for Semi-supervised Medical Image Segmentation|None|[Arxiv](https://arxiv.org/pdf/2305.16216.pdf)|
|2023-05|Z. Zhang and Z. Jiao|Self-aware and Cross-sample Prototypical Learning for Semi-supervised Medical Image Segmentation|None|[MICCAI2023](https://arxiv.org/pdf/2305.16214.pdf)|
|2023-05|H. Cai and Y. Gao|Orthogonal Annotation Benefits Barely-supervised Medical Image Segmentation|[Code](https://github.com/HengCai-NJU/DeSCO)|[CVPR2023](https://openaccess.thecvf.com/content/CVPR2023/papers/Cai_Orthogonal_Annotation_Benefits_Barely-Supervised_Medical_Image_Segmentation_CVPR_2023_paper.pdf)|
|2023-05|H. Basak and Z. yin|Pseudo-Label Guided Contrastive Learning for Semi-Supervised Medical Image Segmentation|[Code](https://github.com/hritam-98/PatchCL-MedSeg)|[CVPR2023](https://openaccess.thecvf.com/content/CVPR2023/papers/Basak_Pseudo-Label_Guided_Contrastive_Learning_for_Semi-Supervised_Medical_Image_Segmentation_CVPR_2023_paper.pdf)|
|2023-05|Y. Wang and X. Gao|MCF: Mutual Correction Framework for Semi-Supervised Medical Image Segmentation|[Code](https://github.com/WYC-321/MCF)|[CVPR2023](https://openaccess.thecvf.com/content/CVPR2023/papers/Wang_MCF_Mutual_Correction_Framework_for_Semi-Supervised_Medical_Image_Segmentation_CVPR_2023_paper.pdf)|
|2023-05|L. Zhong and G. Wang|Semi-supervised Pathological Image Segmentation via Cross Distillation of Multiple Attentions|[Code](https://github.com/HiLab-git/CDMA)|[MICCAI2023](https://arxiv.org/pdf/2305.18830.pdf)|
|2023-05|J. Du and T. Wang|Coarse-Refined Consistency Learning using Pixel-level Features for Semi-supervised Medical Image Segmentation|None|[JBHI2023](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10131969)|
|2023-05|L. Qiu and H. Ren|Federated Semi-Supervised Learning for Medical Image Segmentation via Pseudo-Label Denoising|None|[JBHI2023](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10121665)|
## Code for semi-supervised medical image segmentation.
Some implementations of semi-supervised learning methods can be found in this [Link](https://github.com/Luoxd1996/SSL4MIS/tree/master/code).

## Social media

<p align="center"><img width="400" alt="image" src="results/wechat.png"></p> 
Welcome to follow our [Wechat official account: iBioMedInfo] and [Xiaohongshu official account: iBioMedInfo], we will share recent studies on biomedical image and bioinformation analysis there.

## Global Collaboration & Questions

**Global Collaboration:** We're on a mission to biomedical research, aiming for artificial intelligence and its applications to biomedical image and bioinformation analysis, promoting the development of the medical community. Collaborate with us to increase competitiveness.

**Questions:** General questions, please contact 'qgking@tju.edu.cn'