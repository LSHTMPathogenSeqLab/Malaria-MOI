# Malaria-MOI

## Introduction

This is a tool to estimate multiplicity of infection (MOI) from BAM and VCF inputs. This is particularly useful in the context of malaria. Compatible with python=3.11.

## Installation

```
conda create -n malariaMOI python=3.11
git clone https://github.com/LSHTMPathogenSeqLab/Malaria-MOI.git
cd /path/to/Malaria-MOI
pip install -e .
```

## Usage

```
malariaMOI --bam <input_bam> --vcf <input_vcf> --outfile <output_json_file>
```

## Help

```
usage: malariaMOI [-h] --bam BAM --vcf VCF --outfile OUTFILE [--maxdist MAXDIST] [--min_count MIN_COUNT]

A simple command line tool for Moi

options:
  -h, --help            show this help message and exit
  --bam BAM             BAM (or cram) file
  --vcf VCF             VCF file
  --outfile OUTFILE     Name of output file
  --maxdist MAXDIST     Maximum distance between the first and last SNP
  --min_count MIN_COUNT
                        Minimum count of haplotype
```
