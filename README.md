## Description

arxivcheck is a module of [bibcure](https://github.com/bibcure/bibcure)
and [scihub2pdf](https://github.com/bibcure/scihub2pdf)
![](https://raw.githubusercontent.com/bibcure/logo/master/gifs/arxivcheck.gif) 

## Install

```
$ sudo python /usr/bin/pip install arxivcheck
```

or if you want the full version

```
$ sudo python /usr/bin/pip install bibcure
```

## Features and how to use


Given a arxiv id...

```
$ arxivcheck 1601.02785
```

Given a arxiv title
```
$ arxivcheck -t Periodic Table of Topological
```

Given a file of titles or ids
```
$ arxivcheck -i  arxivs.txt
```
*  check if has been published, and then returns the updated bib

return outputs like

```
@article{2007Karianearxiv:math/0703567v2,
     author = {Kariane Calta and John Smillie},
     journal = {arxiv:math/0703567v2},
     title = {Algebraically periodic translation surfaces},
     url = {http://arxiv.org/abs/math/0703567v2},
     year = {2007}
}

@article{Bradlyn_2016,
  	doi = {10.1126/science.aaf5037},
  	url = {https://doi.org/10.1126%2Fscience.aaf5037},
  	year = 2016,
  	month = {jul},
  	publisher = {American Association for the Advancement of Science ({AAAS})},
  	volume = {353},
  	number = {6299},
  	pages = {aaf5037},
  	author = {Barry Bradlyn and Jennifer Cano and Zhijun Wang and M. G. Vergniory and C. Felser and R. J. Cava and B. Andrei Bernevig},
  	title = {Beyond Dirac and Weyl fermions: Unconventional quasiparticles in conventional crystals},
  	journal = {Science}
}

```

## bibcure

```
$ bibcure -i input.bib -o output.bib
```

Given a bib file...

* check sure the Arxiv items have been published, then update them(requires
internet connection)

* complete all fields(url, journal, etc) of all bib items using DOI number(requires
internet connection)

* find and create DOI number associated with each bib item which has not
DOI field(requires
internet connection)

* abbreviate jorunals names

```
$ doitobib 10.1038/s41524-017-0032-0
```

Given a DOI number...

* get bib item given a doi(requires
internet connection)

```
$ titletobib An useful paper
```

Given a title...

* search papers related and return a bib for the selected paper(requires
internet connection)
