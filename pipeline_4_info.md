RNA-seq is a technology that examines the whole transcriptome at unprecedented levels of sensitivity. There are a wide range of applications for RNA-seq, from **expression quantification**, **discovery of novel genes** and **gene isoforms**, **differential expression**, and many other types of **functional analysis**.
<br/><br/>

Our **Expression count (STAR) pipeline** is a expression quantification pipeline, wherein you can quantify your rna-seq reads against the reference genome (**[list of supported genome](https://app.basepairtech.com/genomes/)**), the result of this pipeline could be later used for differential expression analysis.

### Brief Methodology:

The analysis begins with quality filtering the input sequencing reads (FASTQ files). The low quality reads and adaptor sequences are removed using [**fastp**](https://academic.oup.com/bioinformatics/article/34/17/i884/5093234). After trimming, reads are aligned to the **reference genome** using [**star**](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3530905/) aligner. The next step is to quantify gene expression. The number of reads that align to each gene is quantified using [**featureCounts**](https://academic.oup.com/bioinformatics/article/30/7/923/232889).

### Input:
**- fastq / bam**

### Output:

##### [**Example Analysis Link**](https://app.basepairtech.com/analyses/30884)

##### Average Run Time : ~20 mins

