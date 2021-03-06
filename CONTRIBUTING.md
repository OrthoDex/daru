# Contributing guide

## Installing daru development dependencies

Either nmatrix or rb-gsl are NOT NECESSARY for using daru. They are just required for an optional speed up and for running the test suite.

To install dependencies, execute the following commands:

  `sudo apt-get update -qq`
  
  `sudo apt-get install -y libgsl0-dev r-base r-base-dev`
  
  `sudo Rscript -e "install.packages(c('Rserve','irr'),,'http://cran.us.r-project.org')"`


Then install remaining dependencies:

  `bundle install`

And run the test suite (should be all green with pending tests):

  `bundle exec rspec`

If you have problems installing nmatrix, please consult the [nmatrix installation wiki](https://github.com/SciRuby/nmatrix/wiki/Installation) or the [mailing list](https://groups.google.com/forum/#!forum/sciruby-dev).

## Daru internals

To get an overview of certain internals of daru and their implementation, go over [this blog post](http://v0dro.github.io/blog/2015/08/16/elaboration-on-certain-internals-of-daru/).
