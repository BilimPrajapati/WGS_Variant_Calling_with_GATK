# WGS_Variant_Calling_with_GATK

This repo contains a complete workflow for identifying variants—including SNPs and indels—from whole genome sequencing (WGS) data. Following GATK best practices, this guide demonstrates how to build a reproducible pipeline using Bash on a Linux system. The workflow spans all essential steps, from raw sequencing reads to downstream analysis:

Quality Control: Evaluate raw sequencing data using FastQC.
Read Alignment: Align reads to the reference genome with BWA-MEM.
Preprocessing: Mark duplicate reads and perform Base Quality Score Recalibration (BQSR).
Variant Calling: Generate GVCFs for each sample using GATK HaplotypeCaller.
Genotyping and Merging: Combine GVCFs and perform joint genotyping with GenotypeGVCFs.
Annotation: Annotate variants using SnpEff to predict functional effects.
Population Analysis: Calculate Fst for population differentiation analysis.

This step-by-step pipeline enables reproducible generation of high-quality variant calls and downstream analyses from WGS data.
