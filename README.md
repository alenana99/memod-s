# `memod-s`

> **Note**

> An easy-to-use workflow for generating BLAH BLAH

![Snakemake](https://img.shields.io/badge/Snakemake-%3E%3D5.10.0%2C%3C5.31.1-green?style=for-the-badge) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white) ![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white) ![Bash](https://img.shields.io/badge/bash-%234EAA25.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

Hi :blush:

`memod-s` is a Snakemake workflow that BLAH BLAH

## ⚙️ Installation

You can start using `memod-s` on your cluster with just one line of code with the [mamba package manager](https://github.com/mamba-org/mamba)

```
mamba create -n memod -c bioconda memod
```

This will create an environment called `memod` and start installing dependencies.

## 🔧 Usage

Clone this repo

```
git clone https://github.com/alenana99/memod_snake.git
```

Run `memod-s` with --help or -h arguments to see usage instructions:

```
python memod-s --help
```
```
Usage: memod-s [-h] -i INPUT_DIRECTORY [-o OUTPUT_DIRECTORY] [-dm DORADO_MODELS [DORADO_MODELS ...]] [-ml FILTLONG_MIN_LENGTH]
               [-kp FILTLONG_KEEP_PERCENT] [-rr RACON_ROUNDS] [-mr MEDAKA_ROUNDS] [-mm MEDAKA_MODEL] [-ed EGGNOG_DB] [-q]

Process files for downstream analysis.

Options:
  -h, --help            show this help message and exit
  -i INPUT_DIRECTORY, --input_directory INPUT_DIRECTORY
                        Specify the input directory containing fast5 or pod5 files
  -o OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
                        Specify the output directory (default: ./memod)
  -dm DORADO_MODELS [DORADO_MODELS ...], --dorado_models DORADO_MODELS [DORADO_MODELS ...]
                        Specify a list of Dorado models
  -ml FILTLONG_MIN_LENGTH, --filtlong_min_length FILTLONG_MIN_LENGTH
                        Specify Filtlong minimum length
  -kp FILTLONG_KEEP_PERCENT, --filtlong_keep_percent FILTLONG_KEEP_PERCENT
                        Specify Filtlong percent
  -rr RACON_ROUNDS, --racon_rounds RACON_ROUNDS
                        Specify racon rounds
  -mr MEDAKA_ROUNDS, --medaka_rounds MEDAKA_ROUNDS
                        Specify medaka rounds
  -mm MEDAKA_MODEL, --medaka_model MEDAKA_MODEL
                        Specify medaka model
  -ed EGGNOG_DB, --eggnog_db EGGNOG_DB
                        Specify EggNOG database path
  -q, --quiet           Minimal standard output

```

## 🐍 Workflow

### Core

1. Convert fast5 files to pod5 with [Pod5 File Format Documentation](https://pod5-file-format.readthedocs.io/en/latest/docs/tools.html#pod5-convert-fast5)
2. Download specific methylation models with Dorado. Check the [avaiable basecalling models](https://github.com/nanoporetech/dorado?tab=readme-ov-file#available-basecalling-models)
3. Basecalling with [Dorado](https://github.com/nanoporetech/dorado)
4. Map reads to reference with minimap2
5. Quality check with
6. Quality filtering with
7. Quality check after fitlering 
8. Assembly with dragonflye
9. Assembly evaluation with quast
10. Genome annotation with prokka
11. Functional annotation with eggnog
12. Call methylation with [MicrobeMod](https://github.com/cultivarium/MicrobeMod)
13. MeStudio 
14. Circular density plot for each motif with 
15. Gene Set Enrichment Analysis with fgsea

### Bonus

1.  Abricate 

## 🖇️ Publications

The `memod-s` workflow BLAH BLAH

```
NOSTRO ARTICOLO
```
```
