# `forest-confidence-interval`: Confidence intervals for Forest algorithms

[![Travis Status](https://travis-ci.org/scikit-learn-contrib/forest-confidence-interval.svg?branch=master)](https://travis-ci.org/scikit-learn-contrib/forest-confidence-interval)
[![Coveralls Status](https://coveralls.io/repos/scikit-learn-contrib/forest-confidence-interval/badge.svg?branch=master&service=github)](https://coveralls.io/r/scikit-learn-contrib/forest-confidence-interval)
[![CircleCI Status](https://circleci.com/gh/scikit-learn-contrib/forest-confidence-interval.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/scikit-learn-contrib/forest-confidence-interval/tree/master)

Forest algorithms are powerful
[ensemble methods](http://scikit-learn.org/stable/modules/classes.html#module-sklearn.ensemble) for classification and regression. However, predictions from these
algorithms do contain some amount of error.

`forest-confidence-interval` is a Python module that adds a calculation of
variance and computes confidence intervals to the basic functionality
implemented in scikit-learn random forest regression or classification objects.
The core functions here calculate an in-bag and error bars for random forest
objects

Compatible with Python2.7 and Python3.6

This module is based on R code from Stefan Wager (see important links below)
and is licensed under the MIT open source license (see [LICENSE](LICENSE))

## Important Links
scikit-learn - http://scikit-learn.org/

Stefan Wager's `randomForestCI` - https://github.com/swager/randomForestCI

## Installation and Usage
Before installing the module you will need `numpy`, `scipy` and `scikit-learn`.  
Dependencies associated with the previous modules may need root privileges to install
```
pip install numpy scipy scikit-learn
```
can also install dependencies with:

```
 pip install -r requirements.txt
 ```

To install `forest-confidence-interval` execute:
```
pip install forestci
```

or, if you are installing from the source code:
```shell
python setup.py install
```

If would like to install the development version of the software use:

```shell
pip install git+git://github.com/scikit-learn-contrib/forest-confidence-interval.git
```

## Examples
See [examples gallery](http://contrib.scikit-learn.org/forest-confidence-interval/auto_examples/index.html)

## Contributing

Contributions are very welcome, but we ask that contributors abide by the
[contributor covenant)[http://contributor-covenant.org/version/1/4/].

To report issues with the software, please post to the
[issue log](https://github.com/scikit-learn-contrib/forest-confidence-interval/issues)
Bug reports are also appreciated, please add them to the issue log after
verifying that the issue does not already exist.
Comments on existing issues are also welcome.

Please submit improvements as pull requests against the repo after verifying
that the existing tests pass and any new code is well covered by unit tests.
Please write code that complies with the Python style guide,
[PEP8](https://www.python.org/dev/peps/pep-0008/)

## Testing
Requires installation of `nose` package. Tests are located in the `forestci/tests` folder
and can be run with the `nosetests` command in the main directory
