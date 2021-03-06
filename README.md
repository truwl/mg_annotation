## Workflow for Metagenome annotation                                                                                                                                                                                                                      
This workflow is based on the JGI/IMG annotation pipeline ([details](https://github.com/kellyrowland/img-omics-wdl)). This is still in progress.  It takes assembled metagenomes and generates structrual and functional annotations.

## Running Workflow in Cromwell

This pipeline is being tested.  Instructions will be posted in the future.

## The Docker image can be found here

[microbiomedata/mg-annotation](https://hub.docker.com/repository/docker/microbiomedata/mg-annotation)


## Input files
expects: fasta

## Output files
```
Multiple GFF files.  More details to come.
```


#### Environment                                                                                                                                                                                                                                                                
 - Linux (with sh/bash)
 - Python >= 3.6 (via conda)
 - Java >= 1.8 (via conda)

#### Third party software used (+ their licenses)
 - Conda (3-clause BSD)
 - tRNAscan-SE >= 2.0 (GNU GPL v3)
 - Infernal 1.1.2 (BSD)
 - CRT-CLI 1.8 (Public domain software, last official version is 1.2, I made changes to it based on Natalia's and David's suggestions)
 - Prodigal 2.6.3 (GNU GPL v3)
 - GeneMarkS-2 >= 1.07 ([Academic license for GeneMark family software](http://topaz.gatech.edu/GeneMark/license_download.cgi))
 - Last >= 983 (GNU GPL v3)
 - HMMER 3.1b2 (3-clause BSD, I am using [Bill's thread optimized hmmsearch](https://github.com/Larofeticus/hpc_hmmsearch))
 - SignalP 4.1 (Academic)
 - TMHMM 2.0 (Academic)

#### Databases used (+ their licenses):
 - Rfam (public domain/CC0 1.0; [more info](http://reusabledata.org/rfam)
 - KEGG (paid subscription, getting KOs/ECs indirectly via IMG NR; [more info](http://reusabledata.org/kegg-ftp)
 - SMART (restrictive license/custom); [more info](http://reusabledata.org/smart)
 - COG (copyright/unlicensed); [more info](http://reusabledata.org/cogs)
 - TIGRFAM (copyleft/LGPL 2.0 or later); [more info](http://reusabledata.org/tigrfams)
 - SUPERFAMILY (permissive/custom); [more info](http://reusabledata.org/supfam)
 - Pfam (public domain/ CC0 1.0); [more info](http://reusabledata.org/pfam)
 - Cath-FunFam (permissive/CC BY 4.0); [more info](http://reusabledata.org/cath)
