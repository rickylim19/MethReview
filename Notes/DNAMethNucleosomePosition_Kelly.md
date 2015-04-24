# Genome-wide mapping of nucleosome positioning and DNA methylation within individual DNA molecules

## Take-home message:

* Using 20bp-windows in DNAmeth to study links with nucleosomal positioning
* 20bp:< than average distance of adjacent GCs enough for nucleosome positioning
* 
## Abstract

* DNAMeth + Nucleosome positioning `->` gene expression
* Developed a new method, NOMe-seq:
    * genome-wide footprint of nucleosome and DNAmeth
    * Using GpC methyltransferases (M.CviPI) + nextGen seq
    * +: less material, < 1 million cells
* anticorrelation of nucleosomalOccup and DNAmeth at CTCF regions, not promoters
* This anticorrelation is not present at promoters
* Evidence for expressed non-CpG promoters are nucleosome-depleted

## Introduction

* Active promoters: lack nucleosomes prior to TSS, unmethylated DNA
* Inactive promoters: densed nucleosomes, unmethylated DNA (poised/repressed), 
                                        , methyhlated DNA (silent) 
* NOMe-seq: Nucleosome occupancy and Methylation sequencing
* NDR: Nucleosome Depleted Region
* Result: Identification of genes likely to be in two divergent allelic states
* These two allelic genes are enriched on the X chr and at know imprinted loci

## Results

* NOMe-seq:
    - M.CviPI methylates GpC not protected by nucleosomes
    - Bisulfite conversion 
    - Note that methylated cytosines protected from conversion to uracil 
        - cytosines within GpC `->` nucleosome positioning
        - cytosines within CpG `->` methylation information
    - Nucleosome occupancy and DNA methylation information:
        - the fraction of methylated reads/all reads covering that position
        - combining CpG and GpC methylation profiles
    - DNA methylation from CpG dinucleotides
    - Nucleosome occupancy from inaccessibility of GpC 
    - 4 possible chromatin configurations:
        - unmethylated & nucleosome-depleted
        - unmethylated & nucleosome-occupied
        - methylated & nucleosome-occupied
        - methylated & nucleosome-depleted
    - Analysis on:
        - GCH: nucleosome accessibility
        - HCG: methylation
        - *H*: C, T, or A
    - Analysis on CpG and non-CpG promoters (figure 2D, 2E):
        - NDR upstream and downstream of TSS is > apparent in CpG than non-CpG
    - CTCF sites, anticorrelation between DNAmeth and nucleosomal occupancy
        - DNA methylation peaks in the linker region between nucleosomes
        - CTCF flanked by well-positioned nucleosomes w/ DNAmethPeaks in between
        - CTCF in IMR90 (Lung fibroblast) and GBM (GlioBlastoma)
        - Promoter H3K4me3 (active): unmethylated DNA and NDR
        - Promoter H3K27me3 (poised): unmethylated DNA and nucleosome occupancy
        - Promoter methylated: methDNA and nucleosome occupancy
        - CpG promoter: 
            - lack of CpG meth 
            - upstream NDR 
            - well-position nucleosome after TSS
        - Non-CpG promoter:
            - CpG methylation
            - nucleosome occupancy
    - Identification of DCA genes (Divergent Chromatin Alles)
        - DCA genes with two combinations:
            - Methylated and Nucleosome inaccessibility
            - Unmtehylated and Nucleosme accessibility
        - Using the within reads analysis compared to the population reads:
            - Within reads: the same reads for methylation and nucleosome methy
            - Population reads: randomly select reads within same positions
    - NOMEseq advantages:
        - identify both meth and nucleosome position simulataneously
        - combination of meth and nucleosome `->` identify combinatorial profile
            within the population of cells
        - Identification of combinatorial profile > sensitivity than using
            two assays in isolation
