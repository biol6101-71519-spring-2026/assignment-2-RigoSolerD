# Assignment 2 Report
# Overall Read Quality

Read quality was evaluated using FastQC and summarized with MultiQC. 
Based on the reports, the overall sequence quality was generally good. Most base quality scores remained 
in the high range. GC content and sequence length distribution appeared consistent and did not show major problems. 
From this analysis, the FASTQ files appear to be of sufficient quality for downstream alignment and analysis.

# Mapping Rates

Reads were aligned to the reference genome using Bowtie2, and alignment statistics were generated using `samtools flagstat`. 
A total of 200,000 reads were processed, and 140,854 reads successfully mapped to the reference genome, 
resulting in an overall mapping rate of 70.43%. This indicates that the majority of reads aligned to the reference, 
but not all reads were successfully mapped.

# Quality Concerns

The mapping rate was 70.43%. Only 12.73% of reads were properly paired, which may indicate differences between the sequencing data 
and the reference genome. While the data were sufficient to generate sorted BAM files and alignment statistics, the mapping rate 
suggests that further preprocessing or verifying the reference genome compatibility could potentially improve alignment results.