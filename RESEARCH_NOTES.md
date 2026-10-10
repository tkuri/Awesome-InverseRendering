# Literature audit — 2026-10-11

This update adds **176 publications**: 174 method/dataset papers and two surveys. The README now has 245 table entries, including the previously unnumbered intrinsic-image survey. Existing papers were retained, with two entries moved to more appropriate sections.

## Selection and search coverage

The list covers intrinsic decomposition, geometry/material/lighting recovery, and image, scene, human and portrait relighting. It includes established vision, graphics and machine-learning venues, 3DV, WACV, and relevant associated workshops. A workshop presentation is labeled separately from the main conference. A preprint is eligible only when a publication venue was confirmed.

The systematic part of the search inspected title lists and relevant abstracts in the following primary proceedings:

- [CVF Open Access](https://openaccess.thecvf.com/menu): CVPR 2022–2026, ICCV 2023/2025, and WACV 2022–2026.
- [ECVA proceedings](https://www.ecva.net/papers.php): ECCV 2018/2020/2022/2024.

These were supplemented by publication records and author pages for earlier foundational papers, SIGGRAPH/SIGGRAPH Asia, Eurographics/EGSR, TOG, CGF, IJCV, TPAMI, NeurIPS, ICLR, AAAI, 3DV, and selected CVPR/ICCV/WACV workshops. This supplemental search was targeted rather than a complete enumeration of every venue/year. Searches included intrinsic decomposition, inverse rendering, relighting, SVBRDF/BRDF, reflectance, material reconstruction, lighting and illumination estimation; additional author-page checks recovered papers whose titles did not contain those terms.

Each new entry links to its primary proceedings record, paper, publisher record or author page. Code links were taken from official implementations or author pages. Publication year follows the listed venue, not the initial arXiv date.

The 174 new method/dataset entries comprise:

| Area | Added entries |
| --- | ---: |
| Intrinsic decomposition: non-DL / DL | 7 / 16 |
| Physical inverse rendering / explicit Gaussian inverse rendering | 4 / 8 |
| Neural fields and multi-view reflectance reconstruction | 50 |
| Image/video decomposition, diffusion and material priors | 15 |
| Lighting estimation | 6 |
| Human/face inverse rendering | 9 |
| Gaussian methods with neural components | 11 |
| Scene/video relighting | 13 |
| Portrait relighting | 27 |
| Datasets and benchmarks | 8 |

## Corrections and classification

- Removed the sentence announcing that inverse-rendering updates had stopped, and the unrelated deblurring comment.
- Moved *Intrinsic Decompositions for Image Editing* (Eurographics/CGF 2017) from DL methods to surveys.
- Identified *A Survey on Intrinsic Images: Delving Deep Into Lambert and Beyond* as IJCV 2022 and placed it in the survey table.
- Replaced the unrelated RIN link for *Intrinsic Image Transformation via Scale Space Decomposition* with its CVPR 2018 paper record.
- Added the official USI3D implementation to the existing CVPR 2020 intrinsic-decomposition entry.
- Moved *Material and Lighting Reconstruction for Complex Indoor Scenes with Texture-space Differentiable Rendering* to non-DL. The [author publication record](https://rgl.epfl.ch/publications/NimierDavid2021Material) describes physical differentiable optimization; EGSR's “DL-only Track” refers to the **Digital Library**, not deep learning.
- Distinguished explicit Gaussian optimization from neural Gaussian pipelines. For example, ReCap optimizes explicit material and lighting parameters; LumiGauss uses an MLP for lighting, LumiMotion uses a deformation network, and GHPT uses pretrained normal supervision. PyTorch/automatic differentiation alone does not determine the classification.
- Described capture conditions in the added inverse-rendering tables instead of inferring binary L/G/M capabilities from titles. In particular, NeILF uses supplied geometry; NeILF++ jointly reconstructs geometry.
- Replaced three unavailable candidate links for Weiss's ICCV 2001 paper, SAMURAI and the DPR implementation with accessible paper/proceedings/code links.

## Validation and limits

Checked table column counts, year ordering, duplicate titles, internal navigation, preservation of the existing bibliography, and Git whitespace errors. An automated HTTP check covered **232 distinct URLs** in the new method/dataset entries and their resources. No HTTP 404 remained. Nine responses were inconclusive because of certificate verification, access restrictions, or a publisher's HTTP 202 response; these were not treated as broken links. An HTTP 200 may also be an anti-bot page, so reachability alone is not evidence of publication or content correctness.

This is a broad curated expansion, not a claim of exhaustive coverage. In particular, ECCV 2026 and all associated workshop proceedings were not systematically enumerated in this pass. Older journal-only literature, every workshop challenge submission, and appearance-related papers without explicit decomposition/relighting goals were not exhaustively collected. Standalone denoising, photometric stereo, reflection removal, text-to-3D generation and ordinary novel-view synthesis were generally excluded unless inverse rendering or relighting was a central contribution. The original legacy L/G/M annotations were retained rather than fully re-audited.

Future additions should verify the primary publication venue, inspect the actual neural components before assigning DL/non-DL, search by title before adding a duplicate, and record official resources only when identifiable.
