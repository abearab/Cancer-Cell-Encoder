# Cancer Cell Encoder
This repository contains scripts for statistical inference and deep learning to study genetic interactions.

Since datasets are limited to very few type of cancer cell line models, we use an auto-encoder structure to learn the
genetic background of cancer cells using gene expression data from the Cancer Cell Line Encyclopedia (CCLE) as part
of [DepMap](https://depmap.org/portal/) project. Theoretically, the encoder part of the model should learn the genetic
background of the cell lines represented in a low dimensional space. We then aim to use this representation of the 
cancer cell lines to enrich other models by adding this background information to the model. These models are those 
that predict genetic interaction between genes using experimental data in large scale 
combinatorial perturbation screen studies such as:

Horlbeck, et al. **Mapping the Genetic Landscape of Human Cells**. _Cell_ (2018)
[**\[Paper\]**](https://doi.org/10.1016/j.cell.2018.06.010) 
[**\[Original Codes\]**](https://github.com/mhorlbeck/GImap_tools)
