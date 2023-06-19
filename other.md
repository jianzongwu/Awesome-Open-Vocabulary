## Datasets & Benchmarks
### Detection
|Datasets|base|novel|Tasks|
|-|-|-|-|
|COCO OVD|48|17|`det.`|
|LVIS OVD|866|337|`det.`|
|PASCAL VOC|-|20|`det.`|
|Objects365|-|365|`det.`|
|LVIS|-|1,203|`det.`|
|OpenImages|-|500|`det.`|

### Semantic Segmentation
> The OV-SS task can be evaluated with different protocols (Zero-Shot, Cross-Dataset, and Annotation-Free). In general, there is not a consensus on evaluation protocol like OV-OD. Recent papers ([TCL](https://arxiv.org/abs/2212.00785), [PACL](https://arxiv.org/abs/2212.04994)) tend to evaluate on the Annotation-Free protocol.

|Datasets|base|novel|Tasks|
|-|-|-|-|
|PASCAL VOC|-|20|`seg.`|
|PASCAL Context|-|59|`seg.`|
|PASCAL Context|-|459|`seg.`|
|ADE20k-150|-|150|`seg.`|
|ADE20k-847|-|847|`seg.`|
|COCO Stuff|-|171|`seg.`|
|Cityscapes|-|19|`seg.`|

### Open Vocabulary Video Understanding

#### Video Classification

|Year|Venue|Keywords|Acronym|Paper Title|Code/Project|
|:-:|:-:|:-:|:-:|-|-|
|2021|arXiv|`vlm.`,`open.`|ActionCLIP|[ActionCLIP: A New Paradigm for Video Action Recognition](https://arxiv.org/abs/2109.08472)|[Code](https://github.com/sallymmx/ActionCLIP)|
|2022|ECCV|`vlm.`,`open.`|I-VL|[Prompting Visual-Language Models for Efficient Video Understanding](https://arxiv.org/abs/2112.04478)|[Project](https://ju-chen.github.io/efficient-prompt)|
|2022|ECCV|`vlm.`|EVL|[Frozen CLIP Models are Efficient Video Learners](https://arxiv.org/abs/2208.03550)|[Code](https://github.com/OpenGVLab/efficient-video-recognition)|
|2022|ECCV|`vlm.`,`open.`|X-CLIP|[Expanding Language-Image Pretrained Models for General Video Recognition](https://arxiv.org/abs/2208.02816)|[Code](https://aka.ms/X-CLIP)|
|2022|arXiv|`vlm.`,`open.`,`audio.`|MOV|[Multimodal Open-Vocabulary Video Classification via Pre-Trained Vision and Language Models](https://arxiv.org/abs/2207.07646)|N/A|
|2023|AAAI|`vlm.`,`open.`|Text4Vis|[Revisiting Classifier: Transferring Vision-Language Models for Video Recognition](https://arxiv.org/abs/2207.01297)|[Code](https://github.com/whwu95/Text4Vis)|
|2023|ICLR|`vlm.`|AIM|[AIM: Adapting Image Models for Efficient Video Action Recognition](https://arxiv.org/abs/2302.03024)|[Project](https://adapt-image-models.github.io/)|
|2023|CVPR|`vlm.`,`open.`|ViFi-CLIP|[Fine-tuned CLIP Models are Efficient Video Learners](https://arxiv.org/abs/2212.03640)|[Code](https://github.com/muzairkhattak/ViFi-CLIP)|
|2023|ICML|`vlm.`,`open.`|Open-VCLIP|[Open-VCLIP: Transforming CLIP to an Open-vocabulary Video Model via Interpolated Weight Optimization](https://arxiv.org/abs/2302.00624)|[Code](https://github.com/wengzejia1/Open-VCLIP)|
|2023|arXiv|`vlm.`,`open.`|ASU|[Video Action Recognition with Attentive Semantic Units](https://arxiv.org/abs/2303.09756)|N/A|
|2023|arXiv|`vlm.`,`open.`|VicTR|[VicTR: Video-conditioned Text Representations for Activity Recognition](https://arxiv.org/abs/2304.02560)|N/A|
|2023|arXiv|`vlm.`,`open.`|MAXI|[MAtch, eXpand and Improve: Unsupervised Finetuning for Zero-Shot Action Recognition with Language Knowledge](https://arxiv.org/abs/2303.08914)|N/A|

#### Tracking

|Year|Venue|Keywords|Acronym|Paper Title|Code/Project|
|:-:|:-:|:-:|:-:|-|-|
|2023|CVPR|`vlm.`,`open.`|OVTrack|[OVTrack: Open-Vocabulary Multiple Object Tracking](https://arxiv.org/abs/2304.08408)|[Project](https://www.vis.xyz/pub/ovtrack/)|

#### Video Instance Segmentation

|Year|Venue|Keywords|Acronym|Paper Title|Code/Project|
|:-:|:-:|:-:|:-:|-|-|
|2023|arXiv|`vlm.`,`open.`|MindVLT|[Towards Open-Vocabulary Video Instance Segmentation](https://arxiv.org/abs/2304.01715)|N/A|
|2023|arXiv|`vlm.`,`open.`|OpenVIS|[OpenVIS: Open-vocabulary Video Instance Segmentation](https://arxiv.org/abs/2305.16835)|N/A|

### Open Vocabulary 3D Scene Understanding

#### 3D Classification

|Year|Venue|Keywords|Acronym|Paper Title|Code/Project|
|:-:|:-:|:-:|:-:|-|-|
|2022|CVPR|`vlm.`|PointCLIP|[PointCLIP: Point Cloud Understanding by CLIP](https://arxiv.org/abs/2112.02413)|[Code](https://github.com/ZrrSkywalker/PointCLIP)|
|2022|arXiv|`vlm.`|CLIP2Point|[CLIP2Point: Transfer CLIP to Point Cloud Classification with Image-Depth Pre-training](https://arxiv.org/abs/2210.01055)|[Code](https://github.com/tyhuang0428/CLIP2Point)|
|2022|arXiv|`vlm.`|PointCLIPV2|[PointCLIP V2: Adapting CLIP for Powerful 3D Open-world Learning](https://arxiv.org/abs/2211.11682)|[Code](https://github.com/yangyangyang127/PointCLIP_V2)|
|2022|arXiv|`vlm.`|LidarCLIP|[LidarCLIP or: How I Learned to Talk to Point Clouds](https://arxiv.org/abs/2212.06858)|[Code](https://github.com/atonderski/lidarclip)|
|2023|CVPR|`vlm.`|ULIP|[ULIP: Learning a Unified Representation of Language, Images, and Point Clouds for 3D Understanding](https://arxiv.org/abs/2212.05171)|[Code](https://github.com/salesforce/ULIP)|

#### 3D Detection

|Year|Venue|Keywords|Acronym|Paper Title|Code/Project|
|:-:|:-:|:-:|:-:|-|-|
|2022|arXiv|`vlm.`|OV-3DETIC|[Open-Vocabulary 3D Detection via Image-level Class and Debiased Cross-modal Contrastive Learning](https://arxiv.org/abs/2207.01987)|N/A|

#### 3D segmentation

|Year|Venue|Keywords|Acronym|Paper Title|Code/Project|
|:-:|:-:|:-:|:-:|-|-|
|2023|CVPR|`vlm.`|PLA|[PLA: Language-Driven Open-Vocabulary 3D Scene Understanding](https://arxiv.org/abs/2211.16312)|[Code](https://dingry.github.io/projects/PLA)|
|2023|CVPR|`vlm.`|CLIP2Scene|[CLIP2Scene: Towards Label-efficient 3D Scene Understanding by CLIP](https://arxiv.org/abs/2301.04926)|[Code](https://github.com/runnanchen/CLIP2Scene)|
|2023|arXiv|`vlm.`|CLIP-FO3D|[CLIP-FO3D: Learning Free Open-world 3D Scene Representations from 2D Dense CLIP](https://arxiv.org/abs/2303.04748)|N/A|

## Related Domains and Beyond

### Class-agnostic Detection and Segmentation

|Year|Venue|Keywords|Acronym|Paper Title|Code/Project|
|:-:|:-:|:-:|:-:|-|-|
|2022|RA-L|-|OLN|[Learning Open-World Object Proposals without Learning to Classify](https://arxiv.org/abs/2108.06753)|[Code](https://github.com/mcahny/object_localization_network)|
|2021|ICCV|-|UVO|[Unidentified Video Objects: A Benchmark for Dense, Open-World Segmentation](https://arxiv.org/abs/2104.04691)|[Project](https://sites.google.com/view/unidentified-video-object/home)|
|2022|CVPR|-|GGN|[Open-World Instance Segmentation: Exploiting Pseudo Ground Truth From Learned Pairwise Affinity](https://arxiv.org/abs/2204.06107)|[Project](https://sites.google.com/view/generic-grouping/)|
|2022|ECCV|-|MViT|[Class-agnostic object detection with multi-modal transformer](https://arxiv.org/abs/2111.11430)|[Code](https://git.io/J1HPY)|
|2022|TPAMI|-|ES|[Open World Entity Segmentation](https://arxiv.org/abs/2107.14228)|[Project](http://luqi.info/Entity_Web/)|
|2022|arXiv|-|CropFormer|[Fine-Grained Entity Segmentation](https://arxiv.org/abs/2211.05776)|[Project](http://luqi.info/entityv2.github.io/)|
