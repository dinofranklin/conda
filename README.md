# Conda environment with environment.yml

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dinofranklin/conda/master?filepath=index.ipynb)

A Binder-compatible repo with an `environment.yml` file.

Access this Binder at the following URL:

https://mybinder.org/v2/gh/dinofranklin/conda/master?filepath=index.ipynb


## Notes

This repository is a fork from https://github.com/binder-examples/conda modified exclusively to support GBC063/UFU classes.

The `environment.yml` file should list all Python libraries on which your notebooks
depend, specified as though they were created using the following `conda` commands:

```
source activate example-environment
conda env export --no-builds -f environment.yml
```

Note that the only libraries available to you will be the ones specified in
the `environment.yml`, so be sure to include everything that you need! 

Also note that conda will possibly try to include OS-specific packages in `environment.yml`, so you
may have to manually prune `environment.yml` to get rid of these packages. Confirmed Mac-OSX-specific
packages that should be removed are:

* libcxxabi=4.0.1
* appnope=0.1.0
* libgfortran=3.0.1
* libcxx=4.0.1
