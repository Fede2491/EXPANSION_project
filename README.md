Some of my codes used in the EXPANSION project: EXPlainable AI through high eNergy physicS for medical Imaging in ONco.

#-

blob.ipynb

This notebook provides the complete pipeline for generating jet images from the dataset JETCLASS:: A Large Dataset for DeepLearning in Jet Physics (link: https://zenodo.org/records/6619768).
Starting from a ROOT file, the data loader loads the main features related to jet physics (pseudorapidity, azimuthal angle, etc.).
The data loader used in this notebook is taken from:  https://github.com/jet-universe/particle_transformer/blob/main/dataloader.py
      
#-

XCAM_sigbkg_1000.ipynb

In this notebook I report the full code of the XAI model in use for the classification task in signal-background (top decay vs qcd events).
The model in use is custumized EfficientNetV2-S, pretrained with ImageNet1k.
Starting from the images generated with blob.ipynb, we performe classification for different jet blob  per single image.
The extreme differences of the images in this example guarantee a perfect classification over the test sample.
The code continues with the explainability part where the metric deletion and insertion are calculated by considering three different CAM methods: GradCAM, ScoreCAM and EigenCAM.
