<!--A curated list of resources for Image and Video Deblurring-->
<!-- PROJECT LOGO -->
<p align="center">
  <h3 align="center">Inverse Rendering</h3>
</p>

## Table of contents

- [Illumination Estimation (DL)](#illumination-estimation-dl)
- [Intrinsic Decomposition (non-DL)](#intrinsic-decomposition-non-dl)
- [Intrinsic Decomposition (DL)](#intrinsic-decomposition-dl)
- [SVBRDF Estimation (non-DL)](#svbrdf-estimation-non-dl)
- [SVBRDF Estimation (DL)](#svbrdf-estimation-dl)
- [Dataset](#dataset)

## Illumination Estimation (DL)
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2017|CVPR|[Deep Outdoor Illumination Estimation](https://arxiv.org/abs/1611.06403)|[Dataset](https://vision.cs.princeton.edu/projects/2012/SUN360/data/)|
|2017|SIGGRAPH ASIA|[Learning to Predict Indoor Illumination from a Single Image](https://arxiv.org/abs/1704.00090)|[Dataset](http://indoor.hdrdb.com/)|
|2018|3DV|[Learning to Estimate Indoor Lighting from 3D Objects](https://arxiv.org/abs/1806.03994)|[Code & Dataset](https://github.com/weberhen/learning_indoor_lighting)|
|2018|SIGGRAPH ASIA|[Relighting Humans: Occlusion-Aware Inverse Rendering for Full-Body Human Images](http://kanamori.cs.tsukuba.ac.jp/projects/relighting_human/)|[Code & Dataset](http://kanamori.cs.tsukuba.ac.jp/projects/relighting_human/)|
|2019|CVPR|[Fast Spatially-Varying Indoor Lighting Estimation](https://arxiv.org/abs/1906.03799)|[Dataset](https://lvsn.github.io/fastindoorlight/)|
|2019|CVPR|[All-Weather Deep Outdoor Lighting Estimation](https://lvsn.github.io/allweather/)|[Dataset](http://outdoor.hdrdb.com/)|
|2019|CVPR|[DeepLight: Learning Illumination for Unconstrained Mobile Mixed Reality](https://arxiv.org/abs/1904.01175)||
|2019|CVPR|[Neural Illumination: Lighting Prediction for Indoor Environments](https://illumination.cs.princeton.edu/)|[Dataset](https://niessner.github.io/Matterport/)|
|2019|ICCV|[Deep Parametric Indoor Lighting Estimation](https://lvsn.github.io/deepparametric/)|[Dataset](https://lvsn.github.io/deepparametric/)|
|2020|CVPR|[Lighthouse: Predicting Lighting Volumes for Spatially-Coherent Illumination](https://people.eecs.berkeley.edu/~pratul/lighthouse/)|[Code](https://github.com/pratulsrinivasan/lighthouse) / [Dataset](https://interiornet.org/)|
|2020|CVPR|[Inverse Rendering for Complex Indoor Scenes: Shape, Spatially-Varying Lighting and SVBRDF from a Single Image](http://cseweb.ucsd.edu/~viscomp/projects/CVPR20InverseIndoor/)|[Code](https://github.com/lzqsd/InverseRenderingOfIndoorScene) / [Dataset](https://ucsd-openrooms.github.io/)|

## Intrinsic Decomposition (non-DL)
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2016|SIGGRAPH|[Live Intrinsic Video](https://gvv.mpi-inf.mpg.de/projects/LiveIntrinsicVideo/)||
|2021|SIGGRAPH|[Real-time Global Illumination Decomposition of Videos](https://zollhoefer.com/papers/arXiv19_GD/page.html)||

## Intrinsic Decomposition (DL)
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2017|Eurographics|[Intrinsic Decompositions for Image Editing](https://perso.liris.cnrs.fr/nicolas.bonneel/intrinsicstar/)|[Code](https://perso.liris.cnrs.fr/nicolas.bonneel/intrinsicstar/supp_materials/code/) [Dataset](https://perso.liris.cnrs.fr/nicolas.bonneel/intrinsicstar/ground_truth/)|
|2017|NeurIPS|[Self-Supervised Intrinsic Image Decomposition](http://rin.csail.mit.edu/)|[Code](https://github.com/JannerM/intrinsics-network) / [Dataset](https://www.shapenet.org/)|
|2018|CVPR|[Intrinsic Image Transformation via Scale Space Decomposition](http://rin.csail.mit.edu/)|[Code](https://github.com/liygcheng/PyrResNet) / [Dataset](http://sintel.is.tue.mpg.de/)|
|2018|CVPR|[Revisiting Deep Intrinsic Image Decompositions](https://arxiv.org/abs/1701.02965)|[Code](https://github.com/fqnchina/IntrinsicImage)|
|2018|CVPR|[Learning Intrinsic Image Decomposition from Watching the World](https://research.cs.cornell.edu/bigtime/)|[Code](https://github.com/zhengqili/unsupervised-learning-intrinsic-images) / [Dataset](https://research.cs.cornell.edu/bigtime/)|
|2018|Pacific Graphics|[Unsupervised Deep Single-Image Intrinsic Decomposition using Illumination-Varying Image Sequences](https://arxiv.org/abs/1803.00805)|[Code](https://github.com/kvanhoey/UnsupervisedIntrinsicDecomposition)|
|2018|ECCV|[CGIntrinsics: Better Intrinsic Image Decomposition through Physically-Based Rendering](https://research.cs.cornell.edu/cgintrinsics/)|[Code](https://github.com/zhengqili/CGIntrinsics) / [Dataset](https://research.cs.cornell.edu/cgintrinsics/)|
|2018|ECCV|[Single Image Intrinsic Decomposition without a Single Intrinsic Image](https://openaccess.thecvf.com/content_ECCV_2018/html/Wei-Chiu_Single_Image_Intrinsic_ECCV_2018_paper.html)||
|2019|CVPR|[InverseRenderNet: Learning single image inverse rendering](https://arxiv.org/abs/1811.12328)|[Code](https://github.com/YeeU/InverseRenderNet) / [Dataset](http://opensurfaces.cs.cornell.edu/publications/intrinsic/)|
|2019|CVPR|[Learning to Separate Multiple Illuminants in a Single Image](https://huizhuo1987.github.io/learningIllum.html)|[Code & Dataset](https://github.com/huizhuo1987/DeepLightSep)|
|2019|ICCV|[Neural Inverse Rendering of an Indoor Scene From a Single Image](https://senguptaumd.github.io/Neural-Inverse-Rendering/)||
|2019|ICCV|[GLoSH: Global-Local Spherical Harmonics for Intrinsic Image Decomposition](https://openaccess.thecvf.com/content_ICCV_2019/html/Zhou_GLoSH_Global-Local_Spherical_Harmonics_for_Intrinsic_Image_Decomposition_ICCV_2019_paper.html)||
|2020|CVPR|[Unsupervised Learning for Intrinsic Image Decomposition from a Single Image](https://arxiv.org/abs/1911.09930)||

## SVBRDF Estimation (non-DL)
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2010|SIGGRAPH|[Manifold bootstrapping for SVBRDF capture](https://dl.acm.org/doi/10.1145/1833349.1778835)||
|2013|SIGGRAPH|[Practical SVBRDF Capture in the Frequency Domain](https://dl.acm.org/doi/10.1145/2461912.2461978)||
|2015|CGF|[Mobile Surface Reflectometry](https://wp.doc.ic.ac.uk/rgi/project/mobile-surface-reflectometry/)||
|2015|SIGGRAPH|[Two-Shot SVBRDF Capture for Stationary Materials](https://dl.acm.org/doi/10.1145/2766967)|[Code & Dataset](https://mediatech.aalto.fi/publications/graphics/TwoShotSVBRDF/)|
|2016|SIGGRAPH ASIA|[Simultaneous Acquisition of Microscale Reflectance and Normals](http://vclab.kaist.ac.kr/siggraphasia2016p2/index.html)||
|2017|SIGGRAPH ASIA|[Polarization imaging reflectometry in the wild](https://wp.doc.ic.ac.uk/rgi/project/polarization-imaging-reflectometry-in-the-wild/)||
## SVBRDF Estimation (DL)
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2016|SIGGRAPH|[Reflectance Modeling by Neural Texture Synthesis](https://mediatech.aalto.fi/publications/graphics/NeuralSVBRDF/)||
|2017|SIGGRAPH|[Modeling Surface Appearance from a Single Photograph using Self-augmented Convolutional Neural Networks](https://arxiv.org/abs/1809.00886)|[Code](https://github.com/msraig/self-augmented-net)|
|2017|ICCV|[Reflectance Capture using Univariate Sampling of BRDFs](https://openaccess.thecvf.com/content_iccv_2017/html/Hui_Reflectance_Capture_Using_ICCV_2017_paper.html)||
|2018|SIGGRAPH|[Single-Image SVBRDF Capture with a Rendering-Aware Deep Network](https://arxiv.org/abs/1810.09718)|[Code & Dataset](https://repo-sam.inria.fr/fungraph/deep-materials/)|
|2021|SIGGRAPH|[Highlight-Aware Two-Stream Network for Single-Image SVBRDF Acquisition](https://sites.cs.ucsb.edu/~lingqi/#publications)||
|2021|CVPR|[Deep Polarization 3D Imaging](https://wp.doc.ic.ac.uk/rgi/project/deep-polarization-3d-imaging/)|[Dataset](https://imperialcollegelondon.app.box.com/s/bbn3t18xostco6rjzr9l7754jb2d22qi)|


## Dataset
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2014|SIGGRAPH|[Intrinsic Images in the Wild](http://opensurfaces.cs.cornell.edu/publications/intrinsic/)|[Dataset](http://opensurfaces.cs.cornell.edu/publications/intrinsic/)|
|2017|CVPR|[Shading Annotations in the Wild](http://opensurfaces.cs.cornell.edu/publications/saw/)|[Dataset](http://opensurfaces.cs.cornell.edu/publications/saw/)|
|2019|ICCV|[A Dataset of Multi-Illumination Images in the Wild](https://projects.csail.mit.edu/illumination/)|[Code](https://github.com/lmurmann/multi_illumination) / [Dataset](https://projects.csail.mit.edu/illumination/)|
|2021|CVPR|[OpenRooms: An Open Framework for Photorealistic Indoor Scene Datasets](https://ucsd-openrooms.github.io/)|[Dataset](https://ucsd-openrooms.github.io/)|
 
