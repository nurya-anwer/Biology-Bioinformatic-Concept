# Biology-Bioinformatic-Concept
WGS. WES. RNAseq, TPM, RPKM, Basic steps for RNAseq differential expression, Biomarker, IC50 Value measures
1) What are the differences between WGS, WES and RNAseq? Give an example of when you would use each type of sequencing?

Next-Generation Sequencing (NGS) is used in various applications such as examining DNA sequences (whole-genome sequencing (WGS), whole-exome sequencing (WES)), RNA-Sequencing ect.
Whole-genome sequencing determines the order of all nucleotides in an individual’s DNA and can uncover variation in any part of the human genome, including coding, noncoding, and mitochondrial DNA (mtDNA) regions. 
In some instances, WGS is the better option because DNA variations outside protein-coding regions can affect gene activity and protein production, potentially leading to genetic disorders.

Whole-exome sequencing focuses on the genomic proteincoding regions (exons). 
Although the human exome represents only 1-5% of the genome, it contains approximately 85% of known disease-related variants.
1 As such, researchers performing WES achieve comprehensive coverage of coding variants such as single nucleotide variants (SNVs) and insertions/deletions (indels). 
Despite lengthier sample preparation due to the additional target enrichment step, scientists benefit from quicker sequencing and data analysis compared to WGS. 
WES provides greater sequencing depth for researchers interested in identifying genetic variants for numerous applications, including population genetics, genetic disease research, and cancer studies.

RNA-sequencing is a sequencing technique which uses next-generation sequencing (NGS) to reveal the presence and quantity of RNA in a biological sample at a given moment, 
analyzing the continuously changing cellular transcriptome. 
Specifically, RNA-Seq facilitates the ability to look at alternative gene spliced transcripts, post-transcriptional modifications, gene fusion, mutations/SNPs and changes in gene expression over time, 
or differences in gene expression in different groups or treatments.

2) Explain what are the differences between the TPM and RPKM normalization methods.

TPM was introduced in an attempt to facilitate comparisons across samples. TPM stands for transcript per million, and the sum of all TPM values is the same in all samples, such that a TPM value represents a relative expression level that, in principle, should be comparable between samples. The measure RPKM (reads per kilobase of exon per million reads mapped) was devised as a within-sample normalization method; as such, it is suitable to compare gene expression levels within a single sample, rescaled to correct for both library size and gene length. The only difference is that you normalize for gene length first, and then normalize for sequencing depth second. However, the effects of this difference are quite profound. When you use TPM, the sum of all TPMs in each sample are the same. This makes it easier to compare the proportion of reads that mapped to a gene in each sample. In contrast, with RPKM , the sum of the normalized reads in each sample may be different, and this makes it harder to compare samples directly.

3) Describe the basics steps you would need to perform an RNAseq differential expression analysis starting from raw data with treated and control groups.




Part1: Raw sequence processing 1: Quality Control – Run QC on the FastQ file from the sequencer 2: Trimming - Turn the raw fastQ file into a trimmed fastQ file containingonly good quality data 3: Mapping – Take the data in the trimmed fastQ file and map it to areference genome to create a BAM file of mapped positions Part 2: Visualisation, Exploration and Differential Expression 4: Visualisation and Quantitation in treated and control groups. 5: Differential Expression analysis with DESeq2 in treated and control groups. 6: Reviewing DESeq2 results in treated and control groups.

4) Give a brief description of what a biomarker is.

Biomarker: A biological molecule found in blood, other body fluids, or tissues that is a sign of a normal or abnormal process, or of a condition or disease. A biomarker may be used to see how well the body responds to a treatment for a disease or condition. Also called molecular marker and signature molecule.

5) Give a brief description of what an IC50 value measures.

IC50 value of the drug indicates the toxicity of the drug to other disease causing organisms. IC50 is a quantitative measure that shows how much a particular inhibitory drug/substance/extract/fraction is needed to inhibit a biological component by 50%.


Translational bioinformatics is an emerging field that addresses the current challenges of integrating increasingly voluminous amounts of molecular and clinical data.  
Its aim is to provide a better understanding of the molecular basis of disease, which in turn will inform clinical practice and ultimately improve human health.

![image](https://user-images.githubusercontent.com/55751454/140979695-28f921b7-e4cf-40f7-b049-cced4d0e9323.png)

![image](https://user-images.githubusercontent.com/55751454/140956931-6525f20c-a50b-4233-93f8-9fecf9fca7b5.png)
