[stars-img]: https://img.shields.io/github/stars/yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications?color=yellow
[stars-url]: https://github.com/yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications/stargazers
[fork-img]: https://img.shields.io/github/forks/yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications?color=lightblue&label=fork
[fork-url]: https://github.com/yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications/network/members
[AKGR-url]: https://github.com/yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications

# Graph Diffusion Models: A Comprehensive Survey of Methods and Applications
This is the summation of all the methods, datasets, and other survey mentioned in our survey 'Graph Diffusion Models: A Comprehensive Survey of Methods and Applications' :fire:. Any problems, please contact shouyuntao@stu.xjtu.edu.cn. Any other interesting papers or codes are welcome. If you find this repository useful to your research or work, it is really appreciated to star this repository :heart:.

[![GitHub stars][stars-img]][stars-url]
[![GitHub forks][fork-img]][fork-url]

<div  align="center"> 
  <img src="https://github.com/yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications/blob/main/fig/methods.jpg" width=100% />
</div>

<div  align="center"> 
  <img src="https://github.com/yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications/blob/main/fig/diffusionshuoming.png" width=100% />
</div>

<div  align="center"> 
  <img src="https://github.com/yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications/blob/main/fig/clas.png" width=100% />
</div>


## Contents
- [Diffusion-based Graph Generative Methods](#diffusion-based-grap-generative-methods)
  - [Contents](#contents)
  - [Molecule generation](#molecule-generation)
    - [Molecule design](#de-novo-molecule-design)
    - [Conformation design](#conformation-design)
    - [De novo ligand design](#de-novo-ligand-design)
    - [Ligand docking](#ligand-docking)
    - [Protein design](#protein-design)
  - [Motion generation](#motion-generation)
    - [Motion synthesis](#motion-synthesis)
    - [Motion prediction](#motion-prediction)
  - [Others](#others)
  - [Datasets](#datasets)
    - [Molecule generation](#molecule-generation-1)
    - [Motion generation](#motion-generation-1)
  - [Other surveys](#other-surveys)


## Molecule generation

### De novo molecule design
| Methods | Paper | Code | Methods | Paper | Code |
| :----: | :----: | :----: | :----: | :----: | :----: |
| DiGress (ICLR-23) | [[paper]](https://arxiv.org/abs/2209.14734) | [[code]](https://github.com/cvignac/DiGress) | MiDi (ICLR-23) | [[paper]](https://openreview.net/forum?id=M6Ifac3G4HK) | [[code]](https://github.com/cvignac/MiDi) | 
| CDGS (NeurIPS-22) | [[paper]](https://openreview.net/forum?id=YD39Pw2HXBXM) | [[code]](https://github.com/GRAPH-0/CDGS) | GCDM (ICLR-23) | [[paper]](https://openreview.net/forum?id=X-tLu3OUE-d) | [[code]](https://github.com/BioinfoMachineLearning/bio-diffusion) |
| EDM (ICML-22) | [[paper]](https://proceedings.mlr.press/v162/hoogeboom22a.html) | [[code]](https://github.com/ehoogeboom/e3_diffusion_for_molecules) |  Wu et al. (NeurIPS-22) | [[paper]](https://openreview.net/forum?id=QagNEt9k8Vi) | - |
| MDM (AAAI-23) | [[paper]](https://arxiv.org/abs/2209.05710) | [[code]](https://github.com/tencent-ailab/MDM) | DiffLinker | [[paper]](https://openreview.net/forum?id=viZ4G1WZxh) | [[code]](https://github.com/igashov/DiffLinker) |
| JODO | [[paper]](https://doi.org/10.48550/arXiv.2305.12347) | [[code]](https://github.com/GRAPH-0/JODO)| SILVR | [[paper]](https://doi.org/10.48550/arXiv.2304.10905) | - |
| HierDiff (ICML-23) | [[paper]](https://proceedings.mlr.press/v202/qiang23a.html) | [[code]](https://github.com/qiangbo1222/HierDiff) | - | - | - |
| BIMODAL | [[paper]](https://pubs.acs.org/doi/pdf/10.1021/acs.jcim.9b00943) | [[code]](https://github.com/ETHmodlab/BIMODAL) |  RationaleRL (ICML20) | [[paper]](https://proceedings.mlr.press/v119/jin20b/jin20b.pdf) | [[code]](https://github.com/wengong-jin/multiobj-rationale) |
| GEOLDM (ICML-23) | [[paper]](https://proceedings.mlr.press/v202/xu23n/xu23n.pdf)| [[code]](https://github.com/MinkaiXu/GeoLDM) | MGM | [[paper]](https://www.nature.com/articles/s41467-021-23415-2.pdf)| -|
| LFM AISTATS-20| [[paper]](https://proceedings.mlr.press/v108/podda20a/podda20a.pdf) | [[code]](https://github.com/marcopodda/fragment-based-dgm) | RetMol | [[paper]](https://arxiv.org/pdf/2208.11126) | [[code]](https://github.com/NVlabs/RetMol) |
| MolGPT | [[paper]](https://chemrxiv.org/engage/api-gateway/chemrxiv/assets/orp/resource/item/60c7588e469df48597f456ae/original/lig-gpt-molecular-generation-using-a-transformer-decoder-model.pdf) | - | Bridge (NeurIPS-2022) | [[paper]](https://proceedings.neurips.cc/paper_files/paper/2022/file/eccc6e11878857e87ec7dd109eaa9eeb-Paper-Conference.pdf) | - |
| Bresson et al. | [[paper]](https://arxiv.org/pdf/1906.03412) | - | FLAG (ICLR-23) | [[paper]](https://openreview.net/pdf?id=Rq13idF0F73) | [[code]](https://github.com/zaixizhang/FLAG) |
| LIMO | [[paper]](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9527083/) | [[code]](https://github.com/Rose-STL-Lab/LIMO) | D3FG NeurIPS-24 | [[paper]](https://proceedings.neurips.cc/paper_files/paper/2023/file/6cdd4ce9330025967dd1ed0bed3010f5-Paper-Conference.pdf) | [[code]](https://github.com/EDAPINENUT/CBGBench/tree/master) |

### Conformation design
| Methods | Paper | Code | Methods | Paper | Code |
| :----: | :----: | :----: | :----: | :----: | :----: |
| ConfGF (ICML-21) | [[paper]](https://proceedings.mlr.press/v139/shi21b.html) | [[code]](https://github.com/DeepGraphLearning/ConfGF) | DGSM (NeurIPS-21) | [[paper]](https://proceedings.neurips.cc/paper_files/paper/2021/file/a45a1d12ee0fb7f1f872ab91da18f899-Paper.pdf) | - | 
| GeoDiff (ICLR-22) | [[paper]](https://openreview.net/forum?id=PzcvxEMzvQC) | [[code]](https://github.com/MinkaiXu/GeoDiff) | ColfNet (ICML-22) | [[paper]](https://proceedings.mlr.press/v162/du22e.html) | - |
| Torsion Diffusion (NeurIPS-22) | [[paper]](https://openreview.net/forum?id=w6fj2r62r_H) | [[code]](https://github.com/gcorso/torsional-diffusion) | DiffMD (AAAI-23) | [[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/25663) | - |
| RINGER| [[paper]](https://doi.org/10.48550/arXiv.2305.19800) | - | - | - | - |
### De novo ligand design
| Methods | Paper | Code | Methods | Paper | Code |
| :----: | :----: | :----: | :----: | :----: | :----: |
| DiffBP | [[paper]](https://arxiv.org/abs/2211.11214) | - | DiffSBDD | [[paper]](https://arxiv.org/abs/2210.13695) | - | 
| TargetDiff (ICLR-23) | [[paper]](https://openreview.net/forum?id=kJqXEPXMsE0) | - | PMDM | [[paper]](https://www.biorxiv.org/content/early/2023/01/30/2023.01.28.526011) | - |
| D3FG | [[paper]](https://doi.org/10.48550/arXiv.2306.13769) | - | - | - | - |
### Ligand docking
| Methods | Paper | Code |
| :----: | :----: | :----: |
| DIFFDOCK (NeurIPS-22) | [[paper]](https://openreview.net/forum?id=fky3a3F80if) | - |
| EDM-Dock (JCIM) | [[paper]](https://doi.org/10.1021/acs.jcim.2c01436) | [[code]](https://github.com/MatthewMasters/EDM-Dock) |
| DPL | [[paper]](https://doi.org/10.1186/s12859-023-05354-5) | [[code]](https://github.com/shuyana/DiffusionProteinLigand) |
| NeuralPLexer | [[paper]](https://doi.org/10.48550/arXiv.2209.15171) | - |
|  E3BIND (ICLR-23) | [[paper]](https://arxiv.org/pdf/2210.06069) | - |



### Protein design
| Methods | Paper | Code | Methods | Paper | Code |
| :----: | :----: | :----: | :----: | :----: | :----: |
| DiffAb (NeurIPS-22) | [[paper]](https://openreview.net/forum?id=jSorGn2Tjg) | - | Anand | [[paper]](https://arxiv.org/abs/2205.15019) | - | 
| PROTSEED (ICLR-23) | [[paper]](https://openreview.net/forum?id=pRCMXcfdihq) | - | ProteinSGM | [[paper]](https://www.biorxiv.org/content/early/2023/02/04/2022.07.13.499967) | [[code]](https://gitlab.com/mjslee0921/proteinsgm) |
| SMCDiff (ICLR-23) | [[paper]](https://arxiv.org/abs/2206.04119) | [[code]](https://github.com/blt2114/ProtDiff_SMCDiff) | GraDe-IF | [[paper]](https://doi.org/10.48550/arXiv.2306.16819) | - |
| EigenFold | [[paper]](https://openreview.net/forum?id=BgbRVzfQqFp) | [[code]](https://github.com/bjing2016/EigenFold) | - | - | - |
| CGM (NeurIPS-19) | [[paper]](https://proceedings.neurips.cc/paper_files/paper/2019/file/f3a4ff4839c56a5f460c88cce3666a2b-Paper.pdf) | [[code]](https://github.com/jingraham/neurips19-graph-protein-design) | SeqDesign | [[paper]](https://www.nature.com/articles/s41467-021-22732-w) | [[code]](https://github.com/debbiemarkslab/SeqDesign) |
| Fold2Seq (ICML-21) | [[paper]](https://proceedings.mlr.press/v139/cao21a/cao21a.pdf) | [[code]](https://github.com/IBM/fold2seq) | EvoDiff | [[paper]](https://www.biorxiv.org/content/10.1101/2023.09.11.556673v1.full.pdf) | - |
| GVP （ICLR-21） | [[paper]](https://openreview.net/pdf?id=1YLJDvSx6J4) | [[code]](https://github.com/drorlab/gvp) | ESM (NeurIPS-21) | [[paper]](https://proceedings.neurips.cc/paper_files/paper/2021/file/f51338d736f95dd42427296047067694-Paper.pdf) | - |

## Motion generation

### Motion synthesis
| Methods | Paper | Code | Homepage | Methods | Paper | Code | Homepage |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| MotionDiffuse | [[paper]](https://arxiv.org/abs/2208.15001) | [[code]](https://github.com/mingyuan-zhang/MotionDiffuse) | [[homepage]](https://mingyuan-zhang.github.io/projects/MotionDiffuse.html) | Modiff | [[paper]](https://arxiv.org/abs/2301.03949) | - | - |
| Ren et al. (ICASSP-23) | [[paper]](https://doi.org/10.1109/ICASSP49357.2023.10096441) | - | - | FLAME (AAAI-23) | [[paper]](https://arxiv.org/abs/2209.00349) | - | - |
| MoFusion (CVPR-23) | [[paper]](https://openaccess.thecvf.com/content/CVPR2023/html/Dabral_Mofusion_A_Framework_for_Denoising-Diffusion-Based_Motion_Synthesis_CVPR_2023_paper.html) | - | [[homepage]](https://vcai.mpi-inf.mpg.de/projects/MoFusion/) | MDM (ICLR-23) | [[paper]](https://arxiv.org/abs/2209.14916) | [[code]](https://github.com/GuyTevet/motion-diffusion-model) | [[homepage]](https://guytevet.github.io/mdm-page/) |
| MLD (CVPR-23) | [[paper]](https://openaccess.thecvf.com/content/CVPR2023/html/Chen_Executing_Your_Commands_via_Motion_Diffusion_in_Latent_Space_CVPR_2023_paper.html) | [[code]](https://github.com/chenfengye/motion-latent-diffusion) | [[homepage]](https://chenxin.tech/mld/) | PriorMDM | [[paper]](https://arxiv.org/abs/2303.01418) | [[code]](https://github.com/priorMDM/priorMDM) | [[homepage]](https://priormdm.github.io/priorMDM-page/) |
| Alexanderson et al. (ACM Trans. Graph.) | [[paper]](https://arxiv.org/abs/2211.09707) | - | - | EDGE (CVPR-23) | [[paper]](https://openaccess.thecvf.com/content/CVPR2023/html/Tseng_EDGE_Editable_Dance_Generation_From_Music_CVPR_2023_paper.html) | [[code]](https://github.com/Stanford-TML/EDGE) | [[homepage]](https://edge-dance.github.io/) |
| SceneDiffuser | [[paper]](https://arxiv.org/abs/2301.06015) | [[code]](https://github.com/scenediffuser/Scene-Diffuser) | [[homepage]](https://scenediffuser.github.io/) | MoDi (CVPR-23) | [[paper]](https://openaccess.thecvf.com/content/CVPR2023/html/Raab_MoDi_Unconditional_Motion_Synthesis_From_Diverse_Data_CVPR_2023_paper.html) | [[code]](https://github.com/sigal-raab/MoDi) | [[homepage]](https://sigal-raab.github.io/MoDi) |
| BiGraphDiff | [[paper]](https://arxiv.org/abs/2301.10134) | - | - | DiffuPose | [[paper]](https://doi.org/10.48550/arXiv.2212.02796) | - | - |
<!-- | - | [[paper]]() | - | - | - | [[paper]]() | - | - |
| - | [[paper]]() | - | - | - | [[paper]]() | - | - | -->
### Motion prediction
| Methods | Paper | Code | Homepage |
| :----: | :----: | :----: | :----: |
| Ahn et al. (ICRA-23) | [[paper]](https://arxiv.org/abs/2302.14503) | [[code]](https://github.com/cotton-ahn/diffusion-motion-prediction) | [[homepage]](https://sites.google.com/view/diffusion-motion-prediction) |
| HumanMAC | [[paper]](https://arxiv.org/abs/2302.03665) | [[code]](https://github.com/LinghaoChan/HumanMAC) | [[homepage]](https://lhchen.top/Human-MAC/) |
| TCD (ICRA-23) | [[paper]](https://doi.org/10.1109/ICRA48891.2023.10160399) | [[code]](https://github.com/vita-epfl/DePOSit) | - |
| DiffMotion | [[paper]](https://doi.org/10.48550/arXiv.2305.12554) | - | - |

## Others
| Methods | Paper | Code | Homepage | Methods | Paper | Code | Homepage |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| EDP-GNN | [[paper]](https://proceedings.mlr.press/v108/niu20a.html) | - | - | GSDM | [[paper]](https://arxiv.org/abs/2211.08892) | - | - |
| NVDiff | [[paper]](https://arxiv.org/abs/2211.10794) | - | - | DPM-GSP | [[paper]](https://arxiv.org/abs/2302.10506) | - | - |
| DiffSTG | [[paper]](https://arxiv.org/abs/2301.13629) | - | - | DIFUSCO | [[paper]](https://arxiv.org/abs/2302.08224) | - | - |
| GraphGDP | [[paper]](https://arxiv.org/abs/2212.01842) | [[code]](https://github.com/GRAPH-0/GraphGDP) | - | HouseDiffusion (CVPR-23) | [[paper]](https://openaccess.thecvf.com/content/CVPR2023/html/Shabani_HouseDiffusion_Vector_Floorplan_Generation_via_a_Diffusion_Model_With_Discrete_CVPR_2023_paper.html) | [[code]](https://github.com/aminshabani/house_diffusion) | [[homepage]](https://aminshabani.github.io/housediffusion/) |
| NAP | [[paper]](https://arxiv.org/abs/2305.16315) | - | [[homepage]](https://www.cis.upenn.edu/~leijh/projects/nap/) | EDGE | [[paper]](https://arxiv.org/abs/2305.04111) | - | - |
| DruM | [[paper]](https://arxiv.org/abs/2302.03596) | - | - | DDM | [[Paper]](https://arxiv.org/abs/2306.13210) | - | - |
| DiffusionNAG | [[paper]](https://arxiv.org/abs/2305.16943) | - | - | TSDiff | [[paper]](https://doi.org/10.21203/rs.3.rs-2924237/v1) | - | - |
| GraphArm | [[paper]](https://openreview.net/forum?id=98J48HZXxd5) | - | - | HGDM | [[paper]](https://doi.org/10.48550/arXiv.2306.07618) | [[code]](https://github.com/GRAPH-0/JODO) | - |
| Lee et al. | [[paper]](https://doi.org/10.1080/15376494.2023.2198528) | - | - | SaGess | [[paper]](https://doi.org/10.48550/arXiv.2306.16827) | - | - |
| SLD | [[paepr]](https://openreview.net/forum?id=AykEgQNPJEK) | - | - | Diff-POI | [[paper]](https://doi.org/10.48550/arXiv.2304.07041) | - | - |
| Brain Diffuser | [[paper]](https://doi.org/10.48550/arXiv.2303.06410) | - | - | Lu et al. | [[paper]](https://doi.org/10.48550/arXiv.2304.05137) | - | - |

## Datasets

|     Dataset     | Dimensionality |         Category         | No.of Graphs (G) | No. of Nodes (N) |
|:---------------:|:--------------:|:------------------------:|:----------------:|:----------------:|
| Community-small |       2D       |          Social          |        100       |    11 < N < 20   |
|    Ego-small    |       2D       |          Social          |        200       |    3 < N < 18    |
|       Grid      |       2D       |           Grid           |        100       |     N <= 400     |
|       QM9       |       3D       | Bioinformatics/Molecular |      130,831     |    3 < N < 29    |
|     ZINC250K    |       3D       | Bioinformatics/Molecular |      249,456     |    6 < N < 38    |
|     Enzymes     |       3D       |  Bioinformatics/Protein  |        600       |    9 < N < 125   |
|      SBM-27     |       2D       |          Social          |        200       |    24 < N < 27   |
|    Planar-60    |       2D       |          Social          |        200       |      N = 60      |
|    AIDS         |       2D       | Bioinformatics/Molecular |        2000      |         -        |
|   Synthie       |       2D       |          Social          |        300       |      N = 100     |
|    Proteins     |       3D       | Bioinformatics/Protein   |        1113      |      N = 39.1    |

### Molecule generation

| Methods | Paper | Source | Methods | Paper | Source |
| :----: | :----: | :----: | :----: | :----: | :----: |
| Zinc | [[paper]](https://doi.org/10.1021/ci3001277) | [[source]](https://zinc.docking.org/) | GEOM-QM9 | [[paper]](https://doi.org/10.1038/sdata.2014.22) | [[source]](https://doi.org/10.7910/DVN/JNGTDF) |
| GEOM-Drugs | [[paper]](https://doi.org/10.1038/s41597-022-01288-4) | [[source]](https://doi.org/10.7910/DVN/JNGTDF) | CrossDocked2020 | [[paper]](https://doi.org/10.1021/acs.jcim.0c00411) | [[source]](https://github.com/gnina/models) |
| BioLiP | [[paper]](https://doi.org/10.1093/nar/gks966) | [[source]](https://zhanggroup.org/BioLiP/index.cgi) | PDBBind | [[paper]](https://doi.org/10.1021/acs.accounts.6b00491) | [[source]](http://www.pdbbind.org.cn/) |
| SAbDab | [[paper]](https://doi.org/10.1093/nar/gkt1043) | [[source]](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabdab) | - | - | - |
### Motion generation

| Methods | Paper | Source | Methods | Paper | Source |
| :----: | :----: | :----: | :----: | :----: | :----: |
| Human3.6M | [[paper]](https://doi.org/10.1109/TPAMI.2013.248) | [[source]](http://vision.imar.ro/human3.6m/description.php) | HumanEva-I | [[paper]](https://doi.org/10.1007/s11263-009-0273-6) | [[source]](http://humaneva.is.tue.mpg.de/) |
| HumanAct12 | [[paper]](https://doi.org/10.1145/3394171.3413635) | [[source]](https://ericguo5513.github.io/action-to-motion/) | HumanML3D | [[paper]](https://openaccess.thecvf.com/content/CVPR2022/html/Guo_Generating_Diverse_and_Natural_3D_Human_Motions_From_Text_CVPR_2022_paper.html) | [[source]](https://github.com/EricGuo5513/HumanML3D) |
| KIT | [[paper]](https://doi.org/10.1089/big.2016.0028) | [[source]](https://motion-annotation.humanoids.kit.edu/dataset/) | BABEL | [[paper]](https://openaccess.thecvf.com/content/CVPR2021/html/Punnakkal_BABEL_Bodies_Action_and_Behavior_With_English_Labels_CVPR_2021_paper.html) | [[source]](https://babel.is.tue.mpg.de/) |
| UESTC | [[paper]](https://doi.org/10.1145/3240508.3240675) | [[source]](https://github.com/HRI-UESTC/CFM-HRI-RGB-D-action-database) | 3DPW | [[paper]](https://openaccess.thecvf.com/content_ECCV_2018/html/Timo_von_Marcard_Recovering_Accurate_3D_ECCV_2018_paper.html) | [[source]](http://virtualhumans.mpi-inf.mpg.de/3DPW) |
| NTU RGB+D | [[paper]](https://openaccess.thecvf.com/content_cvpr_2016/html/Shahroudy_NTU_RGBD_A_CVPR_2016_paper.html) | [[source]](https://rose1.ntu.edu.sg/dataset/actionRecognition/) | AIST++ | [[paper]](https://openaccess.thecvf.com/content/ICCV2021/html/Li_AI_Choreographer_Music_Conditioned_3D_Dance_Generation_With_AIST_ICCV_2021_paper.html) | [[source]](https://google.github.io/aichoreographer) |
| TSG | [[paper]](https://doi.org/10.1145/3267851.3267898) | [[source]]() | ZeroEGGS | [[paper]](https://doi.org/10.1111/cgf.14734) | [[source]](https://github.com/ubisoft/ubisoft-laforge-ZeroEGGS) |

## Other surveys
| Paper | Url | Source | 
| :---- | :----: | :----: 
| Diffusion-based Graph Generative Methods | [[paper]](https://arxiv.org/abs/2401.15617) | [[source]](https://github.com/zhejiangzhuque/Diffusion-based-Graph-Generative-Methods) |
| Diffusion Models: A Comprehensive Survey of Methods and Applications | [[paper]](https://doi.org/10.48550/arXiv.2209.00796) | [[source]](https://github.com/YangLing0818/Diffusion-Models-Papers-Survey-Taxonomy) |
| A Survey on Generative Diffusion Model | [[paper]](https://doi.org/10.48550/arXiv.2209.02646) | [[source]](https://github.com/chq1155/A-Survey-on-Generative-Diffusion-Model) |
| Generative Diffusion Models on Graphs: Methods and Applications | [[paper]](https://doi.org/10.48550/arXiv.2302.02591) | - |
| A Survey on Graph Diffusion Models: Generative AI in Science for Molecule, Protein and Material | [[paper]](https://rgdoi.net/10.13140/RG.2.2.26493.64480) | - |
| Graph-based Molecular Representation Learning | [[paper]](https://doi.org/10.48550/arXiv.2207.04869) | - |
| Generative Models as an Emerging Paradigm in the Chemical Sciences | [[paper]](https://doi.org/10.1021/jacs.2c13467) | - |
| A Survey on Deep Graph Generation: Methods and Applications (LoG-22) | [[paper]](https://doi.org/10.48550/arXiv.2203.06714) | - |
| A Survey on Temporal Graph Representation Learning and Generative Modeling | [[paper]](https://doi.org/10.48550/arXiv.2208.12126) | - |
| Human motion modeling with deep learning: A survey | [[paper]](https://doi.org/10.1016/j.aiopen.2021.12.002) | - |
| MolGenSurvey: A Systematic Survey in Machine Learning Models for Molecule Design | [[paper]](https://doi.org/10.48550/arXiv.2203.14500) | - |

## Acknowledgement :heart:
Thanks to [Diffusion-based-Graph-Generative-Methods](https://github.com/zhejiangzhuque/Diffusion-based-Graph-Generative-Methods).

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications&type=Date)](https://star-history.com/#yuntaoshou/Graph-Diffusion-Models-A-Comprehensive-Survey-of-Methods-and-Applications&Date)
