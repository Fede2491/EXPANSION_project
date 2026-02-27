Some of my codes used in the EXPANSION project: EXPlainable AI through high eNergy physicS for medical Imaging in ONco.

#-

blob.ipynb

This notebook provides the complete pipeline for generating jet images from the dataset JETCLASS:: A Large Dataset for DeepLearning in Jet Physics (link: https://zenodo.org/records/6619768).
Starting from a ROOT file, the data loader loads the main features related to jet physics (pseudorapidity, azimuthal angle, etc.).
The data loader used in this notebook is taken from:  https://github.com/jet-universe/particle_transformer/blob/main/dataloader.py
      
#-

XCAM_sigbkg_1000.ipynb

In this notebook, I present the complete code of the XAI model used for the signal–background classification task (top-quark decay vs. QCD events).
The model is a customized EfficientNetV2-S, pretrained on ImageNet-1k.
Starting from the images generated with blob.ipynb, we perform classification on different jet blobs within each single image.
The extreme differences between the images in this example guarantee perfect classification on the test sample.
The code then proceeds with the explainability stage, where the deletion and insertion metrics are computed using three different CAM methods: Grad-CAM, Score-CAM, and Eigen-CAM.

#-

pretrain_1000_10cl.ipynb

A first test of complete transfer learning from HEP to medical field.
