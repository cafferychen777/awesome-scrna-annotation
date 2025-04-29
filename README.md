# Awesome scRNA Cell Type Annotation

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![GitHub stars](https://img.shields.io/github/stars/cafferychen777/awesome-scrna-annotation?style=social)](https://github.com/cafferychen777/awesome-scrna-annotation/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/cafferychen777/awesome-scrna-annotation?style=social)](https://github.com/cafferychen777/awesome-scrna-annotation/network/members)
[![GitHub contributors](https://img.shields.io/github/contributors/cafferychen777/awesome-scrna-annotation)](https://github.com/cafferychen777/awesome-scrna-annotation/graphs/contributors)
[![Last commit](https://img.shields.io/github/last-commit/cafferychen777/awesome-scrna-annotation)](https://github.com/cafferychen777/awesome-scrna-annotation/commits/main)

> A comprehensive, curated collection of state-of-the-art single-cell RNA sequencing (scRNA-seq) cell type annotation tools, methods, databases, and resources for bioinformatics researchers and computational biologists.

Cell type annotation is a critical step in single-cell RNA sequencing analysis that involves assigning biological identities to clusters of cells based on their gene expression profiles. This repository serves as a central hub for high-quality tools and resources that can help researchers accurately identify cell types in their scRNA-seq datasets.

This collection only includes high-quality tools that either:
- Have more than 100 stars on GitHub, OR
- Are published in prestigious journals (Cell, Nature, Science and their sister journals, or Genome Biology)

## Contents

- [Cell Type Annotation Tools](#cell-type-annotation-tools)
  - [Machine Learning Based](#machine-learning-based)
  - [Reference Based](#reference-based)
  - [Marker Gene Based](#marker-gene-based)
  - [Large Language Model Based](#large-language-model-based)
- [Benchmark Studies](#benchmark-studies)
- [Databases](#databases)
  - [Cell Marker Databases](#cell-marker-databases)
  - [Reference Datasets](#reference-datasets)
- [Tutorials and Workflows](#tutorials-and-workflows)
- [Community Resources](#community-resources)
- [Contributing](#contributing)
- [Star History](#star-history)
- [License](#license)

## Cell Type Annotation Tools

| Tool | Description | Publication | GitHub Stars | Journal |
|------|-------------|-------------|--------------|---------|
| [mLLMCelltype](https://github.com/cafferychen777/mLLMCelltype) | An iterative multi-LLM consensus framework for accurate cell type annotation in single-cell RNA-seq data | Yang C, et al. (2025). Large Language Model Consensus Substantially Improves the Cell Type Annotation Accuracy for scRNA-seq Data. | ![GitHub stars](https://img.shields.io/github/stars/cafferychen777/mLLMCelltype) | bioRxiv |
| [GPTCelltype](https://github.com/Winnie09/GPTCelltype) | Automatic cell type annotation with GPT-4 in single-cell RNA-seq analysis | Hou W, Ji Z. (2024). Reference-free and cost-effective automated cell type annotation with GPT-4 in single-cell RNA-seq analysis. | ![GitHub stars](https://img.shields.io/github/stars/Winnie09/GPTCelltype) | Nature Methods |
| [Seurat](https://github.com/satijalab/seurat) | R toolkit for single cell genomics | Satija R, et al. (2015). Spatial reconstruction of single-cell gene expression data. | ![GitHub stars](https://img.shields.io/github/stars/satijalab/seurat) | Nature Biotechnology |
| [SCANPY](https://github.com/theislab/scanpy) | Single-Cell Analysis in Python | Wolf FA, et al. (2018). SCANPY: large-scale single-cell gene expression data analysis. | ![GitHub stars](https://img.shields.io/github/stars/theislab/scanpy) | Genome Biology |
| [Celltypist](https://github.com/Teichlab/celltypist) | A tool for semi-automatic cell type classification based on logistic regression | Domínguez Conde C, et al. (2022). Cross-tissue immune cell analysis reveals tissue-specific features in humans. | ![GitHub stars](https://img.shields.io/github/stars/Teichlab/celltypist) | Science |
| [ScType](https://github.com/IanevskiAleksandr/sc-type) | Fully-automated and ultra-fast cell-type identification using specific marker combinations | Ianevski A, et al. (2022). Fully-automated and ultra-fast cell-type identification using specific marker combinations from single-cell transcriptomic data. | ![GitHub stars](https://img.shields.io/github/stars/IanevskiAleksandr/sc-type) | Nature Communications |
| [scCATCH](https://github.com/ZJUFanLab/scCATCH) | Automatic Annotation on Cell Types of Clusters from Single-Cell RNA Sequencing Data | Shao X, et al. (2020). scCATCH: Automatic Annotation on Cell Types of Clusters from Single-Cell RNA Sequencing Data. | ![GitHub stars](https://img.shields.io/github/stars/ZJUFanLab/scCATCH) | iScience |
| [CellAssign](https://github.com/Irrationone/cellassign) | Automated, probabilistic assignment of cell types in scRNA-seq data | Zhang AW, et al. (2019). Probabilistic cell-type assignment of single-cell RNA-seq for tumor microenvironment profiling. | ![GitHub stars](https://img.shields.io/github/stars/Irrationone/cellassign) | Nature Methods |
| [scArches](https://github.com/theislab/scarches) | Reference mapping for single-cell genomics with cell type transfer | Lotfollahi M, et al. (2021). Mapping single-cell data to reference atlases by transfer learning. | ![GitHub stars](https://img.shields.io/github/stars/theislab/scarches) | Nature Biotechnology |
| [scGate](https://github.com/carmonalab/scGate) | Marker-based purification of cell types from single-cell RNA-seq datasets | Andreatta M, et al. (2022). scGate: marker-based purification of cell types from heterogeneous single-cell RNA-seq datasets. | ![GitHub stars](https://img.shields.io/github/stars/carmonalab/scGate) | Bioinformatics |
| [popV](https://github.com/YosefLab/popV) | Ensemble method using popular vote of various cell-type transfer tools | Ergen C, Xing G, et al. (2024). Consensus prediction of cell type labels in single-cell data with popV. | ![GitHub stars](https://img.shields.io/github/stars/YosefLab/popV) | Nature Genetics |
| [Garnett](https://github.com/cole-trapnell-lab/garnett) | Cell type classification using marker genes and scRNA-seq data | Pliner HA, et al. (2019). Supervised classification enables rapid annotation of cell atlases. | ![GitHub stars](https://img.shields.io/github/stars/cole-trapnell-lab/garnett) | Nature Methods |
| [scmap](https://github.com/hemberg-lab/scmap) | A tool for unsupervised projection of single cell RNA-seq data | Kiselev VY, et al. (2018). scmap: projection of single-cell RNA-seq data across data sets. | ![GitHub stars](https://img.shields.io/github/stars/hemberg-lab/scmap) | Nature Methods |
| [SingleR](https://github.com/dviraran/SingleR) | Reference-based single-cell RNA-seq annotation | Aran D, et al. (2019). Reference-based analysis of lung single-cell sequencing reveals a transitional profibrotic macrophage. | ![GitHub stars](https://img.shields.io/github/stars/dviraran/SingleR) | Nature Immunology |
| [Azimuth](https://github.com/satijalab/azimuth) | Reference-based annotation for single-cell data | Hao Y, et al. (2021). Integrated analysis of multimodal single-cell data. | ![GitHub stars](https://img.shields.io/github/stars/satijalab/azimuth) | Cell |
| [scBERT](https://github.com/TencentAILabHealthcare/scBERT) | Large-scale pretrained deep language model for cell type annotation | Yang F, et al. (2022). scBERT as a large-scale pretrained deep language model for cell type annotation of single-cell RNA-seq data. | ![GitHub stars](https://img.shields.io/github/stars/TencentAILabHealthcare/scBERT) | Nature Machine Intelligence |
| [scGPT](https://github.com/bowang-lab/scGPT) | Foundation model for single-cell multi-omics using generative AI | Cui H, Wang C, et al. (2024). scGPT: toward building a foundation model for single-cell multi-omics using generative AI. | ![GitHub stars](https://img.shields.io/github/stars/bowang-lab/scGPT) | Nature Methods |
| [scDeepSort](https://github.com/ZJUFanLab/scDeepSort) | Pre-trained cell-type annotation method using deep learning with a weighted graph neural network | Shao X, et al. (2021). scDeepSort: a pre-trained cell-type annotation method for single-cell transcriptomics using deep learning with a weighted graph neural network. | ![GitHub stars](https://img.shields.io/github/stars/ZJUFanLab/scDeepSort) | Nucleic Acids Research |
| [scJoint](https://github.com/SydneyBioX/scJoint) | Transfer learning for data integration of atlas-scale single-cell RNA-seq and ATAC-seq data | Lin Y, et al. (2022). scJoint integrates atlas-scale single-cell RNA-seq and ATAC-seq data with transfer learning. | ![GitHub stars](https://img.shields.io/github/stars/SydneyBioX/scJoint) | Nature Biotechnology |

## Benchmark Studies

| Study | Description | Publication | Journal |
|-------|-------------|-------------|---------|
| [Single-cell RNA-seq annotation benchmarking](https://www.nature.com/articles/s41592-021-01336-8) | Systematic comparison of single-cell RNA-seq cell type annotation methods | Abdelaal et al., 2019 | Nature Methods |
| [A comparison of automatic cell identification methods](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1795-z) | Benchmarking automatic cell identification methods for scRNA-seq | Zhao et al., 2020 | Genome Biology |

## Databases

| Database | Description | Publication | URL |
|----------|-------------|-------------|-----|
| [CellMarker](http://biocc.hrbmu.edu.cn/CellMarker/) | Database of cell markers in different tissues | Zhang et al., 2019 | [Link](http://biocc.hrbmu.edu.cn/CellMarker/) |
| [PanglaoDB](https://panglaodb.se/) | Single-cell RNA sequencing database for expression data | Franzén et al., 2019 | [Link](https://panglaodb.se/) |
| [Cell Ontology](http://www.obofoundry.org/ontology/cl.html) | Structured vocabulary for cell types | Diehl et al., 2016 | [Link](http://www.obofoundry.org/ontology/cl.html) |

## Tutorials and Workflows

| Title | Description | URL |
|-------|-------------|-----|
| [Orchestrating Single-Cell Analysis with Bioconductor](https://bioconductor.org/books/release/OSCA/) | Comprehensive guide to scRNA-seq analysis | [Link](https://bioconductor.org/books/release/OSCA/) |
| [Seurat - Guided Clustering Tutorial](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html) | Tutorial for cell type identification with Seurat | [Link](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html) |

## Community Resources

| Resource | Description | URL |
|----------|-------------|-----|
| [Single Cell Genomics Day](https://www.singlecellgenomicsday.com/) | Annual event dedicated to single-cell genomics | [Link](https://www.singlecellgenomicsday.com/) |
| [Single Cell Omics](https://www.reddit.com/r/singlecellomics/) | Reddit community for single-cell omics discussions | [Link](https://www.reddit.com/r/singlecellomics/) |
| [Bioconductor Single Cell](https://bioconductor.org/packages/release/BiocViews.html#___SingleCell) | Collection of Bioconductor packages for single-cell analysis | [Link](https://bioconductor.org/packages/release/BiocViews.html#___SingleCell) |

## Contributing

We welcome contributions to this repository! Please read our [contributing guidelines](CONTRIBUTING.md) before submitting a pull request.

If you find this resource useful, please consider giving it a ⭐️ star to help others discover it!

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=cafferychen777/awesome-scrna-annotation&type=Date)](https://star-history.com/#cafferychen777/awesome-scrna-annotation&Date)

## License

This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  <i>Keywords: single-cell RNA sequencing, scRNA-seq, cell type annotation, bioinformatics, computational biology, marker genes, reference mapping, machine learning, large language models, cell atlas, cell ontology</i>
</p>