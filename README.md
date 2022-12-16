<!--A curated list of resources for Image and Video Deblurring-->
<!-- PROJECT LOGO -->
<p align="center">
  <h3 align="center">Intrinsic Decomposition & Inverse Rendering</h3>
</p>

![image](https://user-images.githubusercontent.com/16313809/154192348-ed0b7513-edb1-479b-bf98-c9eb1ce5fbba.png)

[A Survey on Intrinsic Images: Delving Deep Into Lambert and Beyond](https://arxiv.org/abs/2112.03842)

## Table of contents

- [Intrinsic Decomposition (non-DL)](#intrinsic-decomposition-non-dl)
- [Intrinsic Decomposition (DL)](#intrinsic-decomposition-dl)
- [Inverse Rendering (non-DL)](#inverse-rendering-non-dl)
- [Inverse Rendering (DL)](#inverse-rendering-dl)
- [Portrait Relighting (DL)](#portrait-relighting-dl)
- [Dataset](#dataset)

## Intrinsic Decomposition (non-DL)
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2016|SIGGRAPH|[Live Intrinsic Video](https://gvv.mpi-inf.mpg.de/projects/LiveIntrinsicVideo/)||
|2021|SIGGRAPH|[Real-time Global Illumination Decomposition of Videos](https://zollhoefer.com/papers/arXiv19_GD/page.html)||
|2021|Eurographics|[Interactive Photo Editing on Smartphones via Intrinsic Decomposition](https://mdvmp.hpi3d.de/ipesid/other/ipesid_eg2021_main_compressed.pdf)||

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
|2022|CVPR|[PIE-Net: Photometric Invariant Edge Guided Network for Intrinsic Image Decomposition](https://openaccess.thecvf.com/content/CVPR2022/papers/Das_PIE-Net_Photometric_Invariant_Edge_Guided_Network_for_Intrinsic_Image_Decomposition_CVPR_2022_paper.pdf)|[Code](https://github.com/Morpheus3000/PIE-Net)|

## Inverse Rendering (non-DL)
L:Lighting Estimation, G:Geometry Estimation, M:Material Estimation
|Year|Pub|Paper|Repo|L|G|M|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|2010|SIGGRAPH|[Manifold bootstrapping for SVBRDF capture](https://dl.acm.org/doi/10.1145/1833349.1778835)|||&#10003;|&#10003;|
|2013|SIGGRAPH|[Practical SVBRDF Capture in the Frequency Domain](https://dl.acm.org/doi/10.1145/2461912.2461978)|||&#10003;|&#10003;|
|2014|SIGGRAPH ASIA|[Appearance-from-Motion: Recovering Spatially Varying Surface Reflectance under Unknown Lighting](http://yuedong.shading.me/project/afm/afm.htm)||&#10003;|&#10003;|&#10003;|
|2015|CGF|[Mobile Surface Reflectometry](https://wp.doc.ic.ac.uk/rgi/project/mobile-surface-reflectometry/)|||&#10003;|&#10003;|
|2015|SIGGRAPH|[Two-Shot SVBRDF Capture for Stationary Materials](https://dl.acm.org/doi/10.1145/2766967)|[Code & Dataset](https://mediatech.aalto.fi/publications/graphics/TwoShotSVBRDF/)||&#10003;|&#10003;|
|2016|SIGGRAPH ASIA|[Simultaneous Acquisition of Microscale Reflectance and Normals](http://vclab.kaist.ac.kr/siggraphasia2016p2/index.html)|||&#10003;|&#10003;|
|2016|SIGGRAPH ASIA|[Recovering Shape and Spatially-Varying Surface Reflectance under Unknown Illumination](https://www.cs.wm.edu/~ppeers/publications/Xia2016RSS/Xia_SIGGRAPHAsia2016.pdf)||&#10003;|&#10003;|&#10003;|
|2017|SIGGRAPH ASIA|[Polarization imaging reflectometry in the wild](https://wp.doc.ic.ac.uk/rgi/project/polarization-imaging-reflectometry-in-the-wild/)|||&#10003;|&#10003;|
|2018|SIGGRAPH ASIA|[Simultaneous Acquisition of Polarimetric SVBRDF and Normals](http://vclab.kaist.ac.kr/siggraphasia2018p2/index.html)|||&#10003;|&#10003;|
|2021|Eurographics|[Progressive Acquisition of SVBRDF and Shape in Motion](http://vclab.kaist.ac.kr/cgf2020/index.html)|||&#10003;|&#10003;|

## Inverse Rendering (DL)
L:Lighting Estimation, G:Geometry Estimation, M:Material Estimation
|Year|Pub|Paper|Repo|L|G|M|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|2016|SIGGRAPH|[Reflectance Modeling by Neural Texture Synthesis](https://mediatech.aalto.fi/publications/graphics/NeuralSVBRDF/)|||&#10003;|&#10003;|
|2017|CVPR|[Deep Outdoor Illumination Estimation](https://arxiv.org/abs/1611.06403)|[Dataset](https://vision.cs.princeton.edu/projects/2012/SUN360/data/)|&#10003;||
|2017|SIGGRAPH|[Modeling Surface Appearance from a Single Photograph using Self-augmented Convolutional Neural Networks](https://arxiv.org/abs/1809.00886)|[Code](https://github.com/msraig/self-augmented-net)||&#10003;|&#10003;|
|2017|ICCV|[Reflectance Capture using Univariate Sampling of BRDFs](https://openaccess.thecvf.com/content_iccv_2017/html/Hui_Reflectance_Capture_Using_ICCV_2017_paper.html)|||&#10003;|&#10003;|
|2017|SIGGRAPH ASIA|[Learning to Predict Indoor Illumination from a Single Image](https://arxiv.org/abs/1704.00090)|[Dataset](http://indoor.hdrdb.com/)|&#10003;||
|2018|SIGGRAPH|[Single-Image SVBRDF Capture with a Rendering-Aware Deep Network](https://arxiv.org/abs/1810.09718)|[Code & Dataset](https://repo-sam.inria.fr/fungraph/deep-materials/)||&#10003;|&#10003;|
|2018|3DV|[Learning to Estimate Indoor Lighting from 3D Objects](https://arxiv.org/abs/1806.03994)|[Code & Dataset](https://github.com/weberhen/learning_indoor_lighting)|&#10003;||
|2018|SIGGRAPH ASIA|[Relighting Humans: Occlusion-Aware Inverse Rendering for Full-Body Human Images](http://kanamori.cs.tsukuba.ac.jp/projects/relighting_human/)|[Code & Dataset](http://kanamori.cs.tsukuba.ac.jp/projects/relighting_human/)|&#10003;|&#10003;|&#10003;|
|2018|SIGGRAPH ASIA|[Learning to Reconstruct Shape and Spatially-Varying Reflectance from a Single Image](https://cseweb.ucsd.edu/~viscomp/projects/SIGA18ShapeSVBRDF/)|[Code](https://github.com/lzqsd/SingleImageShapeAndSVBRDF) / [Dataset](https://cseweb.ucsd.edu/~viscomp/projects/SIGA18ShapeSVBRDF/)||&#10003;|&#10003;|
|2019|CVPR|[Fast Spatially-Varying Indoor Lighting Estimation](https://arxiv.org/abs/1906.03799)|[Dataset](https://lvsn.github.io/fastindoorlight/)|&#10003;||&#10003;|
|2019|CVPR|[All-Weather Deep Outdoor Lighting Estimation](https://lvsn.github.io/allweather/)|[Dataset](http://outdoor.hdrdb.com/)|&#10003;||
|2019|CVPR|[DeepLight: Learning Illumination for Unconstrained Mobile Mixed Reality](https://arxiv.org/abs/1904.01175)||&#10003;||
|2019|CVPR|[Neural Illumination: Lighting Prediction for Indoor Environments](https://illumination.cs.princeton.edu/)|[Dataset](https://niessner.github.io/Matterport/)|&#10003;|&#10003;||
|2019|ICCV|[Deep Parametric Indoor Lighting Estimation](https://lvsn.github.io/deepparametric/)|[Dataset](https://lvsn.github.io/deepparametric/)|&#10003;||
|2020|CVPR|[Lighthouse: Predicting Lighting Volumes for Spatially-Coherent Illumination](https://people.eecs.berkeley.edu/~pratul/lighthouse/)|[Code](https://github.com/pratulsrinivasan/lighthouse) / [Dataset](https://interiornet.org/)|&#10003;||
|2020|CVPR|[Inverse Rendering for Complex Indoor Scenes: Shape, Spatially-Varying Lighting and SVBRDF from a Single Image](http://cseweb.ucsd.edu/~viscomp/projects/CVPR20InverseIndoor/)|[Code](https://github.com/lzqsd/InverseRenderingOfIndoorScene) / [Dataset](https://ucsd-openrooms.github.io/)|&#10003;|&#10003;|&#10003;|
|2020|ECCV|[Object-Based Illumination Estimation with Rendering-Aware Neural Networks](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123600375.pdf)||&#10003;||&#10003;|
|2020|ECCV|[Single-Shot Neural Relighting and SVBRDF Estimation](https://cseweb.ucsd.edu/~viscomp/projects/ECCV20NeuralRelighting/)|[Code](https://github.com/ssangx/NeuralRelighting) / [Dataset](https://cseweb.ucsd.edu/~viscomp/projects/ECCV20NeuralRelighting/)||&#10003;|&#10003;|
|2020|SIGGRAPH ASIA|[MaterialGAN: Reflectance Capture using a Generative SVBRDF Model](https://shuangz.com/projects/materialgan-sa20/)|[Code](https://github.com/tflsguoyu/materialgan)||&#10003;|&#10003;|
|2021|SIGGRAPH|[Highlight-Aware Two-Stream Network for Single-Image SVBRDF Acquisition](https://sites.cs.ucsb.edu/~lingqi/publications/paper_highlight.pdf)|||&#10003;|&#10003;|
|2021|CVPR|[PhySG: Inverse Rendering with Spherical Gaussians for Physics-based Material Editing and Relighting](https://kai-46.github.io/PhySG-website/) | [Code](https://github.com/Kai-46/PhySG)|&#10003;|&#10003;|&#10003;|
|2021|CVPR|[Deep Polarization Imaging for 3D Shape and SVBRDF Acquisition](https://wp.doc.ic.ac.uk/rgi/project/deep-polarization-3d-imaging/)|[Dataset](https://imperialcollegelondon.app.box.com/s/bbn3t18xostco6rjzr9l7754jb2d22qi)||&#10003;|&#10003;|
|2021|CVPR|[Shape and Material Capture at Home](https://openaccess.thecvf.com/content/CVPR2021/html/Lichy_Shape_and_Material_Capture_at_Home_CVPR_2021_paper.html)|[Code & Dataset](https://github.com/dlichy/ShapeAndMaterial)||&#10003;|&#10003;|
|2021|ICCV|[Learning Indoor Inverse Rendering with 3D Spatially-Varying Lighting](https://nv-tlabs.github.io/inverse-rendering-3d-lighting/) ||&#10003;|&#10003;||
|2021|ICCV|[SurfaceNet: Adversarial SVBRDF Estimation from a Single Image](https://openaccess.thecvf.com/content/ICCV2021/html/Vecchio_SurfaceNet_Adversarial_SVBRDF_Estimation_From_a_Single_Image_ICCV_2021_paper.html)|[Code](https://github.com/perceivelab/surfacenet)||&#10003;|&#10003;|
|2021|AAAI|[EMLight: Lighting Estimation via Spherical Distribution Approximation](https://arxiv.org/abs/2012.11116) ||&#10003;||
|2021|EGSR|[Material and Lighting Reconstruction for Complex Indoor Scenes with Texture-space Differentiable Rendering](http://rgl.epfl.ch/publications/NimierDavid2021Material) ||&#10003;||&#10003;|
|2021|SIGGRAPH ASIA|[Generative Modelling of BRDF Textures from Flash Images](https://henzler.github.io/publication/neuralmaterial/)|[Code](https://github.com/henzler/neuralmaterial)||&#10003;|&#10003;|
|2022|CVPR|[IRISformer: Dense Vision Transformers for Single-Image Inverse Rendering in Indoor Scenes](https://arxiv.org/abs/2206.08423)| [Code](https://github.com/ViLab-UCSD/IRISformer)|&#10003;|&#10003;|&#10003;|


## Portrait Relighting (DL)
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2019|SIGGRAPH|[Single Image Portrait Relighting](https://arxiv.org/abs/1905.00824)||
|2020|CVPR|[Learning Physics-Guided Face Relighting Under Directional Light](https://openaccess.thecvf.com/content_CVPR_2020/html/Nestmeyer_Learning_Physics-Guided_Face_Relighting_Under_Directional_Light_CVPR_2020_paper.html)||
|2020|TOG|[Single Image Portrait Relighting via Explicit Multiple Reflectance Channel Modeling](https://dl.acm.org/doi/abs/10.1145/3414685.3417824)|[Dataset](https://sireer.github.io/projects/FLM_project/)|
|2021|WACV|[Relighting Images in the Wild with a Self-Supervised Siamese Auto-Encoder](https://openaccess.thecvf.com/content/WACV2021/html/Liu_Relighting_Images_in_the_Wild_With_a_Self-Supervised_Siamese_Auto-Encoder_WACV_2021_paper.html)||
|2021|CVPR|[Monocular Reconstruction of Neural Face Reflectance Fields](https://arxiv.org/abs/2008.10247)||
|2021|SIGGRAPH|[Learning to Relight Portraits for Background Replacement](https://augmentedperception.github.io/total_relighting/)||
|2021|ICCV|[Neural Video Portrait Relighting in Real-time via Consistency Modeling](https://zhanglongwen.com/projects/nvpr/)|[Code](https://github.com/ZoneLikeWonderland/Neural-Video-Portrait-Relighting-in-Real-time-via-Consistency-Modeling) / [Dataset](https://zhanglongwen.com/projects/nvpr/dataset.html)|


## Dataset
|Year|Pub|Paper|Repo|
|:---:|:---:|:---:|:---:|
|2014|SIGGRAPH|[Intrinsic Images in the Wild](http://opensurfaces.cs.cornell.edu/publications/intrinsic/)|[Dataset](http://opensurfaces.cs.cornell.edu/publications/intrinsic/)|
|2017|CVPR|[Shading Annotations in the Wild](http://opensurfaces.cs.cornell.edu/publications/saw/)|[Dataset](http://opensurfaces.cs.cornell.edu/publications/saw/)|
|2019|ICCV|[A Dataset of Multi-Illumination Images in the Wild](https://projects.csail.mit.edu/illumination/)|[Code](https://github.com/lmurmann/multi_illumination) / [Dataset](https://projects.csail.mit.edu/illumination/)|
|2021|CVPR|[OpenRooms: An Open Framework for Photorealistic Indoor Scene Datasets](https://ucsd-openrooms.github.io/)|[Dataset](https://ucsd-openrooms.github.io/)|
|2021|ICCV|[Hypersim: A Photorealistic Synthetic Dataset for Holistic Indoor Scene Understanding](https://arxiv.org/abs/2011.02523)|[Dataset](https://github.com/apple/ml-hypersim)|
 
