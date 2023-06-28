## Datasets & Benchmarks

### Detection
> The standard OV-Det use OV-COCO and OV-LVIS datasets for training and evaluation. The detectors are trained on base classes and test both base and novel classes for evaluation.

|Datasets|base|novel|Tasks|
|-|-|-|-|
|COCO OVD|48|17|`det.`|
|LVIS OVD|866|337|`det.`|


### Segmentation

> The OVSS task can be evaluated with different protocols (self-evaluation, cross-evaluation). In general, there is not a consensus on evaluation protocol like OVOD. Please see Sec. 4.2 for details.

#### Open Vocabulary Semantic Segmentation on *self-evaluation setting*

|Datasets|base|novel|
|-|-|-|
|COCO-Stuff|156|15|
|PASCAL VOC|15|5|
|PASCAL Context|49|10|

#### Open Vocabulary Semantic Segmentation on *cross-evaluation setting*

|Datasets|base|novel|
|-|-|-|
|A-847 (ADE20K)|-|847|
|PC-459 (PASCAL Context)|-|459|
|A-150 (ADE20K)|-|150|
|PC-59 (PASCAL Context)|-|59|
|PS-20 (PASCAL VOC)|-|20|

#### Open Vocabulary Instance Segmentation

|Datasets|base|novel|
|-|-|-|
|COCO-Instances|48|17|

#### Open Vocabulary Instance Segmentation

|Datasets|base|novel|
|-|-|-|
|COCO-Instances|48|17|

#### Open Vocabulary Panoptic Segmentation

|Datasets|base|novel|
|-|-|-|
|ADE20K|135|15|
|COCO-Panoptic|156|15|
