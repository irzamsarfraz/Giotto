
<!-- README.md is generated from README.Rmd. Please edit that file -->
Giotto
======

<!-- badges: start -->
<!-- badges: end -->
The goal of Giotto is to process, analyze and visualize **single-cell spatial transcriptomic** data. Simultaneously this package contains the data that was used in the recent [**seqFISH+**](https://www.nature.com/articles/s41586-019-1049-y) paper and can thus be used to explore or re-analyze this dataset.

 

Requirements
------------

-   R (&gt;= 3.5.1)
-   Python (&gt;= 3.0)
-   Unix/Linux

 

Installation
------------

#### R installation

You can install the development version of Giotto with:

``` r
library(devtools)
install_github("RubD/Giotto")
```

Future plan:

``` r
install.packages("Giotto")
```

#### Python tools (optional)

This is necessary to run all available analyses, including Leiden / Louvain clustering and to build and use the interactive visualization tool. An alternative, but less flexible, R version for Louvain clustering is also available. It is advisable to install everything within a specific conda environment and specify the python path in the R function when required.

Required python modules:
- pandas
- igraph
- networkx
- leidenalg
- community

Future plan:

``` python
conda install GioTools
```

#### HMRF

See [**HMRF**](http://www.nature.com/articles/nbt.4260) installation [instructions](http://spatial.rc.fas.harvard.edu/install.html).

 

Examples
--------

[<img src="./inst/images/cortex_image_summary.png" alt="Cortex" width="377" />](./inst/examples/mouse_cortex_svz/mouse_cortex_example.md) [<img src="./inst/images/OB_image_summary.png" alt="OB" width="377" />](./inst/examples/mouse_olfactory_bulb/mouse_olfactory_bulb_example.md)

 

Latest News
-----------

-   First release (beta)
-   ...

 

FAQ
---

Coming soon ...

-   Cortex/SVZ and olfactory bulb data availability?
-   How to create a giotto object with your own spatial network/grid, dimensions reduction, ... ?
-   How to make full use of giotto object flexibility?
-   ...

 

References
----------

-   Eng, C.-H. L. et al. Transcriptome-scale super-resolved imaging in tissues by RNA seqFISH+. Nature 1 (2019). <doi:10.1038/s41586-019-1049-y>

-   Zhu, Q., Shah, S., Dries, R., Cai, L. & Yuan, G.-C. Identification of spatially associated subpopulations by combining scRNAseq and sequential fluorescence in situ hybridization data. Nature Biotechnology (2018). <doi:10.1038/nbt.4260>