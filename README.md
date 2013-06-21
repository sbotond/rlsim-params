# About

This repository holds the corrected relative expression levels and raw parameters estimated from various datasets by
the [rlsim](http://bit.ly/rlsim-git) [bias analysis pipeline](http://bit.ly/rlsim-pl) using the [effest](http://bit.ly/rlsim-doc) tool.

## Cloning the repository

Issue the following in order to clone both the fasta files containing the canonical transcriptome and the JSON file containing the estimated parameters:

```
git clone https://github.com/sbotond/rlsim-params.git
```

**WARNING: the full size of the repository is approximately 290M! If you are interested in the parameter files only then simply download them through the web.**

## Simulating based on the parameter files

Assuming that you have both the fasta and JSON files cloned and `rlsim` is in the path, you can simulate fragments as:

```
bzcat datasets/ERR030874/ERR030874_expr.fas.bz2 | rlsim -v -j datasets/ERR030874/effest_raw_params.json > fragments.fas
```
## Getting more help

Please consult the `rlsim` [repository](http://bit.ly/rlsim-git), the package [documentation](http://rlsim-doc) and the bias analysis pipeline [repository](http://bit.ly/rlsim-pl) for more help.

## Datasets

*Homo sapiens*

|                         Parameter files                                            |              Info URL            | Read length | PCR cycles| Source                         |
|:----------------------------------------------------------------------------------:|:--------------------------------:|:-----------:|:----------|:-------------------------------|
|[SRR065496](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR065496) | [[details]](http://j.mp/10gF04D) |      75     |     -     | human liver carcinoma (HepG2)  |
|[SRR521457](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR521457) | [[details]](http://j.mp/10gF04D) |      75     |     -     | K562 cell line                 |
|[SRR521448](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR521448) | [[details]](http://j.mp/10gF04D) |      75     |     -     | GM12878 cell line              |
|[ERR030885](https://github.com/sbotond/rlsim-params/tree/master/datasets/ERR030885) | [[details]](http://j.mp/10gF8kP) |      50     |     15    | Illumina BodyMap: kidney       |
|[ERR030874](https://github.com/sbotond/rlsim-params/tree/master/datasets/ERR030874) | [[details]](http://j.mp/10gF8kP) |      50     |     15    | Illumina BodyMap: ovary        |

*Mus musculus*

|                         Parameter files                                            |              Info URL            | Read length | PCR cycles| Source                         |
|:----------------------------------------------------------------------------------:|:--------------------------------:|:-----------:|:----------|:-------------------------------|
|[SRR040000](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR040000) | [[details]](http://j.mp/10gFhoe) |      76     |     16    | embryonic stem cells           |
|[SRR530635](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR530635) | [[details]](http://j.mp/109cLZI) |101 stranded |     -     | leukemia cell line (K562 analog), dUTP-based stranded protocol|
|[SRR530634](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR530634) | [[details]](http://j.mp/109cLZI) |101 stranded |     -     | leukemia cell line (K562 analog), dUTP-based stranded protocol|
|[ERR120702](https://github.com/sbotond/rlsim-params/tree/master/datasets/ERR120702) | [[details]](http://j.mp/10gFpUJ) |      72     |     -     | liver                          |
|[SRR549333](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR549333) | [[details]](http://j.mp/10gFoAj) | 99 stranded |     -     | mouse megakaryocyte erythroid progenitor cells with lineages CD16/32 and CD34, dUTP-based stranded protocol|
|[SRR549337](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR549337) | [[details]](http://j.mp/10gFoAj) | 99 stranded |     -     | mouse megakaryocyte erythroid progenitor cells with lineages CD16/32 and CD34, dUTP-based stranded protocol |
|[SRR496440](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR496440) | [[details]](http://j.mp/10gFyaG) |     100     |     -     | multipotential cell line that can be converted by 5-azacytidine into three mesodermal stem cell lineages |

*Drosophila melanogaster*

|                         Parameter files                                            |              Info URL            | Read length | PCR cycles| Source                         |
|:----------------------------------------------------------------------------------:|:--------------------------------:|:-----------:|:----------|:-------------------------------|
|[SRR042423](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR042423) | [[details]](http://j.mp/10gFGad) |      75     |     -     | 30 third-instar wandering larva|
|[SRR059066](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR059066) | [[details]](http://j.mp/10gFGad) |      75     |     -     | 30 third-instar wandering larva|
|[SRR034309](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR034309) | [[details]](http://j.mp/10gFQOU) |      76     |     -     | mixed stage embryos            |
|[SRR031717](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR031717) | [[details]](http://j.mp/109dj1L) |      37     |     -     | S2-DRSC cell line              |
|[SRR015074](https://github.com/sbotond/rlsim-params/tree/master/datasets/SRR015074) | [[details]](http://j.mp/10gFUOP) |      50     |     -     | CME\_W1\_Cl.8+ cell line       |

