## Datasets & Benchmarks

### Detection
> The standard OV-Det use OV-COCO and OV-LVIS datasets for training and evaluation. The detectors are trained on base classes and test both base and novel classes for evaluation.

|Datasets|base|novel|Tasks|
|-|-|-|-|
|COCO OVD|48|17|`det.`|
|LVIS OVD|866|337|`det.`|


### Segmentation
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


