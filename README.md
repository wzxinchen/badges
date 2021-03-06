## badges

Alternate Location for img.shields.io Badges

### Content
- ![GPL (>=2)](https://eddelbuettel.github.io/badges/GPL2+.svg)  
    - https://eddelbuettel.github.io/badges/GPL2+.svg in lieu of 
    - https://img.shields.io/badge/license-GPL%20%28%3E=%202%29-brightgreen.svg?style=flat

### Background

Many R packages use badges in their (R)markdown sources.  Currently, something "bad" happens between the default
[pandoc](http://pandoc.org/) binary and the [shields.io](https://shields.io) service which provides these badges: 
some sort of TLS handshake goes bad and the processing aborts. 

Which means that at least for now, all R processing of .Rmd or .md files using [pandoc](http://pandoc.org/) and containing 
references to [shields.io](https://shields.io) fails.  Which is not good.  Hence this simple cache.  A first package using
it in its `README.md` is [RcppArmadillo](https://github.com/RcppCore/RcppArmadillo). 

### Coverage Badges

Many README.md files also use https://img.shields.io/codecov to display testing coverage. An alternative is to
use a https://codecov.io/ badge.  As concrete example, for Rcpp we switched from
https://img.shields.io/codecov/c/github/RcppCore/Rcpp/master.svg to
https://codecov.io/gh/RcppCore/Rcpp/graph/badge.svg.

### Author

Dirk Eddelbuettel 
