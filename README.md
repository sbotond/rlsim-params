## About

This repository holds the **corrected and uncorrected relative expression levels** and **raw parameters** estimated from various datasets by
the [rlsim](http://bit.ly/rlsim-git) [bias analysis pipeline](http://bit.ly/rlsim-pl) using the [effest](http://bit.ly/rlsim-doc) tool.

Additionally, the **uncorrected expression levels** and **FASTQ files** simulated under the *full* and *flat* models are available for download via the **Files** links in the tables below.

### Cloning the repository

Issue the following in order to clone both the fasta files containing the canonical transcriptome augmented with the estimated relative expression levels and the JSON file containing the estimated parameters:

```
git clone https://github.com/sbotond/rlsim-params.git
```

**WARNING: the full size of the repository is approximately 290M! If you are interested in the parameter files only then simply download them through the web.**

### Simulating based on the parameter files

Assuming that you have both the fasta and JSON files cloned and `rlsim` is in the path, you can simulate fragments as:

```
bzcat datasets/ERR030874/ERR030874_expr.fas.bz2 | rlsim -v -j datasets/ERR030874/effest_raw_params.json > fragments.fas
```
### Getting more help

Please consult the `rlsim` [repository](http://bit.ly/rlsim-git), the package [documentation](http://rlsim-doc) and the bias analysis pipeline [repository](http://bit.ly/rlsim-pl) for more help.

### Datasets

*Homo sapiens*

|                         Files                                            |              Info URL            | Read length | PCR cycles| Source                         |
|:----------------------------------------------------------------------------------:|:--------------------------------:|:-----------:|:----------|:-------------------------------|
|[SRR065496](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR065496) | [[details]](http://j.mp/10gF04D) |      75     |     -     | human liver carcinoma (HepG2)  |
|[SRR521457](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR521457) | [[details]](http://j.mp/10gF04D) |      75     |     -     | K562 cell line                 |
|[SRR521448](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR521448) | [[details]](http://j.mp/10gF04D) |      75     |     -     | GM12878 cell line              |
|[ERR030885](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/ERR030885) | [[details]](http://j.mp/10gF8kP) |      50     |     15    | Illumina BodyMap: kidney       |
|[ERR030874](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/ERR030874) | [[details]](http://j.mp/10gF8kP) |      50     |     15    | Illumina BodyMap: ovary        |

*Mus musculus*

|                         Files                                            |              Info URL            | Read length | PCR cycles| Source                         |
|:----------------------------------------------------------------------------------:|:--------------------------------:|:-----------:|:----------|:-------------------------------|
|[SRR040000](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR040000) | [[details]](http://j.mp/10gFhoe) |      76     |     16    | embryonic stem cells           |
|[SRR530635](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR530635) | [[details]](http://j.mp/109cLZI) |101 stranded |     -     | leukemia cell line (K562 analog), dUTP-based stranded protocol|
|[SRR530634](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR530634) | [[details]](http://j.mp/109cLZI) |101 stranded |     -     | leukemia cell line (K562 analog), dUTP-based stranded protocol|
|[ERR120702](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/ERR120702) | [[details]](http://j.mp/10gFpUJ) |      72     |     -     | liver                          |
|[SRR549333](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR549333) | [[details]](http://j.mp/10gFoAj) | 99 stranded |     -     | mouse megakaryocyte erythroid progenitor cells with lineages CD16/32 and CD34, dUTP-based stranded protocol|
|[SRR549337](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR549337) | [[details]](http://j.mp/10gFoAj) | 99 stranded |     -     | mouse megakaryocyte erythroid progenitor cells with lineages CD16/32 and CD34, dUTP-based stranded protocol |
|[SRR496440](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR496440) | [[details]](http://j.mp/10gFyaG) |     100     |     -     | multipotential cell line that can be converted by 5-azacytidine into three mesodermal stem cell lineages |

*Drosophila melanogaster*

|                         Files                                            |              Info URL            | Read length | PCR cycles| Source                         |
|:----------------------------------------------------------------------------------:|:--------------------------------:|:-----------:|:----------|:-------------------------------|
|[SRR042423](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR042423) | [[details]](http://j.mp/10gFGad) |      75     |     -     | 30 third-instar wandering larva|
|[SRR059066](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR059066) | [[details]](http://j.mp/10gFGad) |      75     |     -     | 30 third-instar wandering larva|
|[SRR034309](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR034309) | [[details]](http://j.mp/10gFQOU) |      76     |     -     | mixed stage embryos            |
|[SRR031717](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR031717) | [[details]](http://j.mp/109dj1L) |      37     |     -     | S2-DRSC cell line              |
|[SRR015074](http://www.ebi.ac.uk/goldman-srv/rlsim/datasets/SRR015074) | [[details]](http://j.mp/10gFUOP) |      50     |     -     | CME\_W1\_Cl.8+ cell line       |


[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/148f65c0b66e11e434c4f7d1f892640e "githalytics.com")](http://githalytics.com/sbotond/rlsim-params)
