# ChromoSSE: Cladogenetic and Anagenetic Models of Chromosome Number Evolution

This repository contains the scripts used to run the ChromoSSE phylogenetic models of
chromosome number evolution.
These models allow one to infer the mode of chromosome number evolution; 
is chromosome evolution occurring primarily within lineages, 
primarily at lineage splitting, 
or in clade-specific combinations of both? 
Furthermore, they estimate the location and timing of possible chromosome speciation events over the phylogeny
as well as ancestral chromosome numbers.

ChromoSSE was implemented in a Bayesian statistical framework, 
specifically in the software [RevBayes](http://revbayes.com), 
to accommodate uncertainty in parameter estimates while leveraging the full power of likelihood based methods. 
Provided here are the Rev scripts needed to run ChromoSSE in [RevBayes](http://revbayes.com).
Please modify these scripts to use your own data,
and feel free to contact me with any questions.

### Requirements:

Please make sure you are using RevBayes v1.0.7 or greater. Some Rev language functions
have changed and earlier versions will not work.

### Tutorial:

I've written a tutorial on how to use RevBayes for a wide range of chromosome evolution analyses using ChromEvol, BiChroM, ChromoSSE and other related models:

* [Tutorial (pdf)](https://github.com/revbayes/revbayes_tutorial/raw/master/tutorial_TeX/RB_Chromosome_Evolution_Tutorial/RB_Chromosome_Evolution_Tutorial.pdf) 
* [Example scripts](http://rawgit.com/revbayes/revbayes_tutorial/master/RB_Chromosome_Evolution_Tutorial/scripts.zip) 
* [Example data](http://rawgit.com/revbayes/revbayes_tutorial/master/RB_Chromosome_Evolution_Tutorial/data.zip) 

### Citation:

Freyman, W.A. and S. Höhna. 2017. Cladogenetic and anagenetic models of chromosome number evolution: a Bayesian model averaging approach. *Systematic Biology* syx065
[[preprint]](http://biorxiv.org/content/early/2016/11/16/086629)
[[journal]](https://academic.oup.com/sysbio/article-abstract/67/2/195/4037179)
[[pdf]](https://willfreyman.org/assets/pdf/2017_Freyman_and_Hoehna.pdf)

### To run an example ChromoSSE analysis:

```
cd examples/aristolochia/
rb aristolochia_analysis.Rev
```

### To plot the output of a ChromoSSE analysis:

Use the [RevGadgets](https://github.com/revbayes/RevGadgets) R package
and [this example R script](plot_results.R) to generate figures like this:

![ChromoSSE plot](examples/aristolochia/data/aristolochia_ancestral_states.jpg)

### Contact:

Will Freyman, UC Berkeley   
willfreyman@gmail.com  
[http://willfreyman.org](http://willfreyman.org)

### Other stuff:

Copyright 2016 Will Freyman     
License: GNU GPLv3 http://www.gnu.org/licenses/gpl.html
