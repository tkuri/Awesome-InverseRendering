# Intrinsic Decomposition, Inverse Rendering & Portrait Relighting

![image](https://user-images.githubusercontent.com/16313809/154192348-ed0b7513-edb1-479b-bf98-c9eb1ce5fbba.png)

A curated reading list of intrinsic image decomposition, recovery of scene geometry/materials/lighting, and portrait relighting.

**Scope:** papers published at major vision, graphics and machine-learning conferences or journals, including CVPR, ICCV, ECCV, SIGGRAPH / SIGGRAPH Asia, NeurIPS, ICLR, AAAI, TPAMI, IJCV, TOG and CGF. 3DV, WACV, Eurographics / EGSR, and relevant workshops of these conferences are also included. Workshop papers are explicitly labeled. An arXiv link may point to the author version of an accepted paper; arXiv-only work is excluded.

**DL** means that the method uses deep learning: a trained network, a scene-optimized neural field/MLP, or a pretrained neural prior. **non-DL** covers explicit physical models and parameter optimization without such a component; automatic differentiation or Gaussian Splatting alone does not imply DL. Hybrid methods are placed in DL when their reconstruction or relighting pipeline uses neural components. Auxiliary masking/feature matching alone is not used to assign DL.

Years refer to the listed publication venue, rather than the first preprint. Resources are official code, data or author project pages where identified; an empty cell means no resource is linked here. Related papers are listed once under their main task. Dataset papers may also occur in method tables when the dataset accompanies a method.

Last literature audit: **2026-10-11**. See [research notes](RESEARCH_NOTES.md) for search coverage, corrections and remaining limitations.

## Table of contents

- [Surveys](#surveys)
- [Intrinsic Decomposition (non-DL)](#intrinsic-decomposition-non-dl)
- [Intrinsic Decomposition (DL)](#intrinsic-decomposition-dl)
- [Inverse Rendering (non-DL)](#inverse-rendering-non-dl)
- [Inverse Rendering (DL)](#inverse-rendering-dl)
- [Portrait Relighting (DL)](#portrait-relighting-dl)
- [Dataset](#dataset)

## Surveys

|Year|Pub|Paper|Resources|
|:---:|:---:|:---:|:---:|
|2017|Eurographics / CGF|[Intrinsic Decompositions for Image Editing](https://perso.liris.cnrs.fr/nicolas.bonneel/intrinsicstar/)|[Code](https://perso.liris.cnrs.fr/nicolas.bonneel/intrinsicstar/supp_materials/code/) [Dataset](https://perso.liris.cnrs.fr/nicolas.bonneel/intrinsicstar/ground_truth/)|
|2021|CGF|[Deep Neural Models for Illumination Estimation and Relighting: A Survey](https://onlinelibrary.wiley.com/doi/10.1111/cgf.14283)||
|2022|IJCV|[A Survey on Intrinsic Images: Delving Deep Into Lambert and Beyond](https://arxiv.org/abs/2112.03842)||
|2026|CGF|[Recent Trends in Inverse Rendering](https://onlinelibrary.wiley.com/doi/10.1111/cgf.70592)||

## Intrinsic Decomposition (non-DL)

|Year|Pub|Paper|Resources|
|:---:|:---:|:---:|:---:|
|2001|ICCV|[Deriving Intrinsic Images from Image Sequences](https://www.cs.jhu.edu/~misha/ReadingSeminar/Papers/Weiss01.pdf)||
|2005|TPAMI|[Recovering Intrinsic Images from a Single Image](https://people.csail.mit.edu/billf/publications/Recovering_Intrinsic_Images.pdf)||
|2008|CVPR|[Intrinsic Image Decomposition with Non-Local Texture Cues](https://www.microsoft.com/en-us/research/publication/intrinsic-image-decomposition-non-local-texture-cues/)||
|2009|SIGGRAPH Asia|[User-Assisted Intrinsic Images](https://people.csail.mit.edu/sparis/publi/2009/sigasia/Bousseau_09_User-assisted_Intrinsic_Images.pdf)||
|2011|NeurIPS|[Recovering Intrinsic Images with a Global Sparsity Prior on Reflectance](https://papers.nips.cc/paper_files/paper/2011/hash/2b8a61594b1f4c4db0902a8a395ced93-Abstract.html)||
|2012|EGSR / CGF|[Intrinsic Images by Clustering](https://giga.cps.unizar.es/~amunoz/projects/EGSR2012_intrinsic/)||
|2016|SIGGRAPH|[Live Intrinsic Video](https://gvv.mpi-inf.mpg.de/projects/LiveIntrinsicVideo/)||
|2021|Eurographics|[Interactive Photo Editing on Smartphones via Intrinsic Decomposition](https://mdvmp.hpi3d.de/ipesid/other/ipesid_eg2021_main_compressed.pdf)||
|2021|SIGGRAPH|[Real-time Global Illumination Decomposition of Videos](https://zollhoefer.com/papers/arXiv19_GD/page.html)||
|2023|CVPR|[Light Source Separation and Intrinsic Image Decomposition Under AC Illumination](https://openaccess.thecvf.com/content/CVPR2023/html/Yoshida_Light_Source_Separation_and_Intrinsic_Image_Decomposition_Under_AC_Illumination_CVPR_2023_paper.html)||

## Intrinsic Decomposition (DL)

|Year|Pub|Paper|Resources|
|:---:|:---:|:---:|:---:|
|2015|ICCV|[Direct Intrinsics: Learning Albedo-Shading Decomposition by Convolutional Regression](https://www.cv-foundation.org/openaccess/content_iccv_2015/html/Narihira_Direct_Intrinsics_Learning_ICCV_2015_paper.html)|[Code](https://github.com/tnarihi/direct-intrinsics)|
|2015|ICCV|[Learning Data-Driven Reflectance Priors for Intrinsic Image Decomposition](https://openaccess.thecvf.com/content_iccv_2015/html/Zhou_Learning_Data-Driven_Reflectance_ICCV_2015_paper.html)||
|2017|CVPR|[Learning Non-Lambertian Object Intrinsics across ShapeNet Categories](https://www.microsoft.com/en-us/research/publication/learning-non-lambertian-object-intrinsics-across-shapenet-categories/)||
|2017|NeurIPS|[Self-Supervised Intrinsic Image Decomposition](http://rin.csail.mit.edu/)|[Code](https://github.com/JannerM/intrinsics-network) / [Dataset](https://www.shapenet.org/)|
|2018|ECCV|[CGIntrinsics: Better Intrinsic Image Decomposition through Physically-Based Rendering](https://research.cs.cornell.edu/cgintrinsics/)|[Code](https://github.com/zhengqili/CGIntrinsics) / [Dataset](https://research.cs.cornell.edu/cgintrinsics/)|
|2018|CVPR|[CNN Based Learning Using Reflection and Retinex Models for Intrinsic Image Decomposition](https://openaccess.thecvf.com/content_cvpr_2018/papers/Baslamisli_CNN_Based_Learning_CVPR_2018_paper.pdf)||
|2018|CVPR|[Intrinsic Image Transformation via Scale Space Decomposition](https://openaccess.thecvf.com/content_cvpr_2018/html/Cheng_Intrinsic_Image_Transformation_CVPR_2018_paper.html)|[Code](https://github.com/liygcheng/PyrResNet) / [Dataset](http://sintel.is.tue.mpg.de/)|
|2018|ECCV|[Joint Learning of Intrinsic Images and Semantic Segmentation](https://www.ecva.net/papers/eccv_2018/papers_ECCV/html/Anil_Baslamisli_Joint_Learning_of_ECCV_2018_paper.php)|[Project](https://ivi.fnwi.uva.nl/cv/intrinseg)|
|2018|CVPR|[Learning Intrinsic Image Decomposition from Watching the World](https://research.cs.cornell.edu/bigtime/)|[Code](https://github.com/zhengqili/unsupervised-learning-intrinsic-images) / [Dataset](https://research.cs.cornell.edu/bigtime/)|
|2018|CVPR|[Revisiting Deep Intrinsic Image Decompositions](https://arxiv.org/abs/1701.02965)|[Code](https://github.com/fqnchina/IntrinsicImage)|
|2018|ECCV|[Single Image Intrinsic Decomposition without a Single Intrinsic Image](https://openaccess.thecvf.com/content_ECCV_2018/html/Wei-Chiu_Single_Image_Intrinsic_ECCV_2018_paper.html)||
|2018|Pacific Graphics|[Unsupervised Deep Single-Image Intrinsic Decomposition using Illumination-Varying Image Sequences](https://arxiv.org/abs/1803.00805)|[Code](https://github.com/kvanhoey/UnsupervisedIntrinsicDecomposition)|
|2019|ICCV|[GLoSH: Global-Local Spherical Harmonics for Intrinsic Image Decomposition](https://openaccess.thecvf.com/content_ICCV_2019/html/Zhou_GLoSH_Global-Local_Spherical_Harmonics_for_Intrinsic_Image_Decomposition_ICCV_2019_paper.html)||
|2019|CVPR|[InverseRenderNet: Learning single image inverse rendering](https://arxiv.org/abs/1811.12328)|[Code](https://github.com/YeeU/InverseRenderNet) / [Dataset](http://opensurfaces.cs.cornell.edu/publications/intrinsic/)|
|2019|CVPR|[Learning to Separate Multiple Illuminants in a Single Image](https://huizhuo1987.github.io/learningIllum.html)|[Code & Dataset](https://github.com/huizhuo1987/DeepLightSep)|
|2019|ICCV|[Neural Inverse Rendering of an Indoor Scene From a Single Image](https://senguptaumd.github.io/Neural-Inverse-Rendering/)||
|2019|ICCV Workshops (PBDL)|[Single Image Intrinsic Decomposition with Discriminative Feature Encoding](https://openaccess.thecvf.com/content_ICCVW_2019/html/PBDL/Wang_Single_Image_Intrinsic_Decomposition_with_Discriminative_Feature_Encoding_ICCVW_2019_paper.html)||
|2020|CVPR|[Unsupervised Learning for Intrinsic Image Decomposition from a Single Image](https://arxiv.org/abs/1911.09930)|[Code](https://github.com/DreamtaleCore/USI3D)|
|2021|IJCV|[ShadingNet: Image Intrinsics by Fine-Grained Shading Decomposition](https://link.springer.com/article/10.1007/s11263-021-01477-5)|[Code](https://github.com/Morpheus3000/ShadingNet)|
|2022|CVPR|[PIE-Net: Photometric Invariant Edge Guided Network for Intrinsic Image Decomposition](https://openaccess.thecvf.com/content/CVPR2022/papers/Das_PIE-Net_Photometric_Invariant_Edge_Guided_Network_for_Intrinsic_Image_Decomposition_CVPR_2022_paper.pdf)|[Code](https://github.com/Morpheus3000/PIE-Net)|
|2023|TOG|[Intrinsic Image Decomposition via Ordinal Shading](https://yaksoy.github.io/intrinsic/)|[Code](https://github.com/compphoto/Intrinsic) / [Data](https://github.com/compphoto/MIDIntrinsics)|
|2023|CVPR|[Unsupervised Intrinsic Image Decomposition With LiDAR Intensity](https://openaccess.thecvf.com/content/CVPR2023/html/Sato_Unsupervised_Intrinsic_Image_Decomposition_With_LiDAR_Intensity_CVPR_2023_paper.html)||
|2024|TOG / SIGGRAPH Asia|[Colorful Diffuse Intrinsic Image Decomposition in the Wild](https://yaksoy.github.io/ColorfulShading/)|[Code](https://github.com/compphoto/Intrinsic)|
|2024|CVPR|[Intrinsic Image Diffusion for Indoor Single-view Material Estimation](https://openaccess.thecvf.com/content/CVPR2024/html/Kocsis_Intrinsic_Image_Diffusion_for_Indoor_Single-view_Material_Estimation_CVPR_2024_paper.html)||
|2024|SIGGRAPH|[IntrinsicDiffusion: Joint Intrinsic Layers from Latent Diffusion Models](https://intrinsicdiffusion.github.io/)|[Code](https://github.com/JundanLuo/IntrinsicDiffusion)|
|2025|ICLR|[IDArb: Intrinsic Decomposition for Arbitrary Number of Input Views and Illuminations](https://openreview.net/forum?id=uuef1HP6X7)|[Code & Data](https://github.com/Lizb6626/IDArb)|
|2025|WACV|[Unsupervised Single-Image Intrinsic Image Decomposition with LiDAR Intensity Enhanced Training](https://openaccess.thecvf.com/content/WACV2025/html/Sato_Unsupervised_Single-Image_Intrinsic_Image_Decomposition_with_LiDAR_Intensity_Enhanced_Training_WACV_2025_paper.html)||
|2026|CVPR|[ReasonX: MLLM-Guided Intrinsic Image Decomposition](https://openaccess.thecvf.com/content/CVPR2026/html/Dirik_ReasonX_MLLM-Guided_Intrinsic_Image_Decomposition_CVPR_2026_paper.html)||
|2026|CVPR|[VT-Intrinsic: Physics-Based Decomposition of Reflectance and Shading using a Single Visible-Thermal Image Pair](https://openaccess.thecvf.com/content/CVPR2026/html/Yuan_VT-Intrinsic_Physics-Based_Decomposition_of_Reflectance_and_Shading_using_a_Single_CVPR_2026_paper.html)||

## Inverse Rendering (non-DL)

L: Lighting Estimation, G: Geometry Estimation, M: Material Estimation. In the legacy tables, a check indicates an estimated quantity; an empty cell does not assert that the quantity is absent from the pipeline. New entries describe the capture setting directly.

### Material capture

|Year|Pub|Paper|Resources|L|G|M|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|2010|SIGGRAPH|[Manifold bootstrapping for SVBRDF capture](https://dl.acm.org/doi/10.1145/1833349.1778835)|||&#10003;|&#10003;|
|2013|SIGGRAPH|[Practical SVBRDF Capture in the Frequency Domain](https://dl.acm.org/doi/10.1145/2461912.2461978)|||&#10003;|&#10003;|
|2014|SIGGRAPH ASIA|[Appearance-from-Motion: Recovering Spatially Varying Surface Reflectance under Unknown Lighting](http://yuedong.shading.me/project/afm/afm.htm)||&#10003;|&#10003;|&#10003;|
|2015|CGF|[Mobile Surface Reflectometry](https://wp.doc.ic.ac.uk/rgi/project/mobile-surface-reflectometry/)|||&#10003;|&#10003;|
|2015|SIGGRAPH|[Two-Shot SVBRDF Capture for Stationary Materials](https://dl.acm.org/doi/10.1145/2766967)|[Code & Dataset](https://mediatech.aalto.fi/publications/graphics/TwoShotSVBRDF/)||&#10003;|&#10003;|
|2016|SIGGRAPH ASIA|[Recovering Shape and Spatially-Varying Surface Reflectance under Unknown Illumination](https://www.cs.wm.edu/~ppeers/publications/Xia2016RSS/Xia_SIGGRAPHAsia2016.pdf)||&#10003;|&#10003;|&#10003;|
|2016|SIGGRAPH ASIA|[Simultaneous Acquisition of Microscale Reflectance and Normals](http://vclab.kaist.ac.kr/siggraphasia2016p2/index.html)|||&#10003;|&#10003;|
|2017|SIGGRAPH ASIA|[Polarization imaging reflectometry in the wild](https://wp.doc.ic.ac.uk/rgi/project/polarization-imaging-reflectometry-in-the-wild/)|||&#10003;|&#10003;|
|2018|SIGGRAPH ASIA|[Simultaneous Acquisition of Polarimetric SVBRDF and Normals](http://vclab.kaist.ac.kr/siggraphasia2018p2/index.html)|||&#10003;|&#10003;|
|2021|EGSR|[Material and Lighting Reconstruction for Complex Indoor Scenes with Texture-space Differentiable Rendering](https://rgl.epfl.ch/publications/NimierDavid2021Material) ||&#10003;||&#10003;|
|2021|Eurographics|[Progressive Acquisition of SVBRDF and Shape in Motion](http://vclab.kaist.ac.kr/cgf2020/index.html)|||&#10003;|&#10003;|

### Physical models and differentiable optimization

|Year|Pub|Paper|Resources|Focus / capture setting|
|:---:|:---:|:---:|:---:|:---:|
|1999|SIGGRAPH|[Inverse Global Illumination: Recovering Reflectance Models of Real Scenes from Photographs](https://doi.org/10.1145/311535.311559)||Scene reflectance and global illumination|
|2015|TPAMI|[Shape, Illumination, and Reflectance from Shading](https://doi.org/10.1109/TPAMI.2014.2377712)||SIRFS; single-image shape, reflectance and lighting|
|2020|ECCV|[Polarimetric Multi-View Inverse Rendering](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/4522_ECCV_2020_paper.php)||Multi-view geometry/material optimization with polarization|
|2021|EGSR / CGF|[Unified Shape and SVBRDF Recovery using Differentiable Monte Carlo Rendering](https://diglib.eg.org/items/77e4af1c-329a-49ff-b1aa-5dfdf214b708)||Joint mesh and SVBRDF optimization|

### Explicit Gaussian inverse rendering

|Year|Pub|Paper|Resources|Focus / capture setting|
|:---:|:---:|:---:|:---:|:---:|
|2024|CVPR|[GS-IR: 3D Gaussian Splatting for Inverse Rendering](https://openaccess.thecvf.com/content/CVPR2024/html/Liang_GS-IR_3D_Gaussian_Splatting_for_Inverse_Rendering_CVPR_2024_paper.html)|[Code](https://github.com/lzhnb/GS-IR)|Explicit Gaussians; material, lighting and occlusion baking|
|2024|ECCV|[Relightable 3D Gaussians: Realistic Point Cloud Relighting with BRDF Decomposition and Ray Tracing](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/6121_ECCV_2024_paper.php)||Explicit BRDF/light decomposition with point ray tracing|
|2025|CVPR|[Differentiable Inverse Rendering with Interpretable Basis BRDFs](https://openaccess.thecvf.com/content/CVPR2025/html/Chung_Differentiable_Inverse_Rendering_with_Interpretable_Basis_BRDFs_CVPR_2025_paper.html)||Flash capture; explicit Gaussians and basis BRDFs|
|2025|ICCV|[Gaussian Splatting with Discretized SDF for Relightable Assets](https://openaccess.thecvf.com/content/ICCV2025/html/Zhu_Gaussian_Splatting_with_Discretized_SDF_for_Relightable_Assets_ICCV_2025_paper.html)|[Code](https://github.com/NK-CS-ZZL/DiscretizedSDF)|Explicit sampled SDF and Gaussian material parameters|
|2025|ICLR|[GI-GS: Global Illumination Decomposition on Gaussian Splatting for Inverse Rendering](https://openreview.net/forum?id=hJIEtJlvhL)||Explicit Gaussian decomposition with global illumination|
|2025|CVPR|[IRGS: Inter-Reflective Gaussian Splatting with 2D Gaussian Ray Tracing](https://arxiv.org/abs/2412.15867)|[Code](https://github.com/fudan-zvg/IRGS)|2D Gaussian ray tracing; inter-reflections|
|2025|CVPR|[ReCap: Better Gaussian Relighting with Cross-Environment Captures](https://openaccess.thecvf.com/content/CVPR2025/html/Li_ReCap_Better_Gaussian_Relighting_with_Cross-Environment_Captures_CVPR_2025_paper.html)|[Code](https://github.com/jingzhi/ReCap)|Gaussian relighting with cross-environment captures|
|2025|CVPR|[SVG-IR: Spatially-Varying Gaussian Splatting for Inverse Rendering](https://openaccess.thecvf.com/content/CVPR2025/html/Sun_SVG-IR_Spatially-Varying_Gaussian_Splatting_for_Inverse_Rendering_CVPR_2025_paper.html)|[Code](https://github.com/learner-shx/SVG-IR)|Spatially varying Gaussian parameters; indirect illumination|

## Inverse Rendering (DL)

### Image-based estimation and material capture

|Year|Pub|Paper|Resources|L|G|M|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|2016|SIGGRAPH|[Reflectance Modeling by Neural Texture Synthesis](https://mediatech.aalto.fi/publications/graphics/NeuralSVBRDF/)|||&#10003;|&#10003;|
|2017|CVPR|[Deep Outdoor Illumination Estimation](https://arxiv.org/abs/1611.06403)|[Dataset](https://vision.cs.princeton.edu/projects/2012/SUN360/data/)|&#10003;|||
|2017|SIGGRAPH ASIA|[Learning to Predict Indoor Illumination from a Single Image](https://arxiv.org/abs/1704.00090)|[Dataset](http://indoor.hdrdb.com/)|&#10003;|||
|2017|SIGGRAPH|[Modeling Surface Appearance from a Single Photograph using Self-augmented Convolutional Neural Networks](https://arxiv.org/abs/1809.00886)|[Code](https://github.com/msraig/self-augmented-net)||&#10003;|&#10003;|
|2017|ICCV|[Reflectance Capture using Univariate Sampling of BRDFs](https://openaccess.thecvf.com/content_iccv_2017/html/Hui_Reflectance_Capture_Using_ICCV_2017_paper.html)|||&#10003;|&#10003;|
|2018|3DV|[Learning to Estimate Indoor Lighting from 3D Objects](https://arxiv.org/abs/1806.03994)|[Code & Dataset](https://github.com/weberhen/learning_indoor_lighting)|&#10003;|||
|2018|SIGGRAPH ASIA|[Learning to Reconstruct Shape and Spatially-Varying Reflectance from a Single Image](https://cseweb.ucsd.edu/~viscomp/projects/SIGA18ShapeSVBRDF/)|[Code](https://github.com/lzqsd/SingleImageShapeAndSVBRDF) / [Dataset](https://cseweb.ucsd.edu/~viscomp/projects/SIGA18ShapeSVBRDF/)||&#10003;|&#10003;|
|2018|SIGGRAPH ASIA|[Relighting Humans: Occlusion-Aware Inverse Rendering for Full-Body Human Images](http://kanamori.cs.tsukuba.ac.jp/projects/relighting_human/)|[Code & Dataset](http://kanamori.cs.tsukuba.ac.jp/projects/relighting_human/)|&#10003;|&#10003;|&#10003;|
|2018|SIGGRAPH|[Single-Image SVBRDF Capture with a Rendering-Aware Deep Network](https://arxiv.org/abs/1810.09718)|[Code & Dataset](https://repo-sam.inria.fr/fungraph/deep-materials/)||&#10003;|&#10003;|
|2019|CVPR|[All-Weather Deep Outdoor Lighting Estimation](https://lvsn.github.io/allweather/)|[Dataset](http://outdoor.hdrdb.com/)|&#10003;|||
|2019|ICCV|[Deep Parametric Indoor Lighting Estimation](https://lvsn.github.io/deepparametric/)|[Dataset](https://lvsn.github.io/deepparametric/)|&#10003;|||
|2019|CVPR|[DeepLight: Learning Illumination for Unconstrained Mobile Mixed Reality](https://arxiv.org/abs/1904.01175)||&#10003;|||
|2019|CVPR|[Fast Spatially-Varying Indoor Lighting Estimation](https://arxiv.org/abs/1906.03799)|[Dataset](https://lvsn.github.io/fastindoorlight/)|&#10003;||&#10003;|
|2019|CVPR|[Neural Illumination: Lighting Prediction for Indoor Environments](https://illumination.cs.princeton.edu/)|[Dataset](https://niessner.github.io/Matterport/)|&#10003;|&#10003;||
|2020|CVPR|[Inverse Rendering for Complex Indoor Scenes: Shape, Spatially-Varying Lighting and SVBRDF from a Single Image](http://cseweb.ucsd.edu/~viscomp/projects/CVPR20InverseIndoor/)|[Code](https://github.com/lzqsd/InverseRenderingOfIndoorScene) / [Dataset](https://ucsd-openrooms.github.io/)|&#10003;|&#10003;|&#10003;|
|2020|CVPR|[Lighthouse: Predicting Lighting Volumes for Spatially-Coherent Illumination](https://people.eecs.berkeley.edu/~pratul/lighthouse/)|[Code](https://github.com/pratulsrinivasan/lighthouse) / [Dataset](https://interiornet.org/)|&#10003;|||
|2020|SIGGRAPH ASIA|[MaterialGAN: Reflectance Capture using a Generative SVBRDF Model](https://shuangz.com/projects/materialgan-sa20/)|[Code](https://github.com/tflsguoyu/materialgan)||&#10003;|&#10003;|
|2020|ECCV|[Object-Based Illumination Estimation with Rendering-Aware Neural Networks](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123600375.pdf)||&#10003;||&#10003;|
|2020|ECCV|[Single-Shot Neural Relighting and SVBRDF Estimation](https://cseweb.ucsd.edu/~viscomp/projects/ECCV20NeuralRelighting/)|[Code](https://github.com/ssangx/NeuralRelighting) / [Dataset](https://cseweb.ucsd.edu/~viscomp/projects/ECCV20NeuralRelighting/)||&#10003;|&#10003;|
|2021|CVPR|[Deep Polarization Imaging for 3D Shape and SVBRDF Acquisition](https://wp.doc.ic.ac.uk/rgi/project/deep-polarization-3d-imaging/)|[Dataset](https://imperialcollegelondon.app.box.com/s/bbn3t18xostco6rjzr9l7754jb2d22qi)||&#10003;|&#10003;|
|2021|AAAI|[EMLight: Lighting Estimation via Spherical Distribution Approximation](https://arxiv.org/abs/2012.11116) ||&#10003;|||
|2021|SIGGRAPH ASIA|[Generative Modelling of BRDF Textures from Flash Images](https://henzler.github.io/publication/neuralmaterial/)|[Code](https://github.com/henzler/neuralmaterial)||&#10003;|&#10003;|
|2021|SIGGRAPH|[Highlight-Aware Two-Stream Network for Single-Image SVBRDF Acquisition](https://sites.cs.ucsb.edu/~lingqi/publications/paper_highlight.pdf)|||&#10003;|&#10003;|
|2021|ICCV|[Learning Indoor Inverse Rendering with 3D Spatially-Varying Lighting](https://nv-tlabs.github.io/inverse-rendering-3d-lighting/) ||&#10003;|&#10003;||
|2021|CVPR|[PhySG: Inverse Rendering with Spherical Gaussians for Physics-based Material Editing and Relighting](https://kai-46.github.io/PhySG-website/) | [Code](https://github.com/Kai-46/PhySG)|&#10003;|&#10003;|&#10003;|
|2021|CVPR|[Shape and Material Capture at Home](https://openaccess.thecvf.com/content/CVPR2021/html/Lichy_Shape_and_Material_Capture_at_Home_CVPR_2021_paper.html)|[Code & Dataset](https://github.com/dlichy/ShapeAndMaterial)||&#10003;|&#10003;|
|2021|ICCV|[SurfaceNet: Adversarial SVBRDF Estimation from a Single Image](https://openaccess.thecvf.com/content/ICCV2021/html/Vecchio_SurfaceNet_Adversarial_SVBRDF_Estimation_From_a_Single_Image_ICCV_2021_paper.html)|[Code](https://github.com/perceivelab/surfacenet)||&#10003;|&#10003;|
|2022|CVPR|[IRISformer: Dense Vision Transformers for Single-Image Inverse Rendering in Indoor Scenes](https://arxiv.org/abs/2206.08423)| [Code](https://github.com/ViLab-UCSD/IRISformer)|&#10003;|&#10003;|&#10003;|

### Neural fields, multi-view reconstruction and reflectance

|Year|Pub|Paper|Resources|Focus / capture setting|
|:---:|:---:|:---:|:---:|:---:|
|2018|ECCV|[Materials for Masses: SVBRDF Acquisition with a Single Mobile Phone Image](https://www.ecva.net/papers/eccv_2018/papers_ECCV/html/Zhengqin_Li_Materials_for_Masses_ECCV_2018_paper.php)||Single mobile flash image; SVBRDF and normals|
|2020|ECCV|[Deep Reflectance Volumes: Relightable Reconstructions from Multi-View Photometric Images](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/362_ECCV_2020_paper.php)||Co-located-light capture; learned reflectance volumes|
|2020|ECCV|[Invertible Neural BRDF for Object Inverse Rendering](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/4521_ECCV_2020_paper.php)||Known geometry; normalizing-flow BRDF and illumination|
|2021|ICCV|[NeRD: Neural Reflectance Decomposition From Image Collections](https://openaccess.thecvf.com/content/ICCV2021/html/Boss_NeRD_Neural_Reflectance_Decomposition_From_Image_Collections_ICCV_2021_paper.html)|[Code](https://github.com/cgtuebingen/NeRD-Neural-Reflectance-Decomposition)|Multi-view capture under varying unknown lighting|
|2021|SIGGRAPH Asia / TOG|[NeRFactor: Neural Factorization of Shape and Reflectance Under an Unknown Illumination](https://arxiv.org/abs/2106.01970)|[Code](https://github.com/google/nerfactor)|Geometry, BRDF and unknown environment lighting|
|2021|CVPR|[NeRV: Neural Reflectance and Visibility Fields for Relighting and View Synthesis](https://openaccess.thecvf.com/content/CVPR2021/html/Srinivasan_NeRV_Neural_Reflectance_and_Visibility_Fields_for_Relighting_and_View_CVPR_2021_paper.html)||Known-light capture; neural reflectance and visibility|
|2021|NeurIPS|[Neural-PIL: Neural Pre-Integrated Lighting for Reflectance Decomposition](https://proceedings.neurips.cc/paper/2021/file/58ae749f25eded36f486bc85feb3f0ab-Paper.pdf)||Neural pre-integrated lighting; reflectance decomposition|
|2022|CVPR|[Extracting Triangular 3D Models, Materials, and Lighting From Images](https://openaccess.thecvf.com/content/CVPR2022/html/Munkberg_Extracting_Triangular_3D_Models_Materials_and_Lighting_From_Images_CVPR_2022_paper.html)|[Code](https://github.com/NVlabs/nvdiffrec)|nvdiffrec; mesh, material and environment optimization|
|2022|CVPR|[IRON: Inverse Rendering by Optimizing Neural SDFs and Materials From Photometric Images](https://openaccess.thecvf.com/content/CVPR2022/html/Zhang_IRON_Inverse_Rendering_by_Optimizing_Neural_SDFs_and_Materials_From_CVPR_2022_paper.html)||Photometric capture; neural SDF and material textures|
|2022|CVPR|[Modeling Indirect Illumination for Inverse Rendering](https://openaccess.thecvf.com/content/CVPR2022/html/Zhang_Modeling_Indirect_Illumination_for_Inverse_Rendering_CVPR_2022_paper.html)|[Project](https://zju3dv.github.io/invrender/)|InvRender; indirect lighting and visibility|
|2022|ECCV|[NeILF: Neural Incident Light Field for Physically-Based Material Estimation](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/1415_ECCV_2022_paper.php)|[Code](https://github.com/apple/ml-neilf)|Known geometry; neural incident light and material fields|
|2022|SIGGRAPH / TOG|[NeROIC: Neural Rendering of Objects from Online Image Collections](https://mlchai.com/publication/kuang2022neroic/)|[Code](https://github.com/snap-research/NeROIC)|Online image collections; geometry, appearance and lighting|
|2022|ECCV|[Neural Radiance Transfer Fields for Relightable Novel-View Synthesis with Global Illumination](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/6143_ECCV_2022_paper.php)||Relightable neural transport with global illumination|
|2022|ECCV|[PS-NeRF: Neural Inverse Rendering for Multi-View Photometric Stereo](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/1832_ECCV_2022_paper.php)|[Project](https://ywq.github.io/psnerf)|Multi-view photometric stereo; shape, materials and lights|
|2022|NeurIPS|[SAMURAI: Shape And Material from Unconstrained Real-world Arbitrary Image collections](https://papers.neurips.cc/paper_files/paper/2022/hash/a8f2713b5c6bdcd3d264f1aa9b9c6f03-Abstract-Conference.html)||Unconstrained image collections; shape and material|
|2022|NeurIPS|[Shape, Light, and Material Decomposition from Images using Monte Carlo Rendering and Denoising](https://papers.neurips.cc/paper_files/paper/2022/hash/8fcb27984bf16ca03cad643244ec470d-Abstract-Conference.html)|[Code](https://github.com/NVlabs/nvdiffrecmc)|nvdiffrecmc; differentiable path tracing and denoising|
|2023|CVPR|[DANI-Net: Uncalibrated Photometric Stereo by Differentiable Shadow Handling, Anisotropic Reflectance Modeling, and Neural Inverse Rendering](https://openaccess.thecvf.com/content/CVPR2023/html/Li_DANI-Net_Uncalibrated_Photometric_Stereo_by_Differentiable_Shadow_Handling_Anisotropic_Reflectance_CVPR_2023_paper.html)||Uncalibrated photometric stereo; shadows and anisotropy|
|2023|ICCV|[Factorized Inverse Path Tracing for Efficient and Accurate Material-Lighting Estimation](https://openaccess.thecvf.com/content/ICCV2023/html/Wu_Factorized_Inverse_Path_Tracing_for_Efficient_and_Accurate_Material-Lighting_Estimation_ICCV_2023_paper.html)|[Code](https://github.com/lwwu2/fipt)|Known geometry; material and lighting via factored transport|
|2023|CVPR|[I2-SDF: Intrinsic Indoor Scene Reconstruction and Editing via Raytracing in Neural SDFs](https://openaccess.thecvf.com/content/CVPR2023/html/Zhu_I2-SDF_Intrinsic_Indoor_Scene_Reconstruction_and_Editing_via_Raytracing_in_CVPR_2023_paper.html)|[Project](https://jingsenzhu.github.io/i2-sdf)|Indoor neural SDF, material and radiance reconstruction|
|2023|ICCV|[IntrinsicNeRF: Learning Intrinsic Neural Radiance Fields for Editable Novel View Synthesis](https://openaccess.thecvf.com/content/ICCV2023/html/Ye_IntrinsicNeRF_Learning_Intrinsic_Neural_Radiance_Fields_for_Editable_Novel_View_ICCV_2023_paper.html)||Room-scale albedo/shading decomposition in NeRF|
|2023|CVPR|[Inverse Rendering of Translucent Objects Using Physical and Neural Renderers](https://openaccess.thecvf.com/content/CVPR2023/html/Li_Inverse_Rendering_of_Translucent_Objects_Using_Physical_and_Neural_Renderers_CVPR_2023_paper.html)||Flash/no-flash capture; shape and subsurface scattering|
|2023|CVPR|[MAIR: Multi-View Attention Inverse Rendering With 3D Spatially-Varying Lighting Estimation](https://openaccess.thecvf.com/content/CVPR2023/html/Choi_MAIR_Multi-View_Attention_Inverse_Rendering_With_3D_Spatially-Varying_Lighting_Estimation_CVPR_2023_paper.html)||Multi-view indoor geometry, SVBRDF and spatial lighting|
|2023|CVPR|[Multi-View Inverse Rendering for Large-Scale Real-World Indoor Scenes](https://openaccess.thecvf.com/content/CVPR2023/html/Li_Multi-View_Inverse_Rendering_for_Large-Scale_Real-World_Indoor_Scenes_CVPR_2023_paper.html)|[Project](https://lzleejean.github.io/TexIR)|TexIR; texture-based lighting and neural material fields|
|2023|CVPR|[NeFII: Inverse Rendering for Reflectance Decomposition With Near-Field Indirect Illumination](https://openaccess.thecvf.com/content/CVPR2023/html/Wu_NeFII_Inverse_Rendering_for_Reflectance_Decomposition_With_Near-Field_Indirect_Illumination_CVPR_2023_paper.html)||Neural radiance cache for near-field indirect lighting|
|2023|ICCV|[NeILF++: Inter-Reflectable Light Fields for Geometry and Material Estimation](https://openaccess.thecvf.com/content/ICCV2023/html/Zhang_NeILF_Inter-Reflectable_Light_Fields_for_Geometry_and_Material_Estimation_ICCV_2023_paper.html)|[Code](https://github.com/apple/ml-neilfpp)|Joint geometry, material and inter-reflectable light fields|
|2023|ICCV|[NEMTO: Neural Environment Matting for Novel View and Relighting Synthesis of Transparent Objects](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_NEMTO_Neural_Environment_Matting_for_Novel_View_and_Relighting_Synthesis_ICCV_2023_paper.html)||Transparent objects; environment matting and relighting|
|2023|SIGGRAPH|[NeRO: Neural Geometry and BRDF Reconstruction of Reflective Objects from Multiview Images](https://liuyuan-pal.github.io/NeRO/)||Reflective objects; geometry, BRDF and lighting|
|2023|CVPR|[Neural Fields Meet Explicit Geometric Representations for Inverse Rendering of Urban Scenes](https://openaccess.thecvf.com/content/CVPR2023/html/Wang_Neural_Fields_Meet_Explicit_Geometric_Representations_for_Inverse_Rendering_of_CVPR_2023_paper.html)||Urban scenes; neural geometry and mesh light transport|
|2023|ICCV|[Neural Microfacet Fields for Inverse Rendering](https://openaccess.thecvf.com/content/ICCV2023/html/Mai_Neural_Microfacet_Fields_for_Inverse_Rendering_ICCV_2023_paper.html)||Neural microfacet reflectance and geometry|
|2023|SIGGRAPH|[Relighting Neural Radiance Fields with Shadow and Highlight Hints](https://nrhints.github.io/)|[Code](https://github.com/iamNCJ/NRHints)|Moving-light capture; shadows and highlights constrain reflectance|
|2023|ICCV|[ReNeRF: Relightable Neural Radiance Fields with Nearfield Lighting](https://openaccess.thecvf.com/content/ICCV2023/html/Xu_ReNeRF_Relightable_Neural_Radiance_Fields_with_Nearfield_Lighting_ICCV_2023_paper.html)||Near-field lighting and relightable neural fields|
|2023|CVPR|[TensoIR: Tensorial Inverse Rendering](https://openaccess.thecvf.com/content/CVPR2023/html/Jin_TensoIR_Tensorial_Inverse_Rendering_CVPR_2023_paper.html)||Tensor-factorized geometry, reflectance and illumination|
|2023|CVPR|[UMat: Uncertainty-Aware Single Image High Resolution Material Capture](https://openaccess.thecvf.com/content/CVPR2023/html/Rodriguez-Pardo_UMat_Uncertainty-Aware_Single_Image_High_Resolution_Material_Capture_CVPR_2023_paper.html)||Single diffuse image; normals, specularity and roughness|
|2023|CVPR|[WildLight: In-the-Wild Inverse Rendering With a Flashlight](https://openaccess.thecvf.com/content/CVPR2023/html/Cheng_WildLight_In-the-Wild_Inverse_Rendering_With_a_Flashlight_CVPR_2023_paper.html)|[Code](https://github.com/za-cheng/WildLight)|Smartphone flashlight capture; neural shape and reflectance|
|2024|ECCV|[Flash Cache: Reducing Bias in Radiance Cache Based Inverse Rendering](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/3991_ECCV_2024_paper.php)||Low-bias neural radiance caching for inverse rendering|
|2024|ECCV|[IntrinsicAnything: Learning Diffusion Priors for Inverse Rendering Under Unknown Illumination](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/7782_ECCV_2024_paper.php)|[Project](https://zju3dv.github.io/IntrinsicAnything/)|Diffusion material priors for unknown-light reconstruction|
|2024|CVPR|[Inverse Rendering of Glossy Objects via the Neural Plenoptic Function and Radiance Fields](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_Inverse_Rendering_of_Glossy_Objects_via_the_Neural_Plenoptic_Function_CVPR_2024_paper.html)|[Project](https://whyy.site/paper/nep)|Neural plenoptic function for local light interactions|
|2024|CVPR|[NeISF: Neural Incident Stokes Field for Geometry and Material Estimation](https://openaccess.thecvf.com/content/CVPR2024/html/Li_NeISF_Neural_Incident_Stokes_Field_for_Geometry_and_Material_Estimation_CVPR_2024_paper.html)||Polarized inverse rendering; neural incident Stokes field|
|2024|ECCV|[Photorealistic Object Insertion with Diffusion-Guided Inverse Rendering](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/7871_ECCV_2024_paper.php)||Diffusion-guided inverse rendering for image compositing|
|2024|3DV|[Physics-based Indirect Illumination for Inverse Rendering](https://denghilbert.github.io/pii/)|[Code](https://github.com/denghilbert/3DV2024-Physics-based-Indirect-Illumination-for-Inverse-Rendering)|Multi-view geometry, materials and indirect lighting|
|2024|CVPR|[SHINOBI: Shape and Illumination using Neural Object Decomposition via BRDF Optimization In-the-wild](https://openaccess.thecvf.com/content/CVPR2024/html/Engelhardt_SHINOBI_Shape_and_Illumination_using_Neural_Object_Decomposition_via_BRDF_CVPR_2024_paper.html)||Unconstrained images; pose, shape, material and lighting|
|2024|SIGGRAPH / TOG|[TensoSDF: Roughness-aware Tensorial Representation for Robust Geometry and Material Reconstruction](https://riga2.github.io/tensosdf/)||Tensorial SDF; roughness-aware geometry and material|
|2024|ECCV|[UniVoxel: Fast Inverse Rendering by Unified Voxelization of Scene Representation](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/9015_ECCV_2024_paper.php)|[Code](https://github.com/freemantom/UniVoxel)|Voxel geometry/material and neural illumination|
|2024|CVPR|[VMINer: Versatile Multi-view Inverse Rendering with Near- and Far-field Light Sources](https://openaccess.thecvf.com/content/CVPR2024/html/Fei_VMINer_Versatile_Multi-view_Inverse_Rendering_with_Near-_and_Far-field_Light_CVPR_2024_paper.html)||Near- and far-field lighting; neural/surface rendering|
|2025|ICCV|[InvRGB+L: Inverse Rendering of Complex Scenes with Unified Color and LiDAR Reflectance Modeling](https://openaccess.thecvf.com/content/ICCV2025/html/Chen_InvRGBL_Inverse_Rendering_of_Complex_Scenes_with_Unified_Color_and_ICCV_2025_paper.html)||RGB and LiDAR reflectance; large relightable scenes|
|2025|CVPR|[IRIS: Inverse Rendering of Indoor Scenes from Low Dynamic Range Images](https://openaccess.thecvf.com/content/CVPR2025/html/Lin_IRIS_Inverse_Rendering_of_Indoor_Scenes_from_Low_Dynamic_Range_CVPR_2025_paper.html)||Indoor material, HDR lighting and camera response|
|2025|CVPR|[LIRM: Large Inverse Rendering Model for Progressive Reconstruction of Shape, Materials and View-dependent Radiance Fields](https://openaccess.thecvf.com/content/CVPR2025/html/Li_LIRM_Large_Inverse_Rendering_Model_for_Progressive_Reconstruction_of_Shape_CVPR_2025_paper.html)||Feed-forward hexa-plane shape and material reconstruction|
|2025|CVPR|[NeISF++: Neural Incident Stokes Field for Polarized Inverse Rendering of Conductors and Dielectrics](https://openaccess.thecvf.com/content/CVPR2025/html/Li_NeISF_Neural_Incident_Stokes_Field_for_Polarized_Inverse_Rendering_of_CVPR_2025_paper.html)||Polarized capture; conductors and dielectrics|
|2025|CVPR|[PBR-NeRF: Inverse Rendering with Physics-Based Neural Fields](https://openaccess.thecvf.com/content/CVPR2025/html/Wu_PBR-NeRF_Inverse_Rendering_with_Physics-Based_Neural_Fields_CVPR_2025_paper.html)|[Code](https://github.com/s3anwu/pbrnerf)|Joint geometry, materials and lighting; physical priors|
|2025|CVPR|[TensoFlow: Tensorial Flow-based Sampler for Inverse Rendering](https://openaccess.thecvf.com/content/CVPR2025/html/Gu_TensoFlow_Tensorial_Flow-based_Sampler_for_Inverse_Rendering_CVPR_2025_paper.html)||Learned normalizing-flow importance sampling|

### Image and video decomposition, diffusion and material priors

|Year|Pub|Paper|Resources|Focus / capture setting|
|:---:|:---:|:---:|:---:|:---:|
|2022|CVPR|[PhyIR: Physics-Based Inverse Rendering for Panoramic Indoor Images](https://openaccess.thecvf.com/content/CVPR2022/html/Li_PhyIR_Physics-Based_Inverse_Rendering_for_Panoramic_Indoor_Images_CVPR_2022_paper.html)||Panoramic indoor geometry, SVBRDF and lighting|
|2024|CVPR|[Diffusion Reflectance Map: Single-Image Stochastic Inverse Rendering of Illumination and Reflectance](https://openaccess.thecvf.com/content/CVPR2024/html/Enyo_Diffusion_Reflectance_Map_Single-Image_Stochastic_Inverse_Rendering_of_Illumination_and_CVPR_2024_paper.html)||Single-image stochastic illumination and reflectance|
|2024|ECCV|[MERLiN: Single-Shot Material Estimation and Relighting for Photometric Stereo](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/1894_ECCV_2024_paper.php)||Single-image material estimation and photometric relighting|
|2024|SIGGRAPH|[RGB↔X: Image Decomposition and Synthesis Using Material- and Lighting-aware Diffusion Models](https://zheng95z.github.io/publications/rgbx24.html)|[Code](https://github.com/zheng95z/rgbx)|Image-space intrinsic channels and conditional synthesis|
|2025|CVPR|[Channel-wise Noise Scheduled Diffusion for Inverse Rendering in Indoor Scenes](https://openaccess.thecvf.com/content/CVPR2025/html/Choi_Channel-wise_Noise_Scheduled_Diffusion_for_Inverse_Rendering_in_Indoor_Scenes_CVPR_2025_paper.html)||Single-image geometry, material and lighting diffusion|
|2025|CVPR|[DiffusionRenderer: Neural Inverse and Forward Rendering with Video Diffusion Models](https://research.nvidia.com/labs/toronto-ai/DiffusionRenderer/)|[Code](https://github.com/nv-tlabs/diffusion-renderer)|Video diffusion for inverse and forward rendering|
|2025|ICCV|[DNF-Intrinsic: Deterministic Noise-Free Diffusion for Indoor Inverse Rendering](https://openaccess.thecvf.com/content/ICCV2025/html/Zheng_DNF-Intrinsic_Deterministic_Noise-Free_Diffusion_for_Indoor_Inverse_Rendering_ICCV_2025_paper.html)|[Code](https://github.com/OnlyZZZZ/DNF-Intrinsic)|Deterministic diffusion/flow intrinsic prediction|
|2025|CVPR|[Neural LightRig: Unlocking Accurate Object Normal and Material Estimation with Multi-Light Diffusion](https://openaccess.thecvf.com/content/CVPR2025/html/He_Neural_LightRig_Unlocking_Accurate_Object_Normal_and_Material_Estimation_with_CVPR_2025_paper.html)|[Project](https://projects.zxhezexin.com/neural-lightrig)|Multi-light diffusion priors; normal and material maps|
|2025|ICCV|[Ouroboros: Single-step Diffusion Models for Cycle-consistent Forward and Inverse Rendering](https://openaccess.thecvf.com/content/ICCV2025/html/Sun_Ouroboros_Single-step_Diffusion_Models_for_Cycle-consistent_Forward_and_Inverse_Rendering_ICCV_2025_paper.html)||Cycle-consistent single-step forward/inverse diffusion|
|2025|ICCV|[SuperMat: Physically Consistent PBR Material Estimation at Interactive Rates](https://openaccess.thecvf.com/content/ICCV2025/html/Hong_SuperMat_Physically_Consistent_PBR_Material_Estimation_at_Interactive_Rates_ICCV_2025_paper.html)|[Project](https://hyj542682306.github.io/SuperMat/)|Single-step diffusion; albedo, metallic and roughness|
|2025|CVPR|[Uni-Renderer: Unifying Rendering and Inverse Rendering Via Dual Stream Diffusion](https://openaccess.thecvf.com/content/CVPR2025/html/Chen_Uni-Renderer_Unifying_Rendering_and_Inverse_Rendering_Via_Dual_Stream_Diffusion_CVPR_2025_paper.html)||Dual-stream forward and inverse rendering diffusion|
|2026|CVPR|[Intrinsic Image Fusion for Multi-View 3D Material Reconstruction](https://openaccess.thecvf.com/content/CVPR2026/html/Kocsis_Intrinsic_Image_Fusion_for_Multi-View_3D_Material_Reconstruction_CVPR_2026_paper.html)||Diffusion material priors fused across views|
|2026|CVPR|[MatMart: Material Reconstruction of 3D Objects via Diffusion](https://openaccess.thecvf.com/content/CVPR2026/html/Wu_MatMart_Material_Reconstruction_of_3D_Objects_via_Diffusion_CVPR_2026_paper.html)||Multi-view material reconstruction with diffusion priors|
|2026|CVPR|[MVInverse: Feed-forward Multiview Inverse Rendering in Seconds](https://openaccess.thecvf.com/content/CVPR2026/html/Wu_MVInverse_Feed-forward_Multiview_Inverse_Rendering_in_Seconds_CVPR_2026_paper.html)||Feed-forward multi-view normals, materials and diffuse shading|
|2026|CVPR|[V-RGBX: Video Editing with Accurate Controls over Intrinsic Properties](https://openaccess.thecvf.com/content/CVPR2026/html/Fang_V-RGBX_Video_Editing_with_Accurate_Controls_over_Intrinsic_Properties_CVPR_2026_paper.html)||Video intrinsic decomposition and controlled synthesis|

### Lighting estimation and HDR environments

|Year|Pub|Paper|Resources|Focus / capture setting|
|:---:|:---:|:---:|:---:|:---:|
|2020|ECCV|[PointAR: Efficient Lighting Estimation for Mobile Augmented Reality](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/4405_ECCV_2020_paper.php)||RGB-D-conditioned mobile lighting estimation|
|2022|ECCV|[Editable Indoor Lighting Estimation](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/2772_ECCV_2022_paper.php)||Parametric lights and high-frequency illumination texture|
|2022|ECCV|[StyleLight: HDR Panorama Generation for Lighting Estimation and Editing](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/2378_ECCV_2022_paper.php)|[Project](https://style-light.github.io/)|Single-image HDR panorama lighting estimation/editing|
|2023|ICCV|[EverLight: Indoor-Outdoor Editable HDR Lighting Estimation](https://openaccess.thecvf.com/content/ICCV2023/html/Dastjerdi_EverLight_Indoor-Outdoor_Editable_HDR_Lighting_Estimation_ICCV_2023_paper.html)||Editable indoor/outdoor HDR illumination|
|2024|CVPR|[LightOctree: Lightweight 3D Spatially-Coherent Indoor Lighting Estimation](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_LightOctree_Lightweight_3D_Spatially-Coherent_Indoor_Lighting_Estimation_CVPR_2024_paper.html)||Octree-based spatially varying indoor lighting|
|2026|CVPR|[Lighting in Motion: Spatiotemporal HDR Lighting Estimation](https://openaccess.thecvf.com/content/CVPR2026/html/Bolduc_Lighting_in_Motion_Spatiotemporal_HDR_Lighting_Estimation_CVPR_2026_paper.html)||Spatiotemporal HDR environment lighting from diffusion|

### Human and face inverse rendering

|Year|Pub|Paper|Resources|Focus / capture setting|
|:---:|:---:|:---:|:---:|:---:|
|2018|CVPR|[SfSNet: Learning Shape, Reflectance and Illuminance of Faces 'in the Wild'](https://openaccess.thecvf.com/content_cvpr_2018/html/Sengupta_SfSNet_Learning_Shape_CVPR_2018_paper.html)||Single-face albedo, normals and illumination|
|2022|ECCV|[Geometry-Aware Single-Image Full-Body Human Relighting](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4385_ECCV_2022_paper.php)||Full-body relighting with geometry and neural rendering|
|2024|CVPR|[Artist-Friendly Relightable and Animatable Neural Heads](https://openaccess.thecvf.com/content/CVPR2024/html/Xu_Artist-Friendly_Relightable_and_Animatable_Neural_Heads_CVPR_2024_paper.html)||Relightable and animatable neural head reconstruction|
|2024|CVPR|[IntrinsicAvatar: Physically Based Inverse Rendering of Dynamic Humans from Monocular Videos via Explicit Ray Tracing](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_IntrinsicAvatar_Physically_Based_Inverse_Rendering_of_Dynamic_Humans_from_Monocular_CVPR_2024_paper.html)||Monocular dynamic humans; physically based ray tracing|
|2024|CVPR|[Monocular Identity-Conditioned Facial Reflectance Reconstruction](https://openaccess.thecvf.com/content/CVPR2024/html/Ren_Monocular_Identity-Conditioned_Facial_Reflectance_Reconstruction_CVPR_2024_paper.html)||Identity-conditioned face reflectance reconstruction|
|2025|CVPR|[Comprehensive Relighting: Generalizable and Consistent Monocular Human Relighting and Harmonization](https://openaccess.thecvf.com/content/CVPR2025/html/Wang_Comprehensive_Relighting_Generalizable_and_Consistent_Monocular_Human_Relighting_and_Harmonization_CVPR_2025_paper.html)||Generalizable monocular human relighting and harmonization|
|2025|CVPR|[GroomLight: Hybrid Inverse Rendering for Relightable Human Hair Appearance Modeling](https://openaccess.thecvf.com/content/CVPR2025/html/Zheng_GroomLight_Hybrid_Inverse_Rendering_for_Relightable_Human_Hair_Appearance_Modeling_CVPR_2025_paper.html)|[Project](https://syntec-research.github.io/GroomLight)|Hair BSDF and learned light-aware residual|
|2025|CVPR|[S^3-Face: SSS-Compliant Facial Reflectance Estimation via Diffusion Priors](https://openaccess.thecvf.com/content/CVPR2025/html/Ren_S3-Face_SSS-Compliant_Facial_Reflectance_Estimation_via_Diffusion_Priors_CVPR_2025_paper.html)||Self-supervised face shape, shading and reflectance|
|2026|CVPR|[WildCap: Facial Albedo Capture in the Wild via Hybrid Inverse Rendering](https://openaccess.thecvf.com/content/CVPR2026/html/Han_WildCap_Facial_Albedo_Capture_in_the_Wild_via_Hybrid_Inverse_CVPR_2026_paper.html)||Smartphone facial albedo capture; learned and physical priors|

### Gaussian methods with neural components

|Year|Pub|Paper|Resources|Focus / capture setting|
|:---:|:---:|:---:|:---:|:---:|
|2025|ICCV|[GaRe: Relightable 3D Gaussian Splatting for Outdoor Scenes from Unconstrained Photo Collections](https://openaccess.thecvf.com/content/ICCV2025/html/Bai_GaRe_Relightable_3D_Gaussian_Splatting_for_Outdoor_Scenes_from_Unconstrained_ICCV_2025_paper.html)||Outdoor Gaussians with learned intrinsic decomposition|
|2025|ICCV|[GeoSplatting: Towards Geometry Guided Gaussian Splatting for Physically-based Inverse Rendering](https://openaccess.thecvf.com/content/ICCV2025/html/Ye_GeoSplatting_Towards_Geometry_Guided_Gaussian_Splatting_for_Physically-based_Inverse_Rendering_ICCV_2025_paper.html)|[Code](https://github.com/PKU-VCL-Geometry/GeoSplatting)|Neural material representation and mesh-guided Gaussians|
|2025|WACV|[LumiGauss: Relightable Gaussian Splatting in the Wild](https://openaccess.thecvf.com/content/WACV2025/html/Kaleta_LumiGauss_Relightable_Gaussian_Splatting_in_the_Wild_WACV_2025_paper.html)|[Code](https://github.com/joaxkal/lumigauss)|Explicit Gaussians with MLP-predicted SH lighting|
|2025|CVPR|[RNG: Relightable Neural Gaussians](https://openaccess.thecvf.com/content/CVPR2025/html/Fan_RNG_Relightable_Neural_Gaussians_CVPR_2025_paper.html)||Light-conditioned neural Gaussians; learned shading|
|2025|ICCV|[SU-RGS: Relightable 3D Gaussian Splatting from Sparse Views under Unconstrained Illuminations](https://openaccess.thecvf.com/content/ICCV2025/html/Zhang_SU-RGS_Relightable_3D_Gaussian_Splatting_from_Sparse_Views_under_Unconstrained_ICCV_2025_paper.html)||Sparse-view decomposition with pretrained semantic supervision|
|2026|CVPR|[GHPT: Real-Time Relightable Gaussian Splatting using Hybrid Path Tracing](https://openaccess.thecvf.com/content/CVPR2026/html/Bo_GHPT_Real-Time_Relightable_Gaussian_Splatting_using_Hybrid_Path_Tracing_CVPR_2026_paper.html)||Gaussian/mesh path tracing; pretrained normal supervision|
|2026|CVPR|[IR-HGP: Physically-Aware Gaussian Inverse Rendering for High-Illumination Scenes via Generative Priors](https://openaccess.thecvf.com/content/CVPR2026/html/Zhang_IR-HGP_Physically-Aware_Gaussian_Inverse_Rendering_for_High-Illumination_Scenes_via_Generative_CVPR_2026_paper.html)||Gaussian inverse rendering with generative lighting priors|
|2026|CVPR|[LumiMotion: Improving Gaussian Relighting with Scene Dynamics](https://openaccess.thecvf.com/content/CVPR2026/html/Kaleta_LumiMotion_Improving_Gaussian_Relighting_with_Scene_Dynamics_CVPR_2026_paper.html)|[Code](https://github.com/joaxkal/LumiMotion)|Dynamic Gaussians with learned deformation; material/light separation|
|2026|CVPR|[MatSpray: Fusing 2D Material World Knowledge on 3D Geometry](https://openaccess.thecvf.com/content/CVPR2026/html/Langsteiner_MatSpray_Fusing_2D_Material_World_Knowledge_on_3D_Geometry_CVPR_2026_paper.html)|[Code](https://github.com/cgtuebingen/MatSpray)|Diffusion material maps fused on Gaussians by a neural merger|
|2026|CVPR|[SGS-Intrinsic: Semantic-Invariant Gaussian Splatting for Sparse-View Indoor Inverse Rendering](https://openaccess.thecvf.com/content/CVPR2026/html/Niu_SGS-Intrinsic_Semantic-Invariant_Gaussian_Splatting_for_Sparse-View_Indoor_Inverse_Rendering_CVPR_2026_paper.html)|[Project](https://github.com/GrumpySloths/SGS_Intrinsic.github.io)|Sparse-view indoor decomposition with semantic priors|
|2026|WACV|[Spec-Gloss Surfels and Normal-Diffuse Priors for Relightable Glossy Objects](https://openaccess.thecvf.com/content/WACV2026/html/Kouros_Spec-Gloss_Surfels_and_Normal-Diffuse_Priors_for_Relightable_Glossy_Objects_WACV_2026_paper.html)||Glossy surfels with learned normal/diffuse priors|

### Scene and video relighting

|Year|Pub|Paper|Resources|Focus / capture setting|
|:---:|:---:|:---:|:---:|:---:|
|2020|ECCV|[Learning to Factorize and Relight a City](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/2473_ECCV_2020_paper.php)||Outdoor time-varying illumination and permanent factors|
|2020|ECCV|[Self-supervised Outdoor Scene Relighting](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/3937_ECCV_2020_paper.php)||Self-supervised albedo, geometry, lighting and relighting|
|2021|CVPR Workshops (NTIRE)|[Physically Inspired Dense Fusion Networks for Relighting](https://openaccess.thecvf.com/content/CVPR2021W/NTIRE/html/Yazdani_Physically_Inspired_Dense_Fusion_Networks_for_Relighting_CVPRW_2021_paper.html)||Depth-guided image relighting with intrinsic decomposition|
|2022|ECCV|[NeRF for Outdoor Scene Relighting](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4998_ECCV_2022_paper.php)||NeRF-OSR; outdoor illumination and viewpoint editing|
|2023|CVPR|[Complementary Intrinsics From Neural Radiance Fields and CNNs for Outdoor Scene Relighting](https://openaccess.thecvf.com/content/CVPR2023/html/Yang_Complementary_Intrinsics_From_Neural_Radiance_Fields_and_CNNs_for_Outdoor_CVPR_2023_paper.html)||Outdoor relighting; CNN and NeRF intrinsic estimates|
|2023|CVPR|[Weakly-Supervised Single-View Image Relighting](https://openaccess.thecvf.com/content/CVPR2023/html/Yi_Weakly-Supervised_Single-View_Image_Relighting_CVPR_2023_paper.html)|[Project](https://renjiaoyi.github.io/relighting/)|Single-view image relighting with weak supervision|
|2024|WACV|[Fast Sun-Aligned Outdoor Scene Relighting Based on TensoRF](https://openaccess.thecvf.com/content/WACV2024/html/Chang_Fast_Sun-Aligned_Outdoor_Scene_Relighting_Based_on_TensoRF_WACV_2024_paper.html)||Outdoor TensoRF relighting with sun alignment|
|2024|ECCV|[The Sky's the Limit: Relightable Outdoor Scenes via a Sky-pixel Constrained Illumination Prior and Outside-In Visibility](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/7067_ECCV_2024_paper.php)|[Code](https://github.com/JADGardner/neusky)|Outdoor relighting; sky-constrained illumination and visibility|
|2025|ICCV|[Light-A-Video: Training-free Video Relighting via Progressive Light Fusion](https://openaccess.thecvf.com/content/ICCV2025/html/Zhou_Light-A-Video_Training-free_Video_Relighting_via_Progressive_Light_Fusion_ICCV_2025_paper.html)||Pretrained diffusion models; temporally consistent relighting|
|2025|ICCV|[LightSwitch: Multi-view Relighting with Material-guided Diffusion](https://openaccess.thecvf.com/content/ICCV2025/html/Litman_LightSwitch_Multi-view_Relighting_with_Material-guided_Diffusion_ICCV_2025_paper.html)||Multi-view material-guided diffusion relighting|
|2025|CVPR|[LumiNet: Latent Intrinsics Meets Diffusion Models for Indoor Scene Relighting](https://openaccess.thecvf.com/content/CVPR2025/html/Xing_LumiNet_Latent_Intrinsics_Meets_Diffusion_Models_for_Indoor_Scene_Relighting_CVPR_2025_paper.html)||Latent intrinsics for indoor image relighting|
|2025|SIGGRAPH|[Physically Controllable Relighting of Photographs](https://yaksoy.github.io/PhysicalRelighting/)||Single-image relighting using intrinsic and geometric predictions|
|2026|CVPR|[FlowPortal: Residual-Corrected Flow for Training-Free Video Relighting and Background Replacement](https://openaccess.thecvf.com/content/CVPR2026/html/Gao_FlowPortal_Residual-Corrected_Flow_for_Training-Free_Video_Relighting_and_Background_Replacement_CVPR_2026_paper.html)||Pretrained flow-model video relighting and background replacement|

## Portrait Relighting (DL)

|Year|Pub|Paper|Resources|
|:---:|:---:|:---:|:---:|
|2019|ICCV|[Deep Single-Image Portrait Relighting](https://openaccess.thecvf.com/content_ICCV_2019/html/Zhou_Deep_Single-Image_Portrait_Relighting_ICCV_2019_paper.html)|[Code](https://github.com/zhhoper/DPR) / [Data preparation](https://github.com/zhhoper/RI_render_DPR)|
|2019|SIGGRAPH|[Single Image Portrait Relighting](https://arxiv.org/abs/1905.00824)||
|2020|CVPR|[Learning Physics-Guided Face Relighting Under Directional Light](https://openaccess.thecvf.com/content_CVPR_2020/html/Nestmeyer_Learning_Physics-Guided_Face_Relighting_Under_Directional_Light_CVPR_2020_paper.html)||
|2020|SIGGRAPH Asia / TOG|[Light Stage Super-Resolution: Continuous High-Frequency Relighting](https://cseweb.ucsd.edu/~viscomp/projects/SIGA20LightstageSuperres/)||
|2020|TOG|[Single Image Portrait Relighting via Explicit Multiple Reflectance Channel Modeling](https://dl.acm.org/doi/abs/10.1145/3414685.3417824)|[Dataset](https://sireer.github.io/projects/FLM_project/)|
|2021|SIGGRAPH|[Learning to Relight Portraits for Background Replacement](https://augmentedperception.github.io/total_relighting/)||
|2021|CVPR|[Monocular Reconstruction of Neural Face Reflectance Fields](https://arxiv.org/abs/2008.10247)||
|2021|ICCV|[Neural Video Portrait Relighting in Real-time via Consistency Modeling](https://zhanglongwen.com/projects/nvpr/)|[Code](https://github.com/ZoneLikeWonderland/Neural-Video-Portrait-Relighting-in-Real-time-via-Consistency-Modeling) / [Dataset](https://zhanglongwen.com/projects/nvpr/dataset.html)|
|2021|WACV|[Relighting Images in the Wild with a Self-Supervised Siamese Auto-Encoder](https://openaccess.thecvf.com/content/WACV2021/html/Liu_Relighting_Images_in_the_Wild_With_a_Self-Supervised_Siamese_Auto-Encoder_WACV_2021_paper.html)||
|2022|CVPR|[Face Relighting With Geometrically Consistent Shadows](https://openaccess.thecvf.com/content/CVPR2022/html/Hou_Face_Relighting_With_Geometrically_Consistent_Shadows_CVPR_2022_paper.html)||
|2022|WACV Workshops (WACI)|[Temporally Consistent Relighting for Portrait Videos](https://openaccess.thecvf.com/content/WACV2022W/WACI/html/Chandran_Temporally_Consistent_Relighting_for_Portrait_Videos_WACVW_2022_paper.html)||
|2023|ICCV|[DiFaReli: Diffusion Face Relighting](https://openaccess.thecvf.com/content/ICCV2023/html/Ponglertnapakorn_DiFaReli_Diffusion_Face_Relighting_ICCV_2023_paper.html)|[Project](https://diffusion-face-relighting.github.io)|
|2023|CVPR|[FaceLit: Neural 3D Relightable Faces](https://openaccess.thecvf.com/content/CVPR2023/html/Ranjan_FaceLit_Neural_3D_Relightable_Faces_CVPR_2023_paper.html)||
|2023|CVPR|[LightPainter: Interactive Portrait Relighting With Freehand Scribble](https://openaccess.thecvf.com/content/CVPR2023/html/Mei_LightPainter_Interactive_Portrait_Relighting_With_Freehand_Scribble_CVPR_2023_paper.html)||
|2023|ICCV|[Relightify: Relightable 3D Faces from a Single Image via Diffusion Models](https://openaccess.thecvf.com/content/ICCV2023/html/Papantoniou_Relightify_Relightable_3D_Faces_from_a_Single_Image_via_Diffusion_ICCV_2023_paper.html)||
|2023|WACV|[SIRA: Relightable Avatars From a Single Image](https://openaccess.thecvf.com/content/WACV2023/html/Caselles_SIRA_Relightable_Avatars_From_a_Single_Image_WACV_2023_paper.html)||
|2024|CVPR Workshops (EDGE)|[EdgeRelight360: Text-Conditioned 360-Degree HDR Image Generation for Real-Time On-Device Video Portrait Relighting](https://openaccess.thecvf.com/content/CVPR2024W/EDGE/html/Lin_EdgeRelight360_Text-Conditioned_360-Degree_HDR_Image_Generation_for_Real-Time_On-Device_Video_CVPRW_2024_paper.html)||
|2024|CVPR|[Holo-Relighting: Controllable Volumetric Portrait Relighting from a Single Image](https://openaccess.thecvf.com/content/CVPR2024/html/Mei_Holo-Relighting_Controllable_Volumetric_Portrait_Relighting_from_a_Single_Image_CVPR_2024_paper.html)||
|2024|SIGGRAPH|[Lite2Relight: 3D-aware Single Image Portrait Relighting](https://vcai.mpi-inf.mpg.de/projects/Lite2Relight/)||
|2024|WACV|[Multi-Level Attention Aggregation for Aesthetic Face Relighting](https://openaccess.thecvf.com/content/WACV2024/html/Pidaparthy_Multi-Level_Attention_Aggregation_for_Aesthetic_Face_Relighting_WACV_2024_paper.html)||
|2024|ECCV|[Personalized Video Relighting With an At-Home Light Stage](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/5689_ECCV_2024_paper.php)||
|2024|CVPR|[Real-time 3D-aware Portrait Video Relighting](https://openaccess.thecvf.com/content/CVPR2024/html/Cai_Real-time_3D-aware_Portrait_Video_Relighting_CVPR_2024_paper.html)||
|2024|CVPR|[Relightable Gaussian Codec Avatars](https://openaccess.thecvf.com/content/CVPR2024/html/Saito_Relightable_Gaussian_Codec_Avatars_CVPR_2024_paper.html)||
|2024|CVPR|[Relightful Harmonization: Lighting-aware Portrait Background Replacement](https://openaccess.thecvf.com/content/CVPR2024/html/Ren_Relightful_Harmonization_Lighting-aware_Portrait_Background_Replacement_CVPR_2024_paper.html)||
|2024|CVPR|[SwitchLight: Co-design of Physics-driven Architecture and Pre-training Framework for Human Portrait Relighting](https://openaccess.thecvf.com/content/CVPR2024/html/Kim_SwitchLight_Co-design_of_Physics-driven_Architecture_and_Pre-training_Framework_for_Human_CVPR_2024_paper.html)||
|2025|SIGGRAPH|[GSHeadRelight: Fast Relightability for 3D Gaussian Head Synthesis](https://s2025.conference-schedule.org/presentation/?id=papers_269&sess=sess117)|[Code](https://github.com/IGLICT/GSHeadRelight)|
|2025|CVPR|[High-Fidelity Relightable Monocular Portrait Animation with Lighting-Controllable Video Diffusion Model](https://openaccess.thecvf.com/content/CVPR2025/html/Guo_High-Fidelity_Relightable_Monocular_Portrait_Animation_with_Lighting-Controllable_Video_Diffusion_Model_CVPR_2025_paper.html)|[Code](https://github.com/MingtaoGuo/Relightable-Portrait-Animation)|
|2025|CVPR|[Lux Post Facto: Learning Portrait Performance Relighting with Conditional Video Diffusion and a Hybrid Dataset](https://openaccess.thecvf.com/content/CVPR2025/html/Mei_Lux_Post_Facto_Learning_Portrait_Performance_Relighting_with_Conditional_Video_CVPR_2025_paper.html)||
|2025|ICLR|[Scaling In-the-Wild Training for Diffusion-based Illumination Harmonization and Editing by Imposing Consistent Light Transport](https://openreview.net/forum?id=u1cQYxRI1H)|[Code](https://github.com/lllyasviel/IC-Light)|
|2025|CVPR|[SynthLight: Portrait Relighting with Diffusion Model by Learning to Re-render Synthetic Faces](https://openaccess.thecvf.com/content/CVPR2025/html/Chaturvedi_SynthLight_Portrait_Relighting_with_Diffusion_Model_by_Learning_to_Re-render_CVPR_2025_paper.html)||
|2025|AAAI|[Text2Relight: Creative Portrait Relighting with Text Guidance](https://ojs.aaai.org/index.php/AAAI/article/download/32194/34349)||
|2026|CVPR|[GeoRelight: Learning Joint Geometrical Relighting and Reconstruction with Flexible Multi-Modal Diffusion Transformers](https://openaccess.thecvf.com/content/CVPR2026/html/Xue_GeoRelight_Learning_Joint_Geometrical_Relighting_and_Reconstruction_with_Flexible_Multi-Modal_CVPR_2026_paper.html)|[Project](https://yuxuan-xue.com/georelight)|
|2026|CVPR|[RelightAnyone: A Generalized Relightable 3D Gaussian Head Model](https://openaccess.thecvf.com/content/CVPR2026/html/Xu_RelightAnyone_A_Generalized_Relightable_3D_Gaussian_Head_Model_CVPR_2026_paper.html)||
|2026|CVPR|[Relightful Video Portrait Harmonization](https://openaccess.thecvf.com/content/CVPR2026/html/Choi_Relightful_Video_Portrait_Harmonization_CVPR_2026_paper.html)||

## Dataset

|Year|Pub|Paper|Resources|
|:---:|:---:|:---:|:---:|
|2009|ICCV|[Ground Truth Dataset and Baseline Evaluations for Intrinsic Image Algorithms](https://billf.mit.edu/publication/ground-truth-dataset-and-baseline-evaluations-intrinsic-image-algorithms/)|[MIT Intrinsics](https://people.csail.mit.edu/rgrosse/intrinsic/)|
|2012|ECCV|[A Naturalistic Open Source Movie for Optical Flow Evaluation](https://is.mpg.de/ps/publications/butler-eccv-2012)|[MPI Sintel](http://sintel.is.tue.mpg.de/)|
|2014|SIGGRAPH|[Intrinsic Images in the Wild](http://opensurfaces.cs.cornell.edu/publications/intrinsic/)|[Dataset](http://opensurfaces.cs.cornell.edu/publications/intrinsic/)|
|2017|CVPR|[Shading Annotations in the Wild](http://opensurfaces.cs.cornell.edu/publications/saw/)|[Dataset](http://opensurfaces.cs.cornell.edu/publications/saw/)|
|2019|ICCV|[A Dataset of Multi-Illumination Images in the Wild](https://projects.csail.mit.edu/illumination/)|[Code](https://github.com/lmurmann/multi_illumination) / [Dataset](https://projects.csail.mit.edu/illumination/)|
|2021|ICCV|[Hypersim: A Photorealistic Synthetic Dataset for Holistic Indoor Scene Understanding](https://arxiv.org/abs/2011.02523)|[Dataset](https://github.com/apple/ml-hypersim)|
|2021|CVPR|[OpenRooms: An Open Framework for Photorealistic Indoor Scene Datasets](https://ucsd-openrooms.github.io/)|[Dataset](https://ucsd-openrooms.github.io/)|
|2023|CVPR|[ReLight My NeRF: A Dataset for Novel View Synthesis and Relighting of Real World Objects](https://openaccess.thecvf.com/content/CVPR2023/html/Toschi_ReLight_My_NeRF_A_Dataset_for_Novel_View_Synthesis_and_CVPR_2023_paper.html)|[Project](https://eyecan-ai.github.io/rene)|
|2023|NeurIPS Datasets & Benchmarks|[Stanford-ORB: A Real-World 3D Object Inverse Rendering Benchmark](https://proceedings.neurips.cc/paper_files/paper/2023/hash/92a821f6c25b29241df6985ceb673a85-Abstract-Datasets_and_Benchmarks.html)|[Code & Data](https://stanfordorb.github.io/)|
|2024|CVPR|[Towards a Perceptual Evaluation Framework for Lighting Estimation](https://openaccess.thecvf.com/content/CVPR2024/html/Giroux_Towards_a_Perceptual_Evaluation_Framework_for_Lighting_Estimation_CVPR_2024_paper.html)|[Project](https://lvsn.github.io/PerceptionMetric/)|
|2025|ICCV|[A Real-world Display Inverse Rendering Dataset](https://openaccess.thecvf.com/content/ICCV2025/html/Choi_A_Real-world_Display_Inverse_Rendering_Dataset_ICCV_2025_paper.html)|[Project](https://michaelcsj.github.io/DIR/)|
|2025|ICCV|[HumanOLAT: A Large-Scale Dataset for Full-Body Human Relighting and Novel-View Synthesis](https://openaccess.thecvf.com/content/ICCV2025/html/Teufel_HumanOLAT_A_Large-Scale_Dataset_for_Full-Body_Human_Relighting_and_Novel-View_ICCV_2025_paper.html)||
|2025|ICCV|[LightCity: An Urban Dataset for Outdoor Inverse Rendering and Reconstruction under Multi-illumination Conditions](https://openaccess.thecvf.com/content/ICCV2025/html/Wang_LightCity_An_Urban_Dataset_for_Outdoor_Inverse_Rendering_and_Reconstruction_ICCV_2025_paper.html)||
