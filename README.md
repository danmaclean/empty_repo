# empty_repo
An empty repo to base new projects on

In this folder structure you can keep and organise your data, scripts and progress as you work on a well defined project.

The folder should be copied and a new one created every time you have a new project in which all the analyses are linked. 

There is no limit to the number of these folder structures you can have, ideally there will be one for every project.

## The folders

Roughly the folders below are for the following items:

### `analysis`

The actual [literate programming](https://datacarpentry.org/rr-literate-programming/03-explore-knitr/) document that your analysis goes into. Use a sensible naming scheme that reflects the chronological order everything was created in e.g `0001_my_first_idea.Rmd`, or `0002_a_better_one.ipynb`. Using the leading zeroes keeps the documents in the right order in your file browser!

### `scripts`

A folder for scripts. Usually `analysis` and `scripts` work closely together. Documents in `analysis` are the primary code, that in `scripts` is more repetitive code that you use a lot or runs a longer or more specific job. Sometimes this is the place to put 'worker' scripts that the `analysis` documents rely on or that get run only once e.g for downloading data.


### `data`

A clean place to keep generated or downloaded data that you will want to keep. Not a place for large e.g sequence datasets, but rather the results of analysis of those. If the file is large you should think carefully about where to store it, in this folder structure may not be the best idea.

### `lab-book`

This contains a number of dated documents explaining the work done on a particular date, it is a bioinformatics lab book. A document might look like `July-2020.md`. And within that document we might have entries like:

> July 2nd, downloaded genome sequence using `scripts/get_ncbi_genomes.py`, analysed 
> the codon usage as described in `analysis/0032_codon_usage_in_oomycetes.Rmd`. 
> Discovered that none of the sequences use TTT. Consider writing up for Nature.

Correspondingly, your paper lab book can contain: `Worked on bioinformatics project, work in my_repo/lab-book/july-2020.md` 

### README.md

A short description of the work in this repo e.g `oomycete genomics project, a project to uncover which oomycetes have interesting genomes.`

