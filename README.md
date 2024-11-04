<div align="center">


# MMAPP
**Multi-branch and Multi-scale Adaptive Progressive Pyramid Network for Multispectral Image Pansharpening.**

______________________________________________________________________
<p align="center">
  <a href="https://ieeexplore.ieee.org/document/10741347">paper</a> •
  <a href="#Abstract">Abstract</a> •
  <a href="#Method">Method</a> •
    <a href="#Dataset">Dataset</a> •
<a href="#Training">Training</a> •
<a href="#Testing">Testing</a> •
  <a href="#Pre-trained-models-and-results">Weights</a> •
  <a href="#Citation">Citation</a><br>
 </p>

[![python](https://img.shields.io/badge/python-%20%203.8-blue.svg)]()
[![license](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/JUSTM0VE0N/MMAPP/blob/main/LICENSE)

</div>

______________________________________________________________________
### Abstract
Pansharpening is the process of integrating two heterogeneous re-mote sensing images to obtain high-resolution multispectral images, which is crucial for downstream tasks. Existing methods utilizing advanced deep learning techniques are able to achieve good sharpen-ing results. However, the heterogeneity between diverse source imag-es is not sufficiently considered, which in turn results in distortions in the sharpening results. Addressing this gap, we have developed a multi-branch pyramid structure, which can build bridges between diverse source images at various scales. It contains three distinct branches, including the PAN branch, the MS branch and the Fusion branch, which efficiently and seamlessly integrates the data flow in distinct branches by means of the pyramid structure. Furthermore, in order to retain more advantageous information, we have developed a specialized adaptive extraction and integration module (AEIM) for each branch, namely, the texture shrinkage adaptive module for the PAN branch, the spectral information consistency module for the MS branch, and the adaptive fusion module for the Fusion branch. These AEIMs are specifically designed to cater to diverse sources and dis-tinct stages of the pansharpening process. The adaptive weights they generate can be used to extract and fuse more advantageous infor-mation. Ultimately, high-fidelity sharpening outcomes are obtained by minimizing the reconstruction errors at various scales in distinct branches. Extensive experiments show that our methodology surpass-es that of representative advanced methods, while maintaining a high level of efficiency. All implementations will be published at MMAPP.


### Method
The overall framework:
<br>
<img src="charts/framework.png" align=center />
The AEIMs in each branch:
<br>
<img src="charts/AEIMs.png" align=center />
