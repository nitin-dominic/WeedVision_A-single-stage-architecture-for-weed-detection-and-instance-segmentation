# WeedVision: A single-stage deep learning architecture to perform weed detection and segmentation using drone-acquired images

### Background
Deep learning (DL) inspired models have achieved tremendous success in locating target weed species through bounding-box approach (single-stage models) or pixel-wise semantic segmentation (two-stage models), but not both. Therefore, the goal of this research study was to develop a single-stage DL architecture that not only locate weed presence through bounding-boxes but also achieves pixel-wise instance segmentation on unmanned aerial system (UAS) acquired remote sensing images. Moreover, the developed architecture experiments on integrating a novel C3 and C3x module within its backbone for dense feature extraction, as well as ProtoNet (Prototypical network) in its head component for weed masking. Furthermore, the proposed architecture has been trained on five categories of dataset exported using multiple combinations of various dataset augmentation techniques, namely, C1, C2, C3, C4, and C5, for which multiple metrics were assessed on desktop graphical processing unit (GPU) and a palm-sized edge device (AGX Xavier). Results suggest that category C4, a combination of six data augmentation techniques, outperformed the remaining categories by achieving precision scores of 85.4 % (bounding-boxes) and 82.8 % (masking) on a GPU. Whereas, the same model converted to TorchScript was able to achieve 79.1 % and 77 % bounding-box and masking accuracy on an edge device, respectively. The model developed in this research has two potential applications when integrated with site-specific weed management technologies. First, it enables real-time weed detection, allowing for the immediate identification of weeds for spot-spraying applications. Second, it facilitates instance weed masking, aiding in the estimation of weed growth extent in actual field conditions. Moreover, the developed architecture combines both computer vision applications - detection and instance segmentation – to provide comprehensive information about weed growth, eliminating the need for multiple algorithm.

### Novel/vital aspects of this research study are:
- Exploring C3 and C3X modules within the DL architecture for robust feature extraction from input images.
- Testing the model on five catrgories of datasets acquired using various combinations of data augmentation techniques.
- Assessing model performance on edge device and real-time tasks.

### Highlights of this research work includes:
- Single-stage model that achieves weed detection and segmentation.
- Integrating C3x module within the backbone for detailed feature extraction.
- Model trained on C4 category achieved the best detection and segmentation scores of 85.4 % and 82.1 %, respectively.
- Model with ONNX format gained 1.25x inference speed on an edge device.

### Hardware used to perform training and inference tasks:
![Detected and segmented weed species in aerial images acquired using UAS.](https://raw.githubusercontent.com/nitin-dominic/NR/master/assets/img/WeedVision.png)
