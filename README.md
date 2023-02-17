# Open Vocabulary Survey


If you find missing cited works or some suggestions to this survey. Please send us an issue. 

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

## Keywords

- `cap.`: Use caption as training data
- `vlm.`: Use pretrained VLMs like CLIP 
- `pl.`: Generate pseudo labels
- `w/o ps.`: Without pixel-level supervision
- `osps.`: Open-Set Panoptic Segmentation
- `pre.`: Vision-language pretraining
- `other.`: Other methods that cannot be grouped into above ones.

## Open Vocabulary Classification 


## Vision Language Modeling 

|Paper|Source|Keywords|
|-|-|-|
|GLIP|||
||||

## Object Detection

|Paper|Source|Keywords|
|-|-|-|
|[Open-Vocabulary Object Detection Using Captions](https://arxiv.org/abs/2011.10678)|CVPR 2021 Oral|`cap.`|
|[RegionCLIP: Region-based Language-Image Pretraining](https://arxiv.org/abs/2112.09106)|arXiv 2021.12|`cap.`, `vlm.`, `pre.`|
|[Learning to Prompt for Open-Vocabulary Object Detection with Vision-Language Model](https://arxiv.org/abs/2203.14940)|CVPR 2022|`vlm.`|
|[Open-vocabulary Object Detection via Vision and Language Knowledge Distillation](https://arxiv.org/abs/2104.13921)|ICLR 2022|`vlm.`|
|[Localized Vision-Language Matching for Open-vocabulary Object Detection](https://arxiv.org/abs/2205.06160)|GCPR 2022|`cap.`|
|[Open-Vocabulary DETR with Conditional Matching](https://arxiv.org/abs/2203.11876)|ECCV 2022 Oral|`vlm.`|
|[Open Vocabulary Object Detection with Pseudo Bounding-Box Labels](https://arxiv.org/abs/2111.09452)|ECCV 2022|`vlm.`, `cap.`, `pl.`|
|[Promptdet: Towards open-vocabulary detection using uncurated images](https://arxiv.org/abs/2203.16513)|ECCV 2022|`vlm.`|
|[Detecting Twenty-thousand Classes using Image-level Supervision](https://arxiv.org/abs/2201.02605)|ECCV 2022|`vlm.`, `pl.`, `w/o ps.`|
|[Exploiting unlabeled data with vision and language models for object detection](https://arxiv.org/abs/2207.08954)|ECCV 2022|`vlm.`. `pl.`|
|[Simple Open-Vocabulary Object Detection with Vision Transformers](https://arxiv.org/abs/2205.06230)|ECCV 2022|`vlm.`, `cap.`|
|[Bridging the Gap between Object and Image-level Representations for Open-Vocabulary Detection](https://arxiv.org/abs/2207.03482)|NIPS 2022|`vlm.`, `pl.`|
|[DetCLIP: Dictionary-Enriched Visual-Concept Paralleled Pre-training for Open-world Detection](https://arxiv.org/abs/2209.09407)|NIPS 2022|`vlm.`, `cap.`|
|[Open-Vocabulary One-Stage Detection with Hierarchical Visual-Language Knowledge Distillation](https://arxiv.org/abs/2203.10593)|arXiv 2022.03|`vlm.`, `cap.`|
|[Open Vocabulary Object Detection with Proposal Mining and Prediction Equalization](https://arxiv.org/abs/2206.11134)|arXiv 2022.06|`vlm.`|
|[F-VLM: Open-Vocabulary Object Detection upon Frozen Vision and Language Models](https://arxiv.org/abs/2209.15639)|arXiv 2022.09|`vlm.`|
|[P3OVD: Fine-grained Visual-Text Prompt-Driven Self-Training for Open-Vocabulary Object Detection](https://arxiv.org/abs/2211.00849)|arXiv 2022.11|`vlm.`, `pl.`|
|[Learning Object-Language Alignments for Open-Vocabulary Object Detection](https://arxiv.org/abs/2211.14843)|arXiv 2022.11|`vlm.`, `pl.`|
|[Learning to Detect and Segment for Open Vocabulary Object Detection](https://arxiv.org/abs/2212.12130)|arXiv 2022.12|`other.`|

## Image Segmentation

### Semantic Segmentation

|Paper|Source|Keywords|
|-|-|-|
|[Language-driven Semantic Segmentation](https://arxiv.org/abs/2201.03546)|ICLR 2022|`vlm.`|
|[GroupViT: Semantic Segmentation Emerges from Text Supervision](https://arxiv.org/abs/2202.11094)|CVPR 2022|`cap.`, `w/o ps.`|
|[ZegFormer: Decoupling Zero-Shot Semantic Segmentation](https://arxiv.org/abs/2112.07910)|CVPR 2022|`vlm.`|
|[Scaling Open-Vocabulary Image Segmentation with Image-Level Labels](https://arxiv.org/abs/2112.12143)|ECCV 2022|`cap.`, `vlm.`|
|[Extract Free Dense Labels from CLIP](https://arxiv.org/abs/2112.01071)|ECCV 2022 Oral|`vlm`, `pl`|
|[A Simple Baseline for Open-Vocabulary Semantic Segmentation with Pre-trained Vision-Language Model](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136890725.pdf)|ECCV 2022|`vlm.`|
|[Open-world Semantic Segmentation via Contrasting and Clustering Vision-Language Embedding](https://arxiv.org/abs/2207.08455)|ECCV 2022|`vlm.`, `w/o ps.`|
|[Open-vocabulary Semantic Segmentation with Frozen Vision-Language Models](https://arxiv.org/abs/2210.15138)|BMVC 2022 Oral|`vlm.`|
|[Open-Vocabulary Semantic Segmentation with Mask-adapted CLIP](https://arxiv.org/abs/2210.04150)|arXiv 2022.10|`vlm.`, `pl.`|
|[SegCLIP: Patch Aggregation with Learnable Centers for Open-Vocabulary Semantic Segmentation](https://arxiv.org/abs/2211.14813)|arXiv 2022.11|`vlm.`, `cap.`, `w/o ps.`|
|[Learning to Generate Text-grounded Mask for Open-world Semantic Segmentation from Only Image-Text Pairs](https://arxiv.org/abs/2212.00785)|arXiv 2022.12|`vlm.`, `cap.`, `w/o ps.`|
|[Open Vocabulary Semantic Segmentation with Patch Aligned Contrastive Learning](https://arxiv.org/abs/2212.04994)|arXiv 2022.12|`vlm.`, `cap.`|
|[Learning Open-vocabulary Semantic Segmentation Models From Natural Language Supervision](https://arxiv.org/abs/2301.09121)|arXiv 2023.01|`cap.`, `w.o ps.`|

### Instance Segmentation
|Paper|Source|Keywords|
|-|-|-|
|[Open-Vocabulary Instance Segmentation via Robust Cross-Modal Pseudo-Labeling](https://arxiv.org/abs/2111.12698)|CVPR 2022||


### Panoptic Segmentation

|Paper|Source|Keywords|
|-|-|-|
|[Exemplar-Based Open-Set Panoptic Segmentation Network](https://arxiv.org/abs/2105.08336)|CVPR 2021|`osps.`|
|[Dual Decision Improves Open-Set Panoptic Segmentation](https://arxiv.org/abs/2207.02504)|arXiv 2022.08|`osps.`|
|[Open-Vocabulary Panoptic Segmentation with MaskCLIP](https://arxiv.org/abs/2208.08984)|arXiv 2022.08|`vlm`, `pl.`|

## Video Scene Understanding

## 3D Scene Understanding 

## Open World

### Keywords

- `first.`: the first paper to propose open world.
- `re.`: revisiting/rethinking open world setting.
- `anno.`: discuss the granularity of annotations.

|Paper|Source|Keywords|
|-|-|-|
|[Towards Open World Recognition](https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Bendale_Towards_Open_World_2015_CVPR_paper.html)|CVPR 2015|`first.`|
|[OW-DETR: Open-world Detection Transformer](https://arxiv.org/abs/2112.01513)|CVPR 2022||
|[Revisiting Open World Object Detection](https://arxiv.org/abs/2201.00471)|arXiv 2022.01|`re.`|
|[Rectifying Open-set Object Detection: A Taxonomy, Practical Applications, and Proper Evaluation](https://arxiv.org/abs/2207.09775)|arXiv 2022.07|`re.`, `anno.`|
|[Open World DETR: Transformer based Open World Object Detection](https://arxiv.org/abs/2212.02969)|arXiv 2022.12||
|[PROB: Probabilistic Objectness for Open World Object Detection](https://arxiv.org/abs/2212.01424)|arXiv 2022.12||
|[Learning to Generate Text-grounded Mask for Open-world Semantic Segmentation from Only Image-Text Pairs](https://arxiv.org/abs/2212.00785)|arXiv 2022.12||


