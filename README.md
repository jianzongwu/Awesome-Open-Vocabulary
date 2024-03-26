[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](https://github.com/jianzongwu/Awesome-Open-Vocabulary/pulls)
<br />
<p align="center">
  <h1 align="center">Towards Open Vocabulary Learning: A Survey</h1>
  <p align="center">
    <b> T-PAMI, 2024 </b>
    <br />
    <a href="https://jianzongwu.github.io/"><strong>Jianzong Wu <sup>*</sup></strong></a>
    .
    <a href="https://lxtgh.github.io/"><strong> Xiangtai Li <sup>*</sup> </strong></a>
    ·
    <a href="https://xushilin1.github.io/"><strong>Shilin Xu  <sup>*</sup></strong></a>
    ·
    <a href="https://yuanhaobo.me/"><strong>Haobo Yuan  <sup>*</sup></strong></a>
    ·
    <a href="https://henghuiding.github.io/"><strong>Henghui Ding</strong></a>
    ·
    <a href="https://iboing.github.io/"><strong>Yibo Yang</strong></a>
    ·
    <a href="https://xialipku.github.io/"><strong>Xia Li</strong></a>
    ·
    <a href="https://zhangzjn.github.io/"><strong>Jiangning Zhang</strong></a>
    ·
    <a href="https://scholar.google.com/citations?user=T4gqdPkAAAAJ&hl=zh-CN"><strong>Yunhai Tong</strong></a>
    ·
    <a href="http://scholar.google.com/citations?user=IL3mSioAAAAJ&hl=zh-CN"><strong>Xudong Jiang</strong></a>
    ·
    <a href="https://scholar.google.com/citations?user=rVsGTeEAAAAJ&hl=zh-CN"><strong>Bernard Ghanem</strong></a>
    ·
    <a href="https://scholar.google.com/citations?user=RwlJNLcAAAAJ&hl=zh-CN"><strong>Dacheng Tao</strong></a>
    ·
  </p>

  <p align="center">
    <a href='https://arxiv.org/abs/2306.15880'>
      <img src='https://img.shields.io/badge/arXiv-PDF-green?style=flat&logo=arXiv&logoColor=green' alt='arXiv PDF'>
    </a>
    <a href='https://ieeexplore.ieee.org/document/10420487'>
      <img src='https://img.shields.io/badge/TPAMI-PDF-blue?style=flat&logo=IEEE&logoColor=green' alt='TPAMI PDF'>
    </a>
  </p>
<br />

This repo is used for recording, tracking, and benchmarking several recent open vocabulary methods to supplement our [survey](https://arxiv.org/abs/2306.15880).  
If you find any work missing or have any suggestions (papers, implementations, and other resources), feel free to [pull requests](https://github.com/jianzongwu/Awesome-Open-Vocabulary/pulls).
We will add the missing papers to this repo as soon as possible.

### 🔥Add Your Paper in our Repo and Survey!!!!!

[-] You are welcome to give us an issue or PR for your open vocabulary learning work !!!!!

[-] Note that: Due to the huge paper in Arxiv, we are sorry to cover all in our survey. You can directly present a PR into this repo and we will record it for next version update of our survey.

[-] **Our survey will be updated in 2024.3.**


### 🔥New

[-] Our work is accepted by T-PAMI !!! 🔥🔥🔥

[-] We update GitHub to record the available paper by the end of **2024/1/10**.

[-] We update GitHub to record the available paper by the end of **2023/7/20**.


### 🔥Highlight!!

[1]  The first survey for open vocabulary learning, including open vocabulary detection/segmentation/tracking.

[2]  It also contains several related domains, including foundation model tuning and open-world detection. 

[3]  We list detailed results for the most representative works and give a fairer and clearer comparison of different approaches.



## Introduction

This survey presents the first detailed survey on open vocabulary tasks, including open-vocabulary object detection, open-vocabulary segmentation, and 3D/video open-vocabulary tasks.

![Alt Text](figs/timeline.jpg)

## Summary of Contents

- [Introduction](#introduction)
- [Summary of Contents](#summary-of-contents)
- [Methods: A Survey](#methods-a-survey)
  - [Open Vocabulary Object Detection](#open-vocabulary-object-detection)
  - [Open Vocabulary Segmentation](#open-vocabulary-segmentation)
    - [Semantic Segmentation](#semantic-segmentation)
    - [Instance Segmentation](#instance-segmentation)
    - [Panoptic Segmentation](#panoptic-segmentation)
  - [Open Vocabulary Video Understanding](#open-vocabulary-video-understanding)
    - [Video Classification](#video-classification)
    - [Tracking](#tracking)
    - [Video Instance Segmentation](#video-instance-segmentation)
  - [Open Vocabulary 3D Scene Understanding](#open-vocabulary-3d-scene-understanding)
    - [3D Classification](#3d-classification)
    - [3D Detection](#3d-detection)
    - [3D segmentation](#3d-segmentation)
- [Related Domains and Beyond](#related-domains-and-beyond)
  - [Class-agnostic Detection and Segmentation](#class-agnostic-detection-and-segmentation)
  - [Open-World Object Detection](#open-world-object-detection)
  - [Open-Set Panoptic Segmentation](#open-set-panoptic-segmentation)
- [Acknowledgement](#acknowledgement)
- [Contact](#contact)

## Methods: A Survey

**Keywords**

- `cap.`: Use caption as auxiliary training data
- `vlm.`: Use pretrained VLMs like CLIP 
- `pl.`: Generate pseudo labels
- `w/o ps.`: Training without pixel-level supervision
- `pre.`: Vision-language pretraining
- `diff.`: Use diffusion models
- `unify`: Unify several tasks (semantic segmentation, instance segmentation, and panoptic segmentation)
- `sam`: Use SAM (Segment Anything Model)
- `open.`: Demonstrated with open-set capability. (only for Video Understanding)
- `audio.`: With audio modality.
- `bench`: Propose a benchmark.
- `other`: Other methods that cannot be grouped into above ones.
- `no-train`: Does not need training.

### Open Vocabulary Object Detection

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2021|CVPR|`cap.`|[Open-Vocabulary Object Detection Using Captions](https://arxiv.org/abs/2011.10678)|[Code](https://github.com/alirezazareian/ovr-cnn)|
|2022|ICLR|`vlm.`|[Open-vocabulary Object Detection via Vision and Language Knowledge Distillation](https://arxiv.org/abs/2104.13921)|[Code](https://github.com/tensorflow/tpu/tree/master/models/official/detection/projects/vild)|
|2022|CVPR|`cap.`, `vlm.`, `pre.`|[RegionCLIP: Region-based Language-Image Pretraining](https://arxiv.org/abs/2112.09106)|[Code](https://github.com/microsoft/RegionCLIP)|
|2022|CVPR|`vlm.`|[Learning to Prompt for Open-Vocabulary Object Detection with Vision-Language Model](https://arxiv.org/abs/2203.14940)|[Code](https://github.com/dyabel/detpro)|
|2022|CVPR|`vlm.`, `cap.`|[Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation](https://arxiv.org/abs/2203.10593)|[Code](https://github.com/mengqiDyangge/HierKD)|
|2022|CVPR|`cap.`, `vlm.`|[Grounded Language-Image Pre-training](https://arxiv.org/pdf/2112.03857.pdf)|[[Code](https://github.com/microsoft/GLIP)]|
|2022|NeurIPS|`cap.`, `vlm.`|[GLIPv2: Unifying Localization and VL Understanding](https://arxiv.org/pdf/2206.05836.pdf)|[Code](https://github.com/microsoft/GLIP)|
|2022|GCPR|`cap.`|[Localized Vision-Language Matching for Open-vocabulary Object Detection](https://arxiv.org/abs/2205.06160)|[Code](https://github.com/lmb-freiburg/locov)|
|2022|ECCV|`vlm.`|[Open-Vocabulary DETR with Conditional Matching](https://arxiv.org/abs/2203.11876)|[Code](https://github.com/yuhangzang/OV-DETR)|
|2022|ECCV|`vlm.`, `cap.`, `pl.`|[Open Vocabulary Object Detection with Pseudo Bounding-Box Labels](https://arxiv.org/abs/2111.09452)|[Code](https://github.com/salesforce/PB-OVD)|
|2022|ECCV|`vlm.`|[Promptdet: Towards open-vocabulary detection using uncurated images](https://arxiv.org/abs/2203.16513)|[Code](https://github.com/fcjian/PromptDet)|
|2022|ECCV|`vlm.`, `pl.`, `w/o ps.`|[Detecting Twenty-thousand Classes using Image-level Supervision](https://arxiv.org/abs/2201.02605)|[Code](https://github.com/facebookresearch/Detic)|
|2022|ECCV|`vlm.`. `pl.`|[Exploiting unlabeled data with vision and language models for object detection](https://arxiv.org/abs/2207.08954)|[Code](https://github.com/xiaofeng94/VL-PLM)|
|2022|ECCV|`vlm.`, `cap.`|[Simple Open-Vocabulary Object Detection with Vision Transformers](https://arxiv.org/abs/2205.06230)|[Code](https://github.com/google-research/scenic/tree/main/scenic/projects/owl_vit)|
|2022|NeurIPS|`vlm.`, `pl.`|[Bridging the Gap between Object and Image-level Representations for Open-Vocabulary Detection](https://arxiv.org/abs/2207.03482)|[Code](https://github.com/hanoonaR/object-centric-ovd)|
|2022|NeurIPS|`vlm.`, `cap.`|[DetCLIP: Dictionary-Enriched Visual-Concept Paralleled Pre-training for Open-world Detection](https://arxiv.org/abs/2209.09407)|N/A|
|2022|arXiv|`vlm.`|[Open Vocabulary Object Detection with Proposal Mining and Prediction Equalization](https://arxiv.org/abs/2206.11134)|[Code](https://github.com/peixianchen/MEDet)|
|2022|arXiv|`vlm.`, `pl.`|[P3OVD: Fine-grained Visual-Text Prompt-Driven Self-Training for Open-Vocabulary Object Detection](https://arxiv.org/abs/2211.00849)|N/A|
|2023|ICLR|`vlm.`, `pl.`|[Learning Object-Language Alignments for Open-Vocabulary Object Detection](https://arxiv.org/abs/2211.14843)|[Code](https://github.com/clin1223/VLDet)|
|2023|ICLR|`vlm.`|[F-VLM: Open-Vocabulary Object Detection upon Frozen Vision and Language Models](https://arxiv.org/abs/2209.15639)|[Code](https://github.com/google-research/google-research/tree/master/fvlm)|
|2023|CVPR|`other.`, `vlm.` |[Learning to Detect and Segment for Open Vocabulary Object Detection](https://arxiv.org/abs/2212.12130)|N/A|
|2023|CVPR|`vlm.`, `cap.`|[Aligning Bag of Regions for Open-Vocabulary Object Detection](https://arxiv.org/abs/2302.13996)|[Code](https://github.com/wusize/ovdet)|
|2023|CVPR|`vlm.`|[Object-Aware Distillation Pyramid for Open-Vocabulary Object Detection](https://arxiv.org/abs/2303.05892)|[Code](https://github.com/LutingWang/OADP)|
|2023|CVPR|`vlm.`|[CORA: Adapting CLIP for Open-Vocabulary Detection with Region Prompting and Anchor Pre-Matching](https://arxiv.org/abs/2303.13076)|N/A|
|2023|CVPR|`vlm.`, `pl.`|[DetCLIPv2: Scalable Open-Vocabulary Object Detection Pre-training via Word-Region Alignment](https://arxiv.org/abs/2304.04514)|N/A|
|2023|CVPR|`vlm.`|[Region-Aware Pretraining for Open-Vocabulary Object Detection with Vision Transformers](https://arxiv.org/abs/2305.07011)|N/A|
|2023|ICML|`vlm.`|[Multi-Modal Classifiers for Open-Vocabulary Object Detection](https://arxiv.org/abs/2306.05493)|[Project](https://www.robots.ox.ac.uk/~vgg/research/mm-ovod/)|
|2023|arXiv|`vlm.`|[GridCLIP: One-Stage Object Detection by Grid-Level CLIP Representation Learning](https://arxiv.org/abs/2303.09252)|N/A|
|2023|arXiv|`vlm.`, `cap.`|[Enhancing the Role of Context in Region-Word Alignment for Object Detection](https://arxiv.org/abs/2303.10093)|N/A|
|2023|arXiv|`cap.`, `pl.`|[Open-Vocabulary Object Detection using Pseudo Caption Labels](https://arxiv.org/abs/2303.13040)|N/A|
|2023|arXiv|`vlm.`, `pl.`|[Three ways to improve feature alignment for open vocabulary detection](https://arxiv.org/abs/2303.13518)|N/A|
|2023|arXiv|`vlm.`|[Prompt-Guided Transformers for End-to-End Open-Vocabulary Object Detection](https://arxiv.org/abs/2303.14386)|N/A|
|2023|arXiv|`vlm.`, `cap.`, `pl.`|[MaMMUT: A Simple Architecture for Joint Learning for MultiModal Tasks](https://arxiv.org/abs/2303.16839)|N/A|
|2023|arXiv|`vlm.`, `cap.`, `pl.`|[Scaling Open-Vocabulary Object Detection](arxiv.org/abs/2306.09683)|N/A|
|2023|arXiv|`vlm.`|[Open-Vocabulary Object Detection via Scene Graph Discovery](http://arxiv.org/abs/2307.03339)|N/A|
|2023|ICCV|`vlm.`|[Detection-Oriented Image-Text Pretraining for Open-Vocabulary Detection](https://arxiv.org/abs/2310.00161)|[Code](https://github.com/google-research/google-research/tree/master/fvlm/dito)|
|2023|arXiv|`vlm.`|[EdaDet: Open-Vocabulary Object Detection Using Early Dense Alignment](https://arxiv.org/abs/2309.01151)|[Code](https://chengshiest.github.io/edadet/)|
|2023|KDD|`vlm.`|[What Makes Good Open-Vocabulary Detector: A Disassembling Perspective](https://arxiv.org/abs/2309.00227)|N/A|
|2023|NeurIPS |`vlm.`|[CoDet: Co-Occurrence Guided Region-Word Alignment for Open-Vocabulary Object Detection](https://arxiv.org/abs/2310.16667)|[Code](https://github.com/cvmi-lab/codet)|
|2023|arXiv|`vlm.`|[DST-Det: Simple Dynamic Self-Training for Open-Vocabulary Object Detection](https://arxiv.org/abs/2310.01393)|[Code](https://github.com/xushilin1/dst-det)|
|2023|arXiv|`vlm.`|[Taming Self-Training for Open-Vocabulary Object Detection](https://arxiv.org/abs/2308.06412)|[Code](https://github.com/xiaofeng94/sas-det)|
|2023|arXiv|`unify.`, `vlm.`, `pre.`|[CLIPSelf: Vision Transformer Distills Itself for Open-Vocabulary Dense Prediction](https://arxiv.org/abs/2310.01403)|[Code](https://github.com/wusize/CLIPSelf)|
|2023|arXiv|`bench`|[The devil is in the fine-grained details: Evaluating open-vocabulary object detectors for fine-grained understanding](https://arxiv.org/abs/2311.17518)|[Project](https://lorebianchi98.github.io/FG-OVD/)|
|2023|BMVC|`vlm.`|[Open-Vocabulary Object Detection with Meta Prompt Representation and Instance Contrastive Optimization]([http://arxiv.org/abs/2307.03339](https://proceedings.bmvc2023.org/93/))|N/A|
|2024|AAAI|`vlm.`|[Simple Image-level Classification Improves Open-vocabulary Object Detection](https://arxiv.org/abs/2312.10439)|[Code](https://github.com/mala-lab/sic-cads)|
|2024|AAAI|`vlm.`|[ProxyDet: Synthesizing Proxy Novel Classes via Classwise Mixup for Open-Vocabulary Object Detection](https://arxiv.org/abs/2312.07266)|[Code](https://github.com/clovaai/ProxyDet)|
|2024|AAAI|`unify.`, `vlm.`, `pre.`|[CLIM: Contrastive Language-Image Mosaic for Region Representation](https://arxiv.org/abs/2312.11376)|[Code](https://github.com/wusize/CLIM)|
|2024|WACV|`vlm.`|[LP-OVOD: Open-Vocabulary Object Detection by Linear Probing](https://arxiv.org/abs/2310.17109)|[Code](https://github.com/VinAIResearch/LP-OVOD)|
|2024|CVPR|`vlm.`|[YOLO-World: Real-Time Open-Vocabulary Object Detection](https://arxiv.org/abs/2401.17270)|[Code](https://github.com/AILab-CVC/YOLO-World)|

### Open Vocabulary Segmentation

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2023|CVPR|`unify.`, `vlm.` |[Primitive Generation and Semantic-related Alignment for Universal Zero-Shot Segmentation](https://henghuiding.github.io/PADing/)|[Code](https://github.com/heshuting555/PADing)|
|2023|CVPR|`unify.`, `vlm.` |[FreeSeg: Unified, Universal and Open-Vocabulary Image Segmentation](https://arxiv.org/abs/2303.17225)|[Code](https://github.com/bytedance/FreeSeg)|
|2023|arXiv|`unify.`, `vlm.` |[OpenSD: Unified Open-Vocabulary Segmentation and Detection](https://arxiv.org/abs/2312.06703)|[Code](https://github.com/strongwolf/OpenSD)|

#### Semantic Segmentation

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2022|ICLR|`vlm.`|[Language-driven Semantic Segmentation](https://arxiv.org/abs/2201.03546)|[Code](https://github.com/isl-org/lang-seg)|
|2022|CVPR|`cap.`, `w/o ps.`|[GroupViT: Semantic Segmentation Emerges from Text Supervision](https://arxiv.org/abs/2202.11094)|[Code](https://github.com/NVlabs/GroupViT)|
|2022|CVPR|`vlm.`|[ZegFormer: Decoupling Zero-Shot Semantic Segmentation](https://arxiv.org/abs/2112.07910)|[Code](https://github.com/dingjiansw101/ZegFormer)|
|2022|ECCV|`cap.`, `vlm.`|[Scaling Open-Vocabulary Image Segmentation with Image-Level Labels](https://arxiv.org/abs/2112.12143)|N/A|
|2022|ECCV|`vlm`, `pl`, `w/o ps.`|[Extract Free Dense Labels from CLIP](https://arxiv.org/abs/2112.01071)|[Code](https://github.com/chongzhou96/MaskCLIP)|
|2022|ECCV|`vlm.`|[A Simple Baseline for Open-Vocabulary Semantic Segmentation with Pre-trained Vision-Language Model](https://arxiv.org/abs/2112.14757)|[Code](https://github.com/MendelXu/zsseg.baseline)|
|2022|ECCV|`vlm.`, `cap.`, `w/o ps.`|[Open-world Semantic Segmentation via Contrasting and Clustering Vision-Language Embedding](https://arxiv.org/abs/2207.08455)|N/A|
|2022|BMVC|`vlm.`|[Open-vocabulary Semantic Segmentation with Frozen Vision-Language Models](https://arxiv.org/abs/2210.15138)|[Code](https://github.com/chaofanma/Fusioner)|
|2022|arXiv|`vlm.`, `cap.`, `pl`, `w/o ps.`|[Perceptual Grouping in Contrastive Vision-Language Models](https://arxiv.org/abs/2210.09996)|[Code](https://github.com/kahnchana/clippy)|
|2022|arXiv|`vlm.`, `cap.`, `pl`, `w/o ps.`|[SegCLIP: Patch Aggregation with Learnable Centers for Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2211.14813)|[Code](https://github.com/ArrowLuo/SegCLIP)|
|2022|arXiv|`vlm.`, `cap.`, `w/o ps.`|[Open Vocabulary Semantic Segmentation with Patch Aligned Contrastive Learning](https://arxiv.org/abs/2212.04994)|N/A|
|2023|CVPR|`vlm.`, `pre.`|[Generalized Decoding for Pixel, Image, and Language](https://arxiv.org/abs/2212.11270)|[Code](https://github.com/microsoft/X-Decoder/tree/main)|
|2023|CVPR|`vlm.`, `pl.`|[Open-Vocabulary Semantic Segmentation with Mask-adapted CLIP](https://arxiv.org/abs/2210.04150)|[Code](https://github.com/facebookresearch/ov-seg)|
|2023|CVPR|`cap.`, `vlm.`, `w/o ps.`|[Learning Open-vocabulary Semantic Segmentation Models From Natural Language Supervision](https://arxiv.org/abs/2301.09121)|[Code](https://github.com/Jazzcharles/OVSegmentor/)|
|2023|CVPR|`vlm.`|[Side Adapter Network for Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2302.12242)|[Codd](https://github.com/MendelXu/SAN)|
|2023|arXiv|`vlm.`, `unify`|[A Simple Framework for Open-Vocabulary Segmentation and Detection](https://arxiv.org/abs/2303.08131)|[Code](https://github.com/IDEA-Research/OpenSeeD)|
|2023|arXiv|`vlm.`|[Global Knowledge Calibration for Fast Open-Vocabulary Segmentation](https://arxiv.org/abs/2303.09181)|N/A|
|2023|arXiv|`vlm.`|[CAT-Seg: Cost Aggregation for Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2303.11797)|[Code](https://github.com/KU-CVLAB/CAT-Seg)|
|2023|arXiv|`vlm.`, `unify`|[Prompt Pre-Training with Twenty-Thousand Classes for Open-Vocabulary Visual Recognition](https://arxiv.org/abs/2304.04704)|[Code](https://github.com/amazon-science/prompt-pretraining)|
|2023|arXiv|`vlm.`, `unify`|[Segment Everything Everywhere All at Once](https://arxiv.org/abs/2304.06718)|[Code](https://github.com/UX-Decoder/Segment-Everything-Everywhere-All-At-Once)|
|2023|arXiv|`vlm.`|[MVP-SEG: Multi-View Prompt Learning for Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2304.06957)|N/A|
|2023|arXiv|`vlm.`|[TagCLIP: Improving Discrimination Ability of Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2304.07547)|N/A|
|2023|arXiv|`vlm.`, `w/o ps.`, `sam`|[Exploring Open-Vocabulary Semantic Segmentation without Human Labels](https://arxiv.org/abs/2306.00450)|N/A|
|2023|arXiv|`vlm.`, `unify`|[DaTaSeg: Taming a Universal Multi-Dataset Multi-Task Segmentation Model](https://arxiv.org/abs/2306.01736)|N/A|
|2023|arXiv|`diff.`|[Diffusion Models for Zero-Shot Open-Vocabulary Segmentation](https://arxiv.org/abs/2306.09316)|[Project](https://www.robots.ox.ac.uk/~vgg/research/ovdiff/)|
|2023|ICCV|`diff.`|[Diffumask: Synthesizing images with pixel-level annotations for semantic segmentation using diffusion models](https://arxiv.org/abs/2303.11681)|[Project](https://weijiawu.github.io/DiffusionMask/)|
|2023|ICCV|`diff.`|[Guiding Text-to-Image Diffusion Model Towards Grounded Generation](https://arxiv.org/abs/2301.05221)|[Project](https://lipurple.github.io/Grounded_Diffusion/)|
|2023|NeurIPS|`cap.`, `w/o ps.`|[Uncovering Prototypical Knowledge for Weakly Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2310.19001)|[Code](https://github.com/Ferenas/PGSeg)|
|2023|arXiv|`vlm.`|[SED: A Simple Encoder-Decoder for Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2311.15537)|[Code](https://github.com/xb534/SED)|
|2023|arXiv|`vlm.`, `no-train`|[Plug-and-Play, Dense-Label-Free Extraction of Open-Vocabulary Semantic Segmentation from Vision-Language Models](https://arxiv.org/abs/2311.17095)|N/A|
|2023|arXiv|`vlm.`, `no-train`|[Grounding Everything: Emerging Localization Properties in Vision-Language Transformers](https://arxiv.org/abs/2312.00878)|[Code](https://github.com/WalBouss/GEM)|
|2023|arXiv|`vlm.`|[Open-Vocabulary Segmentation with Semantic-Assisted Calibration](https://arxiv.org/abs/2312.04089)|N/A|
|2023|arXiv|`vlm.`, `no-train`|[Self-Guided Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2312.04539)|N/A|
|2023|arXiv|`no-train.`, `vlm.`, `sam`|[CLIP as RNN: Segment Countless Visual Concepts without Training Endeavor](https://arxiv.org/abs/2312.07661)|[Project](https://torrvision.com/clip_as_rnn/)|
|2023|arXiv|`vlm.`|[CLIP-DINOiser: Teaching CLIP a few DINO tricks](https://arxiv.org/abs/2312.12359)|N/A|
|2023|arXiv|`vlm.`, `pl.`|[CLIP Is Also a Good Teacher: A New Learning Framework for Inductive Zero-shot Semantic Segmentation](https://arxiv.org/pdf/2310.02296)|N/A|

#### Instance Segmentation

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2023|CVPR|`vlm.`|[Semantic-Promoted Debiasing and Background Disambiguation for Zero-Shot Instance Segmentation](https://henghuiding.github.io/D2Zero/)|[Code](https://github.com/heshuting555/D2Zero)|
|2022|CVPR|`cap.`, `pl.`, `vlm.`|[Open-Vocabulary Instance Segmentation via Robust Cross-Modal Pseudo-Labeling](https://arxiv.org/abs/2111.12698)|[Code](https://github.com/hbdat/cvpr22_cross_modal_pseudo_labeling)|
|2023|CVPR|`vlm`, `cap`, `w/o ps.`|[Mask-free OVIS: Open-Vocabulary Instance Segmentation without Manual Mask Annotations](https://arxiv.org/abs/2303.16891)|[Code](https://github.com/Vibashan/Maskfree-OVIS)|
|2023|arXiv|`cap.`|[Betrayed by Captions: Joint Caption Grounding and Generation for Open Vocabulary Instance Segmentation](https://arxiv.org/abs/2301.00805)|[Code](https://github.com/jianzongwu/betrayed-by-captions)|
|2023|arXiv|`cap.`|[Leveraging Open-Vocabulary Diffusion to Camouflaged Instance Segmentation](https://arxiv.org/abs/2312.17505)|N/A|


#### Panoptic Segmentation

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2023|CVPR|`unify.`, `vlm.` |[Primitive Generation and Semantic-related Alignment for Universal Zero-Shot Segmentation](https://henghuiding.github.io/PADing/)|[Code](https://github.com/heshuting555/PADing)|
|2022|arXiv|`vlm`|[Open-Vocabulary Panoptic Segmentation with MaskCLIP](https://arxiv.org/abs/2208.08984)|N/A|
|2023|CVPR|`diff`, `vlm`|[Open-Vocabulary Panoptic Segmentation with Text-to-Image Diffusion Models](https://arxiv.org/abs/2303.04803)|[Code](https://github.com/NVlabs/ODISE)|
|2023|arXiv|`vlm.`|[Open-vocabulary Panoptic Segmentation with Embedding Modulation](https://arxiv.org/abs/2303.11324)|N/A|
|2023|arXiv|`vlm.`, `unify`|[Hierarchical Open-vocabulary Universal Image Segmentation]([https://arxiv.org/abs/2303.11324](https://arxiv.org/abs/2307.00764))| [Code](https://github.com/berkeley-hipie/HIPIE)|
|2023|arXiv|`vlm.`|[Generalizable Semantic Vision Query Generation for Zero-shot Panoptic and Semantic Segmentation]([https://arxiv.org/pdf/2402.13697)|N/A|

### Open Vocabulary Video Understanding

#### Video Classification

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2021|arXiv|`vlm.`,`open.`|[ActionCLIP: A New Paradigm for Video Action Recognition](https://arxiv.org/abs/2109.08472)|[Code](https://github.com/sallymmx/ActionCLIP)|
|2022|ECCV|`vlm.`,`open.`|[Prompting Visual-Language Models for Efficient Video Understanding](https://arxiv.org/abs/2112.04478)|[Project](https://ju-chen.github.io/efficient-prompt)|
|2022|ECCV|`vlm.`|[Frozen CLIP Models are Efficient Video Learners](https://arxiv.org/abs/2208.03550)|[Code](https://github.com/OpenGVLab/efficient-video-recognition)|
|2022|ECCV|`vlm.`,`open.`|[Expanding Language-Image Pretrained Models for General Video Recognition](https://arxiv.org/abs/2208.02816)|[Code](https://aka.ms/X-CLIP)|
|2022|arXiv|`vlm.`,`open.`,`audio.`|[Multimodal Open-Vocabulary Video Classification via Pre-Trained Vision and Language Models](https://arxiv.org/abs/2207.07646)|N/A|
|2023|AAAI|`vlm.`,`open.`|[Revisiting Classifier: Transferring Vision-Language Models for Video Recognition](https://arxiv.org/abs/2207.01297)|[Code](https://github.com/whwu95/Text4Vis)|
|2023|ICLR|`vlm.`|[AIM: Adapting Image Models for Efficient Video Action Recognition](https://arxiv.org/abs/2302.03024)|[Project](https://adapt-image-models.github.io/)|
|2023|CVPR|`vlm.`,`open.`|[Fine-tuned CLIP Models are Efficient Video Learners](https://arxiv.org/abs/2212.03640)|[Code](https://github.com/muzairkhattak/ViFi-CLIP)|
|2023|ICML|`vlm.`,`open.`|[Open-VCLIP: Transforming CLIP to an Open-vocabulary Video Model via Interpolated Weight Optimization](https://arxiv.org/abs/2302.00624)|[Code](https://github.com/wengzejia1/Open-VCLIP)|
|2023|ICCV|`vlm.`,`open.`|[Video Action Recognition with Attentive Semantic Units](https://arxiv.org/abs/2303.09756)|N/A|
|2023|ICCV|`vlm.`,`open.`|[MAtch, eXpand and Improve: Unsupervised Finetuning for Zero-Shot Action Recognition with Language Knowledge](https://arxiv.org/abs/2303.08914)|[Code](https://github.com/wlin-at/MAXI)|
|2023|arXiv|`vlm.`,`open.`|[VicTR: Video-conditioned Text Representations for Activity Recognition](https://arxiv.org/abs/2304.02560)|N/A|
|2023|arXiv|`vlm.`,`open.`|[Generating Action-conditioned Prompts for Open-vocabulary Video Action Recognition](https://arxiv.org/abs/2312.02226)|N/A|

#### Tracking

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2023|CVPR|`vlm.`,`open.`|[OVTrack: Open-Vocabulary Multiple Object Tracking](https://arxiv.org/abs/2304.08408)|[Project](https://www.vis.xyz/pub/ovtrack/)|

#### Video Instance Segmentation

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2023|ICCV|`vlm.`,`open.`|[Towards Open-Vocabulary Video Instance Segmentation](https://arxiv.org/abs/2304.01715)|[Code](https://github.com/haochenheheda/LVVIS)|
|2023|arXiv|`vlm.`,`open.`|[OpenVIS: Open-vocabulary Video Instance Segmentation](https://arxiv.org/abs/2305.16835)|N/A|
|2023|arXiv|`vlm.`,`open.`|[DVIS++: Improved Decoupled Framework for Universal Video Segmentation](https://arxiv.org/abs/2312.13305)|[Code](https://github.com/zhang-tao-whu/DVIS_Plus)|

### Open Vocabulary 3D Scene Understanding

#### 3D Classification

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2022|CVPR|`vlm.`|[PointCLIP: Point Cloud Understanding by CLIP](https://arxiv.org/abs/2112.02413)|[Code](https://github.com/ZrrSkywalker/PointCLIP)|
|2023|CVPR|`vlm.`|[ULIP: Learning a Unified Representation of Language, Images, and Point Clouds for 3D Understanding](https://arxiv.org/abs/2212.05171)|[Code](https://github.com/salesforce/ULIP)|
|2023|ICCV|`vlm.`|[PointCLIP V2: Adapting CLIP for Powerful 3D Open-world Learning](https://arxiv.org/abs/2211.11682)|[Code](https://github.com/yangyangyang127/PointCLIP_V2)|
|2023|ICCV|`vlm.`|[CLIP2Point: Transfer CLIP to Point Cloud Classification with Image-Depth Pre-training](https://arxiv.org/abs/2210.01055)|[Code](https://github.com/tyhuang0428/CLIP2Point)|
|2023|ICML|`vlm.`|[Contrast with Reconstruct: Contrastive 3D Representation Learning Guided by Generative Pretraining](https://openreview.net/forum?id=80IfYewOh1)|[Code](https://github.com/qizekun/ReCon)|
|2024|WACV|`vlm.`|[LidarCLIP or: How I Learned to Talk to Point Clouds](https://arxiv.org/abs/2212.06858)|[Code](https://github.com/atonderski/lidarclip)|

#### 3D Detection

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2022|arXiv|`vlm.`|[Open-Vocabulary 3D Detection via Image-level Class and Debiased Cross-modal Contrastive Learning](https://arxiv.org/abs/2207.01987)|N/A|
|2023|CVPR|`vlm.`|[Open-Vocabulary Point-Cloud Object Detection without 3D Annotation](https://arxiv.org/abs/2304.00788v1)|[Code](https://github.com/lyhdet/OV-3DET)|
|2023|NeurIPS|`vlm.`|[CoDA: Collaborative Novel Box Discovery and Cross-modal Alignment for Open-vocabulary 3D Object Detection](https://arxiv.org/abs/2310.02960)|[Project](https://yangcaoai.github.io/publications/CoDA.html)|
|2023|arXiv|`vlm.`|[Object2Scene: Putting Objects in Context for Open-Vocabulary 3D Detection](https://arxiv.org/abs/2309.09456)|N/A|
|2023|arXiv|`vlm.`|[FM-OV3D: Foundation Model-based Cross-modal Knowledge Blending for Open-Vocabulary 3D Detection](https://arxiv.org/abs/2312.14465)|N/A|
|2023|arXiv|`vlm.`|[OpenSight: A Simple Open-Vocabulary Framework for LiDAR-Based Object Detection](https://arxiv.org/abs/2312.08876)|N/A|

#### 3D segmentation

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2023|CVPR|`vlm.`|[PLA: Language-Driven Open-Vocabulary 3D Scene Understanding](https://arxiv.org/abs/2211.16312)|[Code](https://dingry.github.io/projects/PLA)|
|2023|CVPR|`vlm.`|[CLIP2Scene: Towards Label-efficient 3D Scene Understanding by CLIP](https://arxiv.org/abs/2301.04926)|[Code](https://github.com/runnanchen/CLIP2Scene)|
|2023|CVPR|`vlm.`|[OpenScene: 3D Scene Understanding with Open Vocabularies](https://arxiv.org/abs/2211.15654)|[Project](https://pengsongyou.github.io/openscene)|
|2023|ICCVW|`vlm.`|[CLIP-FO3D: Learning Free Open-world 3D Scene Representations from 2D Dense CLIP](https://arxiv.org/abs/2303.04748)|N/A|
|2023|NeurIPS|`vlm.`|[OpenMask3D: Open-Vocabulary 3D Instance Segmentation](https://arxiv.org/abs/2306.13631)|[Project](https://openmask3d.github.io/)|
|2023|arXiv|`vlm.`|[OpenIns3D: Snap and Lookup for 3D Open-vocabulary Instance Segmentation](https://arxiv.org/abs/2309.00616)|[Project](https://zheninghuang.github.io/OpenIns3D/)|
|2023|arXiv|`vlm.`|[Open3DIS: Open-vocabulary 3D Instance Segmentation with 2D Mask Guidance](https://arxiv.org/abs/2312.10671)|[Project](https://open3dis.github.io)|

## Related Domains and Beyond

### Class-agnostic Detection and Segmentation

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2022|RA-L|-|[Learning Open-World Object Proposals without Learning to Classify](https://arxiv.org/abs/2108.06753)|[Code](https://github.com/mcahny/object_localization_network)|
|2021|ICCV|-|[Unidentified Video Objects: A Benchmark for Dense, Open-World Segmentation](https://arxiv.org/abs/2104.04691)|[Project](https://sites.google.com/view/unidentified-video-object/home)|
|2022|CVPR|-|[Open-World Instance Segmentation: Exploiting Pseudo Ground Truth From Learned Pairwise Affinity](https://arxiv.org/abs/2204.06107)|[Project](https://sites.google.com/view/generic-grouping/)|
|2022|ECCV|-|[Class-agnostic object detection with multi-modal transformer](https://arxiv.org/abs/2111.11430)|[Code](https://git.io/J1HPY)|
|2022|TPAMI|-|[Open World Entity Segmentation](https://arxiv.org/abs/2107.14228)|[Project](http://luqi.info/Entity_Web/)|
|2022|arXiv|-|[Fine-Grained Entity Segmentation](https://arxiv.org/abs/2211.05776)|[Project](http://luqi.info/entityv2.github.io/)|

### Open-World Object Detection

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2015|CVPR|-|[Towards Open World Recognition](https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Bendale_Towards_Open_World_2015_CVPR_paper.html)|N/A|
|2021|CVPR|-|[Towards Open World Object Detection.](https://arxiv.com/abs/2103.02603)|[Code](https://github.com/JosephKJ/OWOD)|
|2022|CVPR|-|[OW-DETR: Open-world Detection Transformer](https://arxiv.org/abs/2112.01513)|[Code](https://github.com/akshitac8/OW-DETR)|
|2022|ECCV|-|[UC-OWOD: Unknown-Classified Open World Object Detection](https://arxiv.com/abs/2207.11455)|[Code](https://github.com/JohnWuzh/UC-OWOD)|
|2022|arXiv|-|[Revisiting Open World Object Detection](https://arxiv.org/abs/2201.00471)|[Code](https://github.com/RE-OWOD/RE-OWOD)|
|2022|arXiv|-|[Rectifying Open-set Object Detection: A Taxonomy, Practical Applications, and Proper Evaluation](https://arxiv.org/abs/2207.09775)|[N/A]
|2022|arXiv|-|[Open World DETR: Transformer based Open World Object Detection](https://arxiv.org/abs/2212.02969)|N/A|
|2023|CVPR|-|[PROB: Probabilistic Objectness for Open World Object Detection](https://arxiv.org/abs/2212.01424)|[Code](https://github.com/orrzohar/PROB)|
|2023|arXiv|-|[Open World Object Detection in the Era of Foundation Models](https://arxiv.org/abs/2312.05745)|[Code](https://github.com/orrzohar/FOMO)|
|2023|arXiv|-|[Hyp-OW: Exploiting Hierarchical Structure Learning with Hyperbolic Distance Enhances Open World Object Detection](https://arxiv.org/abs/2306.14291)|[N/A]|

### Open-Set Panoptic Segmentation

|Year|Venue|Keywords|Paper Title|Code/Project|
|:-:|:-:|:-:|-|-|
|2021|CVPR|-|[Exemplar-Based Open-Set Panoptic Segmentation Network](https://arxiv.org/abs/2105.08336)|[Project](https://cv.snu.ac.kr/research/EOPSN/)|
|2022|arXiv|-|[Dual Decision Improves Open-Set Panoptic Segmentation](https://arxiv.org/abs/2207.02504)|[Code](https://github.com/HeimingX/OPS_dual_decision)|

## Acknowledgement

If you find our survey and repository useful for your research project, please consider citing our paper:

```bibtex
@article{wu2023open,
      title={Towards Open Vocabulary Learning: A Survey}, 
      author={Jianzong Wu and Xiangtai Li and Shilin Xu and Haobo Yuan and Henghui Ding and Yibo Yang and Xia Li and Jiangning Zhang and Yunhai Tong and Xudong Jiang and Bernard Ghanem and Dacheng Tao},
      year={2024},
      journal={T-PAMI},
}
```

## Contact

```
jzwu@stu.pku.edu.cn
```
```
lxtpku@pku.edu.cn or xiangtai94@gmail.com
```
