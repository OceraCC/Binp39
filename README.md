
**This tool has not yet been published. So the tool is not accessible for now. But it is an executable instruction once it is published.**

**Installation**

Before using FlaGCsnap, ensure that you have Python installed on your system along with the necessary dependencies.
Follow these steps to install flagcsnap:

1. Create and activate a Conda environment:

```bash
conda create -n flagcsnap python aria2 biopython cctyper treeswift diamond ete3 famsa fasttree infernal ncbi-datasets-cli padloc pandas=1.4.3 requests taxonkit numpy pyarrow==12.0.1 matplotlib defense-finder rich rich-click -c conda-forge -c bioconda -c padlocbio -c russel88   
conda activate flagcsnap
```

2. Clone the repository:
     
```bash
git clone https://github.com/pentamorfico/flagcsnap.git
cd flagcsnap
```
 
3. Install the package:

```bash
python -m pip install -e .
```
 
4. Run script to setup databases and other stuff (this will be done automatically when the conda package is available)

```bash
bash setup.sh 
```
 

**Usage**
1. Prepare the input file

    The example file is available at Github (https://github.com/OceraCC/Binp39/blob/main/terypc.txt).


2. Run FlagCSnap

```bash
flagcsnap --input terypc.txt
```
