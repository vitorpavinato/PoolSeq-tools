# PoolSeq-tools

## **Tools for the analyses of whole-genome Pool-seq data.**
It is not my intention to have a comprehensive list. Here I added tools I found useful, tools that others found useful (and tested their performance with simulated and/or real data), tools that were rewritten and maintained by others as an attempt to keep the tool update and easy to use, or tools I think might need some update, maintenance etc.

The first time a software/pipeline/approach appears in this document, I included its webpage link (if available).

### **Pipelines**

[GRENEPIPE](https://github.com/moiexpositoalonsolab/grenepipe) by [Lucas Czech](https://github.com/lczech).

### **Tools for variant calling**

In the context of population genomics studies:
- [MAPGD](https://github.com/LynchLab/MAPGD)
- [SNAPE-pooled](https://github.com/EmanueleRaineri/snape-pooled)
- [PoolSNP](https://github.com/capoony/PoolSNP)
- [VarScan](http://varscan.sourceforge.net)

In the context of association studies:
- [CRISP](https://github.com/vibansal/crisp/)
- [SNPSeeker](http://genetics.wustl.edu/rmlab/software/)
- [SNVer](http://snver.sourceforge.net)
- [EM-SNP](https://dornsife.usc.edu/labs/fsun/programs/)

### **Tools for the estimation of population allele frequencies**
- [Popoolation](https://github.com/lczech/popoolation)
- [Popoolations2](https://sourceforge.net/p/popoolation2/wiki/Manual/) for the original implementation.
- [Poopolations2](https://github.com/lczech/popoolation2) for the re-implementation by [Lucas Czech](https://github.com/lczech)
- [Pool-HMM](https://forge-dga.jouy.inra.fr/projects/pool-hmm) for the original implementation.
- [Pool-HMM](https://github.com/lczech/PoolHMM)  for the re-implementation by [Lucas Czech](https://github.com/lczech)

### **Tools for the estimation of the allele frequency spectrum (folded and unfolded)**
- Pool-HMM

> ### Note on how these methods account for sequencing errors:
> - No error: Poopolation 1 & 2, PIFs;
> - Arbitrary choice: SNVer;
> - Estimate it from tri-allelic sites: MAPGD;
> - Estimate it using multiple pools: EM-SNP;
> - Trust PHRED score: Pool-HMM, Psafe?, SNAPE-pooled;
> - Estimate using a known control sequence: SNPSeeker;

### **Tools for the analyses of time-series genomic data**

Tools to look for signature of selection (directional selection)

- [LLS](https://github.com/ThomasTaus/poolSeq)
- [CLEAR](https://github.com/airanmehr/clear)
- [poolFreqDiff](https://github.com/RAWWiberg/poolFreqDiff)
- [poolSeq](https://github.com/ThomasTaus/poolSeq)

Tools for demographic inference ($N_e$)
- [NEST](https://github.com/ThomasTaus/Nest)

### **Tools for inference of selection in single-point or time-series genomic data**
- Pool-HMM & Freq-HMM
- Poopolation 1 & 2

### **Tools for the analyses of single-point genomic data**

For the calculation of summary statistics
- [Poolfstat](https://rdrr.io/cran/poolfstat/) 
It was the first implementation of unbiased $F_{ST}$ estimator of Weir & Cockerham $\theta$ for Pool-seq data. Recently it grew and incorporated many cool modern population genetics statistics for admixture analysis (Patterson's 'F2', 'F3', 'F3*', 'F4' and D parameters). It also has functions for the fitting, building and visualization of admixture graphs.

- Popoolation
- Popoolation2
- [Npstat](https://github.com/lucaferretti/npstat)
- [grenedalf](https://github.com/lczech/grenedalf)
- [PIXY](https://github.com/ksamuk/pixy)

For admixture graphs
- Poolfstat

For demographic model inference 
- [Moments](https://moments.readthedocs.io/en/latest/introduction.html) based on the SFS
- [TREEMIX](https://bitbucket.org/nygcresearch/treemix/src)
- [Stairway2](https://github.com/xiaoming-liu/stairway-plot-v2)
- [∂a∂i](https://bitbucket.org/gutenkunstlab/dadi)

For the identification of selective sweeps (hard sweeps)
- Pool-HMM with LOCAL SCORES
- [SelEstim](http://www1.montpellier.inra.fr/CBGP/software/selestim/index.html)

For the identification of selection in CNVs
- [poolDiffCNV](https://github.com/andrewkern/poolDiffCNV)

For signature of selection using association methods (usually with environmental correlation)
- [SAMBADA](http://lasig.epfl.ch/sambada)
- [PCAdapt](http://membres-timc.imag.fr/Michael.Blum/PCAdapt.html)
- [BAYPASS](http://www1.montpellier.inra.fr/CBGP/software/baypass/)

For the estimation of linkage disequilibrium statistics
- [LDx](https://sourceforge.net/p/ldx/wiki/User%20Manual/)
- MAPGD

For the inference of the recombination landscape
- [RELERNN](https://github.com/kr-colab/ReLERNN)

## **Tools for the analyses of transposable elements**

Transposable elements calling and diversity statistics
- [PopoolationTE](https://sourceforge.net/projects/popoolationte/). This tool works for the analysis of TE insertions.
- [PopoolationTE2](https://sourceforge.net/p/popoolation-te2/wiki/Home/). This tool is for comparative analyzes among samples.
- [TEMP](https://github.com/JialiUMassWengLab/TEMP)
- [RetroSeq](https://github.com/tk2/RetroSeq)
- [VariationHunter](http://variationhunter.sourceforge.net/Home)
- [GASVPro](http://code.google.com/p/gasv/)

## **TODO's**
> <mark style="background-color: #FFFF00"> - Write SNAPE in C++ </mark>