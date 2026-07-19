# Awesome Property-Driven Time-Series Representation Learning

**Understanding Time-Series Representations: A Property-Driven Survey**

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#contributing)

This repository accompanies the survey **Understanding Time-Series Representations: A Property-Driven Survey** by Kunpeng Xu, Soumaya Cherkaoui, Limei Lin, Chao Lin, Lifei Chen, Feng Xia, Jie Wu, and Shengrui Wang.

The survey organizes time-series representation learning (TSRL) literature from a **property-driven perspective**, emphasizing the properties learned representations should exhibit rather than primarily grouping methods by learning paradigm or architecture. It covers supervised, self-supervised, and pre-trained foundation-model approaches across forecasting, classification, anomaly detection, imputation, retrieval, clustering, segmentation, and related tasks.

The repository provides a living collection of reviewed methods, benchmarks, related surveys, and resources aligned with the survey's property-driven taxonomy: temporal fidelity, structural integrity, robustness, and transferability.

`Paper:` coming soon  |  `arXiv:` coming soon  |  `Citation:` [BibTeX](#citation)

![Conceptual overview of time-series representation learning, including data characteristics, learning paradigms, representation forms, and supported downstream tasks.](figures/fig1.png)
*Figure 1. Conceptual overview of time-series representation learning (TSRL): data characteristics, learning paradigms, representation forms, and downstream support.*

## Table of Contents

- [Property-Driven Taxonomy](#property-driven-taxonomy)
  - [Full Taxonomy Map (Figure 4)](#full-taxonomy-map-figure-4)
  - [P1: Temporal Fidelity](#p1-temporal-fidelity)
  - [P2: Structural Integrity](#p2-structural-integrity)
  - [P3: Robustness](#p3-robustness)
  - [P4: Transferability](#p4-transferability)
  - [Consolidated Taxonomy Table](#consolidated-taxonomy-table)
- [Learning Paradigms](#learning-paradigms)
- [Domain-Specific Applications](#domain-specific-applications)
- [Benchmark Datasets](#benchmark-datasets)
- [Related Surveys](#related-surveys)
- [Other Awesome Repositories](#other-awesome-repositories)
- [Repository Structure](#repository-structure)
- [Contributing](#contributing)
- [Citation](#citation)
- [License](#license)

## Property-Driven Taxonomy

The survey asks a representation-centered question: **what properties should learned time-series representations exhibit?** The resulting taxonomy groups methods by the representation properties they primarily target.

![Survey roadmap connecting the property taxonomy with learning paradigms, domain-specific applications, benchmarks, and evaluation tasks.](figures/roadmap.png)
*Figure 3. Survey roadmap.*

### Full Taxonomy Map (Figure 4)

![Representative property-driven taxonomy map of time-series representation learning methods grouped by temporal fidelity, structural integrity, robustness, and transferability.](figures/fig4.png)
*Figure 4. Representative property-driven taxonomy map.*

### P1: Temporal Fidelity
Temporal fidelity concerns short-term dependency modeling, long-term dependency modeling, and multi-scale temporal structure.

### P2: Structural Integrity
Structural integrity concerns multivariate relationships, frequency-domain structure, and decomposition-based representations.

### P3: Robustness
Robustness concerns noise and missing data, non-stationarity and concept drift, and irregular sampling.

### P4: Transferability
Transferability concerns cross-task, cross-domain, and cross-modal generalization.

### Consolidated Taxonomy Table

| Property | Sub-property | Paper | Authors | Venue/Year | Description | Links |
|---|---|---|---|---|---|---|
| P1 | P1.1 Short-term dependency modeling | Local Geometry Attention for Time Series Forecasting under Realistic Corruptions | Dongbin Kim, Youngjoo Park, Woojin Jeong, Jaewook Lee | ICLR, 2026 | Models local geometric structure while evaluating forecasting robustness under realistic corruptions. | [OpenReview](https://openreview.net/forum?id=NCQPCxN7ds) |
| P1 | P1.1 Short-term dependency modeling | A CDGFN-Based Quantum Multisource Information Fusion With Its Application in Time Series Classification | Junhao Yu, Fuyuan Xiao, Yi Zhang, Zehong Cao, Chin-Teng Lin | IEEE TKDE, 2026 | Uses quantum multisource information fusion for local time-series classification patterns. | [DOI](https://doi.org/10.1109/TKDE.2026.3652983) |
| P1 | P1.1 Short-term dependency modeling | ModernTCN: A Modern Pure Convolution Structure for General Time Series Analysis | Luo Donghao, Wang Xue | ICLR, 2024 | Revisits convolutional encoders for general time-series analysis with modern architectural choices. | [OpenReview](https://openreview.net/forum?id=vpJMJerXHU) |
| P1 | P1.1 Short-term dependency modeling | Omni-Scale CNNs: a simple and effective kernel size configuration for time series classification | Wensi Tang, Guodong Long, Lu Liu, Tianyi Zhou, et al. | ICLR, 2022 | Uses omni-scale convolutional kernels to capture discriminative local patterns for time-series classification. | [OpenReview](https://openreview.net/forum?id=PDYs7Z2XFGv) |
| P1 | P1.1 Short-term dependency modeling | An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling | Shaojie Bai, J. Zico Kolter, Vladlen Koltun | arXiv, 2018 | Establishes temporal convolutional networks as strong generic sequence encoders with dilated local receptive fields. | [arXiv](https://arxiv.org/abs/1803.01271) |
| P1 | P1.2 Long-term dependency modeling | TEDM: Time Series Forecasting with Elucidated Diffusion Models | Edgardo Solano Carrillo, Sreerag V. Naveenachandran, Julia Niebling | ICLR, 2026 | Uses diffusion modeling for long-horizon forecasting representations and denoising. | [OpenReview](https://openreview.net/forum?id=kQee8MObMc) |
| P1 | P1.2 Long-term dependency modeling | FlowPath: Learning Data-Driven Manifolds with Invertible Flows for Robust Irregularly-sampled Time Series Classification | YongKyung Oh, Dong-Young Lim, Sungil Kim | AAAI, 2026 | Learns continuous data-driven manifolds for long-range and irregular time-series representations. | [DOI](https://doi.org/10.1609/aaai.v40i29.39643) |
| P1 | P1.2 Long-term dependency modeling | Aurora: Towards Universal Generative Multimodal Time Series Forecasting | Xingjian Wu, Jianxin Jin, Wanghui Qiu, Peng Chen, et al. | ICLR, 2026 | Builds a generative multimodal foundation model for transferable long-context forecasting. | [OpenReview](https://openreview.net/forum?id=VVJ6Ck9JBl) |
| P1 | P1.2 Long-term dependency modeling | TimeDART: A Diffusion Autoregressive Transformer for Self-Supervised Time Series Representation | Daoyu Wang, Mingyue Cheng, Zhiding Liu, Qi Liu | ICML, 2025 | Combines diffusion and autoregressive Transformer objectives for long-context self-supervised representations. | [OpenReview](https://openreview.net/forum?id=v2G9HML7ep) |
| P1 | P1.2 Long-term dependency modeling | Moirai-MoE: Empowering Time Series Foundation Models with Sparse Mixture of Experts | Xu Liu, Juncheng Liu, Gerald Woo, Taha Aksu, et al. | ICML, 2025 | Uses sparse mixture-of-experts foundation modeling for long-context token-level time-series representation. | [OpenReview](https://openreview.net/forum?id=SrEOUSyJcR) |
| P1 | P1.2 Long-term dependency modeling | TrajCogn: leveraging LLMs for cognizing movement patterns and travel purposes from trajectories | Zeyu Zhou, Yan Lin, Haomin Wen, Shengnan Guo, et al. | IJCAI, 2025 | Uses LLM-based trajectory representations for mobility pattern and purpose understanding. | [DOI](https://doi.org/10.24963/ijcai.2025/411) |
| P1 | P1.2 Long-term dependency modeling | Mamba: Linear-Time Sequence Modeling with Selective State Spaces | Albert Gu, Tri Dao | arXiv, 2024 | Provides selective state-space sequence modeling for efficient long-context representation learning. | [arXiv](https://arxiv.org/abs/2312.00752) |
| P1 | P1.2 Long-term dependency modeling | A Time Series is Worth 64 Words: Long-term Forecasting with Transformers | Yuqi Nie, Nam H. Nguyen, Phanwadee Sinthong, Jayant Kalagnanam | ICLR, 2023 | Introduces patch-wise tokenization to improve Transformer efficiency and long-horizon forecasting. | [OpenReview](https://openreview.net/forum?id=Jbdc0vTOcol) |
| P1 | P1.2 Long-term dependency modeling | A Transformer-based Framework for Multivariate Time Series Representation Learning | George Zerveas, Srideepika Jayaraman, Dhaval Patel, Anuradha Bhamidipaty, et al. | KDD, 2021 | Learns global temporal representations for multivariate series with Transformer encoders. | [DOI](https://doi.org/10.1145/3447548.3467401) |
| P1 | P1.3 Multi-scale temporal structure | TimeMixer++: A General Time Series Pattern Machine for Universal Predictive Analysis | Shiyu Wang, Jiawei Li, Xiaoming Shi, Zhou Ye, et al. | ICLR, 2025 | Extends multi-scale pattern mixing with frequency and decomposition views for universal predictive analysis. | [OpenReview](https://openreview.net/forum?id=1CLzLXSFNn) |
| P1 | P1.3 Multi-scale temporal structure | HDMixer: Hierarchical Dependency with Extendable Patch for Multivariate Time Series Forecasting | Qihe Huang, Lei Shen, Ruixin Zhang, Jiahuan Cheng, et al. | AAAI, 2024 | Combines extendable patches and hierarchical mixing to capture short-term, long-term, and cross-variable dependencies. | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/29155) |
| P1 | P1.3 Multi-scale temporal structure | TimeMixer: Decomposable Multiscale Mixing for Time Series Forecasting | Shiyu Wang, Haixu Wu, Xiaoming Shi, Tengge Hu, et al. | ICLR, 2024 | Mixes temporal patterns across decomposed scales for long- and short-term forecasting. | [OpenReview](https://openreview.net/forum?id=7oLshfEIC2) |
| P1 | P1.3 Multi-scale temporal structure | TimesNet: Temporal 2D-Variation Modeling for General Time Series Analysis | Haixu Wu, Tengge Hu, Yong Liu, Hang Zhou, et al. | ICLR, 2023 | Models multi-period temporal variation by transforming one-dimensional series into two-dimensional temporal representations. | [OpenReview](https://openreview.net/forum?id=ju_Uqw384Oq) |
| P2 | P2.1 Multivariate relationships | Low Rank Transformer for Multivariate Time Series Anomaly Detection and Localization | Charalampos Shimillas, Kleanthis Malialis, Konstantinos Fokianos, Marios Polycarpou | ICLR, 2026 | Models multivariate anomaly structure with low-rank Transformer representations. | [OpenReview](https://openreview.net/forum?id=ZtPIBpVojC) |
| P2 | P2.1 Multivariate relationships | CoRA: Boosting Time Series Foundation Models for Multivariate Forecasting through Correlation-aware Adapter | Hanyin Cheng, Xingjian Wu, Yang Shu, Zhongwen Rao, et al. | ICLR, 2026 | Adds correlation-aware adapters to strengthen multivariate foundation-model representations. | [OpenReview](https://openreview.net/forum?id=JRlNrcTllN) |
| P2 | P2.1 Multivariate relationships | DUET: Dual Clustering Enhanced Multivariate Time Series Forecasting | Xiangfei Qiu, Xingjian Wu, Yan Lin, Chenjuan Guo, et al. | KDD, 2025 | Uses dual clustering to capture multivariate temporal structure for forecasting. | [DOI](https://doi.org/10.1145/3690624.3709325) |
| P2 | P2.1 Multivariate relationships | FreEformer: frequency enhanced transformer for multivariate time series forecasting | Wenzhen Yue, Yong Liu, Xianghua Ying, Bowei Xing, et al. | IJCAI, 2025 | Combines multivariate forecasting with frequency-enhanced Transformer representations. | [DOI](https://doi.org/10.24963/ijcai.2025/401) |
| P2 | P2.1 Multivariate relationships | Causality-Aware Contrastive Learning for Robust Multivariate Time-Series Anomaly Detection | HyunGi Kim, Jisoo Mok, Dongjun Lee, Jaihyun Lew, et al. | ICML, 2025 | Learns causal multivariate representations for robust time-series anomaly detection. | [OpenReview](https://openreview.net/forum?id=EGpueKe6TP) |
| P2 | P2.1 Multivariate relationships | AdaPTS: Adapting Univariate Foundation Models to Probabilistic Multivariate Time Series Forecasting | Abdelhakim Benechehab, Vasilii Feofanov, Giuseppe Paolo, Albert Thomas, et al. | ICML, 2025 | Adapts univariate foundation models to probabilistic multivariate forecasting. | [OpenReview](https://openreview.net/forum?id=yeICCRy3lE) |
| P2 | P2.1 Multivariate relationships | Moirai-MoE: Empowering Time Series Foundation Models with Sparse Mixture of Experts | Xu Liu, Juncheng Liu, Gerald Woo, Taha Aksu, et al. | ICML, 2025 | Uses mixture-of-experts routing to support multivariate foundation-model representations. | [OpenReview](https://openreview.net/forum?id=SrEOUSyJcR) |
| P2 | P2.1 Multivariate relationships | TrajCogn: leveraging LLMs for cognizing movement patterns and travel purposes from trajectories | Zeyu Zhou, Yan Lin, Haomin Wen, Shengnan Guo, et al. | IJCAI, 2025 | Models structural relationships in urban trajectory representations. | [DOI](https://doi.org/10.24963/ijcai.2025/411) |
| P2 | P2.1 Multivariate relationships | MSGNet: Learning Multi-Scale Inter-series Correlations for Multivariate Time Series Forecasting | Wanlin Cai, Yuxuan Liang, Xianggen Liu, Jianshuai Feng, Yuankai Wu | AAAI, 2024 | Uses frequency analysis and adaptive graph convolution to learn inter-series correlations across scales. | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/28991) |
| P2 | P2.1 Multivariate relationships | Fully-Connected Spatial-Temporal Graph for Multivariate Time-Series Data | Yucheng Wang, Yuecong Xu, Jianfei Yang, Min Wu, et al. | AAAI, 2024 | Constructs fully connected spatial-temporal graphs to capture dependencies between sensors and timestamps. | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/29500) |
| P2 | P2.1 Multivariate relationships | Crossformer: Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting | Yunhao Zhang, Junchi Yan | ICLR, 2023 | Uses two-stage attention to model cross-dimension dependencies in multivariate forecasting. | [OpenReview](https://openreview.net/forum?id=vSVLM2j9eie) |
| P2 | P2.2 Frequency-domain structure | TSPulse: Tiny Pre-Trained Models with Disentangled Representations for Rapid Time-Series Analysis | Vijay Ekambaram, Subodh Kumar, Arindam Jati, Sumanta Mukherjee, et al. | ICLR, 2026 | Learns compact disentangled representations with frequency-related structure for rapid analysis. | [OpenReview](https://openreview.net/forum?id=Kw2mvnzCoc) |
| P2 | P2.2 Frequency-domain structure | FreEformer: frequency enhanced transformer for multivariate time series forecasting | Wenzhen Yue, Yong Liu, Xianghua Ying, Bowei Xing, et al. | IJCAI, 2025 | Uses frequency enhancement to improve multivariate time-series forecasting representations. | [DOI](https://doi.org/10.24963/ijcai.2025/401) |
| P2 | P2.2 Frequency-domain structure | TimeMixer++: A General Time Series Pattern Machine for Universal Predictive Analysis | Shiyu Wang, Jiawei Li, Xiaoming Shi, Zhou Ye, et al. | ICLR, 2025 | Incorporates frequency-domain views into general multi-scale predictive representations. | [OpenReview](https://openreview.net/forum?id=1CLzLXSFNn) |
| P2 | P2.2 Frequency-domain structure | FITS: Modeling Time Series with $10k$ Parameters | Zhijian Xu, Ailing Zeng, Qiang Xu | ICLR, 2024 | Uses lightweight frequency interpolation for efficient time-series forecasting. | [OpenReview](https://openreview.net/forum?id=bWcnvZ3qMb) |
| P2 | P2.2 Frequency-domain structure | Self-Supervised Contrastive Pre-Training For Time Series via Time-Frequency Consistency | Xiang Zhang, Ziyuan Zhao, Theodoros Tsiligkaridis, Marinka Zitnik | NeurIPS, 2022 | Aligns time-domain and frequency-domain views for self-supervised time-series representation learning. | [OpenReview](https://openreview.net/forum?id=OJ4mMfGKLN) |
| P2 | P2.2 Frequency-domain structure | FEDformer: Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting | Tian Zhou, Ziqing Ma, Qingsong Wen, Xue Wang, et al. | ICML, 2022 | Combines decomposition with frequency-enhanced attention for long-term seasonal forecasting. | [PMLR](https://proceedings.mlr.press/v162/zhou22g.html) |
| P2 | P2.3 Decomposition-based representations | TimeMixer++: A General Time Series Pattern Machine for Universal Predictive Analysis | Shiyu Wang, Jiawei Li, Xiaoming Shi, Zhou Ye, et al. | ICLR, 2025 | Combines universal pattern modeling with decomposition-based time-series representations. | [OpenReview](https://openreview.net/forum?id=1CLzLXSFNn) |
| P2 | P2.3 Decomposition-based representations | TimeMixer: Decomposable Multiscale Mixing for Time Series Forecasting | Shiyu Wang, Haixu Wu, Xiaoming Shi, Tengge Hu, et al. | ICLR, 2024 | Mixes decomposed temporal patterns across scales for forecasting. | [OpenReview](https://openreview.net/forum?id=7oLshfEIC2) |
| P2 | P2.3 Decomposition-based representations | Are Transformers Effective for Time Series Forecasting? | Ailing Zeng, Muxi Chen, Lei Zhang, Qiang Xu | AAAI, 2023 | Introduces simple linear decomposition baselines that challenge complex Transformer forecasting models. | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/26317) |
| P2 | P2.3 Decomposition-based representations | A Shapelet-Based Framework for Unsupervised Multivariate Time Series Representation Learning | Zhiyu Liang, Jianfeng Zhang, Chen Liang, Hongzhi Wang, et al. | PVLDB, 2023 | Learns interpretable shapelet-based representations for unsupervised multivariate time-series analysis. | [DOI](https://doi.org/10.14778/3632093.3632103) |
| P2 | P2.3 Decomposition-based representations | Autoformer: Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting | Haixu Wu, Jiehui Xu, Jianmin Wang, Mingsheng Long | NeurIPS, 2021 | Embeds series decomposition and auto-correlation mechanisms into Transformer forecasting. | [OpenReview](https://openreview.net/forum?id=J4gRj6d5Qm) |
| P3 | P3.1 Noise and missing data | Local Geometry Attention for Time Series Forecasting under Realistic Corruptions | Dongbin Kim, Youngjoo Park, Woojin Jeong, Jaewook Lee | ICLR, 2026 | Evaluates and improves forecasting representations under realistic corruptions. | [OpenReview](https://openreview.net/forum?id=NCQPCxN7ds) |
| P3 | P3.1 Noise and missing data | TEDM: Time Series Forecasting with Elucidated Diffusion Models | Edgardo Solano Carrillo, Sreerag V. Naveenachandran, Julia Niebling | ICLR, 2026 | Learns denoising-oriented forecasting representations through elucidated diffusion models. | [OpenReview](https://openreview.net/forum?id=kQee8MObMc) |
| P3 | P3.1 Noise and missing data | Low Rank Transformer for Multivariate Time Series Anomaly Detection and Localization | Charalampos Shimillas, Kleanthis Malialis, Konstantinos Fokianos, Marios Polycarpou | ICLR, 2026 | Targets robust multivariate anomaly detection and localization under noisy observations. | [OpenReview](https://openreview.net/forum?id=ZtPIBpVojC) |
| P3 | P3.1 Noise and missing data | FlowPath: Learning Data-Driven Manifolds with Invertible Flows for Robust Irregularly-sampled Time Series Classification | YongKyung Oh, Dong-Young Lim, Sungil Kim | AAAI, 2026 | Learns robust manifold representations for corrupted and irregularly sampled time series. | [DOI](https://doi.org/10.1609/aaai.v40i29.39643) |
| P3 | P3.1 Noise and missing data | Causality-Aware Contrastive Learning for Robust Multivariate Time-Series Anomaly Detection | HyunGi Kim, Jisoo Mok, Dongjun Lee, Jaihyun Lew, et al. | ICML, 2025 | Uses causality-aware contrastive learning to improve robustness in anomaly detection. | [OpenReview](https://openreview.net/forum?id=EGpueKe6TP) |
| P3 | P3.1 Noise and missing data | TimeDART: A Diffusion Autoregressive Transformer for Self-Supervised Time Series Representation | Daoyu Wang, Mingyue Cheng, Zhiding Liu, Qi Liu | ICML, 2025 | Uses diffusion denoising and autoregressive modeling for noisy time-series representation learning. | [OpenReview](https://openreview.net/forum?id=v2G9HML7ep) |
| P3 | P3.1 Noise and missing data | Applying quantum autoencoders for time series anomaly detection | Robin Frehner, Kurt Stockinger | Quantum Machine Intelligence, 2025 | Applies quantum autoencoders to anomaly-detection representations under reconstruction noise. | [DOI](https://doi.org/10.1007/s42484-025-00285-1) |
| P3 | P3.1 Noise and missing data | Self-Supervised Learning of Time Series Representation via Diffusion Process and Imputation-Interpolation-Forecasting Mask | Zineb Senane, Lele Cao, Valentin Leonhard Buchner, Yusuke Tashiro, et al. | KDD, 2024 | Learns robust representations through diffusion-based masking for imputation, interpolation, and forecasting. | [DOI](https://doi.org/10.1145/3637528.3671673) |
| P3 | P3.1 Noise and missing data | SimMTM: A Simple Pre-Training Framework for Masked Time-Series Modeling | Jiaxiang Dong, Haixu Wu, Haoran Zhang, Li Zhang, et al. | NeurIPS, 2023 | Uses masked time-series modeling to learn representations robust to missing segments. | [OpenReview](https://openreview.net/forum?id=ginTcBUnL8) |
| P3 | P3.2 Non-stationarity and concept drift | Dish-TS: A General Paradigm for Alleviating Distribution Shift in Time Series Forecasting | Wei Fan, Pengyang Wang, Dongkun Wang, Dongjie Wang, et al. | AAAI, 2023 | Models input- and output-space distribution shifts with learnable distribution coefficients. | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/25914) |
| P3 | P3.2 Non-stationarity and concept drift | Non-stationary Transformers: Exploring the Stationarity in Time Series Forecasting | Yong Liu, Haixu Wu, Jianmin Wang, Mingsheng Long | NeurIPS, 2022 | Introduces de-stationary attention to handle non-stationary temporal distributions. | [OpenReview](https://openreview.net/forum?id=ucNDIDRNjjv) |
| P3 | P3.2 Non-stationarity and concept drift | Reversible Instance Normalization for Accurate Time-Series Forecasting against Distribution Shift | Taesung Kim, Jinhee Kim, Yunwon Tae, Cheonbok Park, et al. | ICLR, 2022 | Normalizes each instance reversibly to mitigate distribution shift in forecasting. | [OpenReview](https://openreview.net/forum?id=cGDAkQo1C0p) |
| P3 | P3.3 Irregular sampling | FlowPath: Learning Data-Driven Manifolds with Invertible Flows for Robust Irregularly-sampled Time Series Classification | YongKyung Oh, Dong-Young Lim, Sungil Kim | AAAI, 2026 | Handles irregularly sampled series with invertible-flow manifold representations. | [DOI](https://doi.org/10.1609/aaai.v40i29.39643) |
| P3 | P3.3 Irregular sampling | ContiFormer: Continuous-Time Transformer for Irregular Time Series Modeling | Yuqi Chen, Kan Ren, Yansen Wang, Yuchen Fang, et al. | NeurIPS, 2023 | Combines continuous-time dynamics with Transformer modeling for irregularly sampled series. | [OpenReview](https://openreview.net/forum?id=YJDz4F2AZu) |
| P3 | P3.3 Irregular sampling | Multi-Time Attention Networks for Irregularly Sampled Time Series | Satya Narayan Shukla, Benjamin Marlin | ICLR, 2021 | Uses continuous attention mechanisms to handle variable observation times. | [OpenReview](https://openreview.net/forum?id=4c0J6lwQ4_) |
| P3 | P3.3 Irregular sampling | Latent Ordinary Differential Equations for Irregularly-Sampled Time Series | Yulia Rubanova, Ricky T. Q. Chen, David K. Duvenaud | NeurIPS, 2019 | Learns continuous-time latent dynamics for interpolation and extrapolation from irregular observations. | [PDF](https://proceedings.neurips.cc/paper_files/paper/2019/file/42a6845a557bef704ad8ac9cb4461d43-Paper.pdf) |
| P4 | P4.1 Cross-task generalization | TSPulse: Tiny Pre-Trained Models with Disentangled Representations for Rapid Time-Series Analysis | Vijay Ekambaram, Subodh Kumar, Arindam Jati, Sumanta Mukherjee, et al. | ICLR, 2026 | Provides compact pre-trained representations for rapid multi-task time-series analysis. | [OpenReview](https://openreview.net/forum?id=Kw2mvnzCoc) |
| P4 | P4.1 Cross-task generalization | Aurora: Towards Universal Generative Multimodal Time Series Forecasting | Xingjian Wu, Jianxin Jin, Wanghui Qiu, Peng Chen, et al. | ICLR, 2026 | Supports universal generative forecasting across tasks and modalities. | [OpenReview](https://openreview.net/forum?id=VVJ6Ck9JBl) |
| P4 | P4.1 Cross-task generalization | CoRA: Boosting Time Series Foundation Models for Multivariate Forecasting through Correlation-aware Adapter | Hanyin Cheng, Xingjian Wu, Yang Shu, Zhongwen Rao, et al. | ICLR, 2026 | Adapts foundation models for multivariate forecasting through correlation-aware transfer. | [OpenReview](https://openreview.net/forum?id=JRlNrcTllN) |
| P4 | P4.1 Cross-task generalization | Repurposing Foundation Model for Generalizable Medical Time Series Classification | Nan Huang, Haishuai Wang, Zihuai He, Marinka Zitnik, Xiang Zhang | ICLR, 2026 | Repurposes foundation models for generalizable medical time-series classification. | [OpenReview](https://openreview.net/forum?id=wNEzRYiyZM) |
| P4 | P4.1 Cross-task generalization | TimeMixer++: A General Time Series Pattern Machine for Universal Predictive Analysis | Shiyu Wang, Jiawei Li, Xiaoming Shi, Zhou Ye, et al. | ICLR, 2025 | Supports multi-task predictive analysis through general time-series pattern representations. | [OpenReview](https://openreview.net/forum?id=1CLzLXSFNn) |
| P4 | P4.1 Cross-task generalization | AdaPTS: Adapting Univariate Foundation Models to Probabilistic Multivariate Time Series Forecasting | Abdelhakim Benechehab, Vasilii Feofanov, Giuseppe Paolo, Albert Thomas, et al. | ICML, 2025 | Adapts foundation representations for probabilistic multivariate forecasting. | [OpenReview](https://openreview.net/forum?id=yeICCRy3lE) |
| P4 | P4.1 Cross-task generalization | In-Context Fine-Tuning for Time-Series Foundation Models | Matthew Faw, Rajat Sen, Yichen Zhou, Abhimanyu Das | ICML, 2025 | Studies efficient in-context adaptation for time-series foundation models. | [OpenReview](https://openreview.net/forum?id=uxzgGLWPj2) |
| P4 | P4.1 Cross-task generalization | Moirai-MoE: Empowering Time Series Foundation Models with Sparse Mixture of Experts | Xu Liu, Juncheng Liu, Gerald Woo, Taha Aksu, et al. | ICML, 2025 | Expands time-series foundation models with sparse expert routing for transfer across tasks. | [OpenReview](https://openreview.net/forum?id=SrEOUSyJcR) |
| P4 | P4.1 Cross-task generalization | MOMENT: A Family of Open Time-series Foundation Models | Mononito Goswami, Konrad Szafer, Arjun Choudhry, Yifu Cai, et al. | ICML, 2024 | Provides open foundation models for multi-task time-series representation learning. | [OpenReview](https://openreview.net/forum?id=FVvf69a5rx) |
| P4 | P4.1 Cross-task generalization | A decoder-only foundation model for time-series forecasting | Abhimanyu Das, Weihao Kong, Rajat Sen, Yichen Zhou | ICML, 2024 | Introduces TimesFM for zero-shot and transfer forecasting with a decoder-only foundation model. | [PMLR](https://proceedings.mlr.press/v235/das24c.html) |
| P4 | P4.1 Cross-task generalization | Chronos: Learning the Language of Time Series | Abdul Fatir Ansari, Lorenzo Stella, Ali Caner Turkmen, Xiyuan Zhang, et al. | TMLR, 2024 | Tokenizes time series and trains language-model-style forecasters for probabilistic zero-shot prediction. | [OpenReview](https://openreview.net/forum?id=gerNCVqqtR) |
| P4 | P4.2 Cross-domain adaptation | Repurposing Foundation Model for Generalizable Medical Time Series Classification | Nan Huang, Haishuai Wang, Zihuai He, Marinka Zitnik, Xiang Zhang | ICLR, 2026 | Adapts foundation representations across medical time-series datasets and domains. | [OpenReview](https://openreview.net/forum?id=wNEzRYiyZM) |
| P4 | P4.2 Cross-domain adaptation | ClimaX: A foundation model for weather and climate | Tung Nguyen, Johannes Brandstetter, Ashish Kapoor, Jayesh K. Gupta, et al. | ICML, 2023 | Pre-trains a weather and climate foundation model for adaptation across atmospheric tasks and datasets. | [PMLR](https://proceedings.mlr.press/v202/nguyen23a.html) |
| P4 | P4.2 Cross-domain adaptation | Prompt federated learning for weather forecasting: toward foundation models on meteorological data | Shengchao Chen, Guodong Long, Tao Shen, Jing Jiang | IJCAI, 2023 | Uses federated prompt learning for privacy-preserving weather forecasting across heterogeneous regions. | [DOI](https://doi.org/10.24963/ijcai.2023/393) |
| P4 | P4.2 Cross-domain adaptation | Self-Supervised Pre-training for Time Series Classification | Pengxiang Shi, Wenwen Ye, Zheng Qin | IJCNN, 2021 | Studies self-supervised pre-training and fine-tuning for cross-domain time-series classification. | [DOI](https://doi.org/10.1109/IJCNN52387.2021.9533426) |
| P4 | P4.3 Cross-modal fusion | Aurora: Towards Universal Generative Multimodal Time Series Forecasting | Xingjian Wu, Jianxin Jin, Wanghui Qiu, Peng Chen, et al. | ICLR, 2026 | Uses multimodal generative modeling for cross-modal time-series forecasting. | [OpenReview](https://openreview.net/forum?id=VVJ6Ck9JBl) |
| P4 | P4.3 Cross-modal fusion | TimeCMA: Towards LLM-Empowered Multivariate Time Series Forecasting via Cross-Modality Alignment | Chenxi Liu, Qianxiong Xu, Hao Miao, Sun Yang, et al. | AAAI, 2025 | Aligns time-series and language-model spaces for cross-modal forecasting. | [DOI](https://doi.org/10.1609/aaai.v39i18.34067) |
| P4 | P4.3 Cross-modal fusion | MM-Path: Multi-modal, Multi-granularity Path Representation Learning | Ronghui Xu, Hanyin Cheng, Chenjuan Guo, Hongfan Gao, et al. | KDD, 2025 | Learns multi-modal, multi-granularity representations for path and mobility data. | [DOI](https://doi.org/10.1145/3690624.3709209) |
| P4 | P4.3 Cross-modal fusion | TrajCogn: leveraging LLMs for cognizing movement patterns and travel purposes from trajectories | Zeyu Zhou, Yan Lin, Haomin Wen, Shengnan Guo, et al. | IJCAI, 2025 | Fuses trajectory signals with LLM representations for mobility analytics. | [DOI](https://doi.org/10.24963/ijcai.2025/411) |
| P4 | P4.3 Cross-modal fusion | Time-LLM: Time Series Forecasting by Reprogramming Large Language Models | Ming Jin, Shiyu Wang, Lintao Ma, Zhixuan Chu, et al. | ICLR, 2024 | Reprograms large language models for time-series forecasting through cross-modal alignment. | [OpenReview](https://openreview.net/forum?id=Unb5CVPtae) |
| P4 | P4.3 Cross-modal fusion | GPT4MTS: Prompt-based Large Language Model for Multimodal Time-series Forecasting | Furong Jia, Kevin Wang, Yixiang Zheng, Defu Cao, Yan Liu | AAAI, 2024 | Fuses numerical time series with textual context for multimodal forecasting. | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/30383) |
| P4 | P4.3 Cross-modal fusion | Large Language Models Are Zero-Shot Time Series Forecasters | Nate Gruver, Marc Anton Finzi, Shikai Qiu, Andrew Gordon Wilson | NeurIPS, 2023 | Casts numerical time series as text to enable zero-shot forecasting with language models. | [OpenReview](https://openreview.net/forum?id=md68e8iZK1) |

## Learning Paradigms

| Paradigm | Representative methods from the survey | Notes |
|---|---|---|
| Fully supervised methods | TCN, OS-CNN, TST, PatchTST, TimesNet, Crossformer, Autoformer | Optimized directly for labeled downstream tasks such as forecasting or classification. |
| Self-supervised methods | TS-TCC, TF-C, SimMTM, TSDE, TimesURL, CSL, SSP-TSC | Learn reusable encoders through masking, contrastive objectives, reconstruction, diffusion, or pretext tasks. |
| Pre-trained foundation models | MOMENT, TimesFM, Chronos, Timer, UniTS, Moirai, Time-LLM | Scale pre-training across datasets and support zero-shot, few-shot, prompting, or fine-tuning workflows. |

## Domain-Specific Applications

| Domain | Representative references | Property emphasis |
|---|---|---|
| Healthcare | PhysioNet/CinC Challenge 2017; STraTS; COMET; GRU-D | Robustness to missingness and irregular sampling, plus multivariate clinical structure. |
| Finance | AI in Finance; regime-shift and non-stationarity methods such as RevIN and Dish-TS | Non-stationarity, high-frequency noise, and transfer across market regimes. |
| Climate and Environment | Pangu-Weather; FourCastNet; ClimaX; MetePFL | Long-range spatiotemporal dependency, physical structure, and cross-region adaptation. |
| Urban and Transportation | DCRNN; UrbanGPT; UniST; TrajCogn | Spatiotemporal graph structure, heterogeneous context, and cross-modal mobility signals. |

## Benchmark Datasets

| Task | Datasets |
|---|---|
| Forecasting | ETT, Weather, Electricity (ECL), Traffic, M4 |
| Classification | UCR Archive, UEA Archive, UCI HAR, PhysioNet 2012 |
| Anomaly Detection | SMD, MSL/SMAP, SWaT, TSB-UAD |
| Imputation | PhysioNet 2019, ETT/Weather with simulated missingness |
| Segmentation | TSSB, UTSA |
| Foundation-model evaluation | GIFT-Eval, Monash forecasting archive |

## Related Surveys

| Survey | Authors | Venue/Year | Link |
|---|---|---|---|
| Representation Learning: A Review and New Perspectives | Yoshua Bengio, Aaron Courville, Pascal Vincent | IEEE TPAMI, 2013 | [DOI](https://doi.org/10.1109/TPAMI.2013.50) |
| A review of unsupervised feature learning and deep learning for time-series modeling | Martin Langkvist, Lars Karlsson, Amy Loutfi | Pattern Recognition Letters, 2014 | [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0167865514000221) |
| Self-Supervised Learning for Time Series Analysis: Taxonomy, Progress, and Prospects | Kexin Zhang, Qingsong Wen, Chaoli Zhang, Rongyao Cai, et al. | IEEE TPAMI, 2024 | [DOI](https://doi.org/10.1109/TPAMI.2024.3387317) |
| Foundation Models for Time Series Analysis: A Tutorial and Survey | Yuxuan Liang, Haomin Wen, Yuqi Nie, Yushan Jiang, et al. | KDD, 2024 | [DOI](https://doi.org/10.1145/3637528.3671451) |
| Universal Time-Series Representation Learning: A Survey | Patara Trirat, Yooju Shin, Junhyeok Kang, Youngeun Nam, et al. | arXiv, 2024 | [arXiv](https://arxiv.org/abs/2401.03717) |
| Transformers in time series: a survey | Qingsong Wen, Tian Zhou, Chaoli Zhang, Weiqi Chen, et al. | IJCAI, 2023 | [DOI](https://doi.org/10.24963/ijcai.2023/759) |

## Other Awesome Repositories

- [awesome-deep-time-series-representations](https://github.com/itouchz/awesome-deep-time-series-representations) - A broad awesome list for deep time-series representation learning.
- Add related repositories through pull requests, especially resources that align with the property-driven taxonomy.

## Repository Structure

```text
.
|-- README.md
`-- figures/
    |-- fig1.png
    |-- fig4.png
    `-- roadmap.png
```

## Contributing

This repository is a living resource and may be updated as new TSRL methods, benchmarks, and related surveys appear.

Contributions are welcome. Please open an issue or pull request for missing papers, incorrect metadata, broken links, or taxonomy suggestions. Proposed additions should fit the property-driven taxonomy and preserve official paper titles, author lists, venues, and links.

When adding a paper, please include:

- Paper title, authors, venue, and year.
- A stable link such as DOI, arXiv, OpenReview, project page, or GitHub repository.
- The most relevant property category and subcategory.
- A concise one-line description.

## Citation

If this survey or repository is useful for your research, please cite:

```bibtex
@misc{xu2026understanding,
  title  = {Understanding Time-Series Representations: A Property-Driven Survey},
  author = {Xu, Kunpeng and Cherkaoui, Soumaya and Lin, Limei and
            Lin, Chao and Chen, Lifei and Xia, Feng and Wu, Jie and
            Wang, Shengrui},
  year   = {2026}
}
```

## License

License information is currently TBD. Please update this section once the repository license is finalized.
