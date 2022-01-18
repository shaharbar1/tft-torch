[comment]: <> (Modify also docs/installation.rst if change the README.md)

[comment]: <> (Modify also LICENSE.rst if change the README.md)

tft-torch
=====

[comment]: <> (Modify also docs/badges.rst if you change the badges)

[comment]: <> (Modify also LICENSE.rst if you change the license)
![alt text](https://img.shields.io/badge/build-passing-brightgreen)
![alt text](https://img.shields.io/badge/docs-passing-brightgreen)
![alt text](https://img.shields.io/badge/version-0.0.1-blue)
![alt text](https://img.shields.io/badge/license-MIT-blue)

**tft-torch** is a ``Python`` library that
implements <cite>["Temporal Fusion Transformers for Interpretable Multi-horizon Time Series Forecasting"][1]</cite>
using pytorch framework. The library provides a complete implementation of a time-series multi-horizon forecasting model
with state-of-the-art performance on several benchmark datasets.

This library works for Python 3.7 and higher and PyTorch 1.6.0 and higher.

Installation
------------
This library is distributed on [PyPi](missing_url) and can be installed using ``pip``.
<span style="color:red">Still need to take care of this</span>.

~~~~~~~~~~~~~~~~~~~~~~
$ pip install tft-torch 
~~~~~~~~~~~~~~~~~~~~~~

The command above will automatically install all the required dependencies. Please visit the
[installation](needs_to_be_fixed) page for more details.

<span style="color:red">Still need to take care of this</span>.


Getting started
---------------
Check out the tutorial **place link** for a demonstration how to use the library.
<span style="color:red">Still need to take care of this</span>.


Documentation
-------------
For more information, refer to our
[blogpost](broken_link)
and
[complete documentation](broken_link).



# Reference

This repository suggests an implementation of a model based on the work presented in the following paper:

```
@misc{lim2020temporal,
      title={Temporal Fusion Transformers for Interpretable Multi-horizon Time Series Forecasting}, 
      author={Bryan Lim and Sercan O. Arik and Nicolas Loeff and Tomas Pfister},
      year={2020},
      eprint={1912.09363},
      archivePrefix={arXiv},
      primaryClass={stat.ML}
}
```
Some parts of the implementation rely on [mattsherar](https://github.com/mattsherar)'s TFT implementation, available as part of the [Temporal_Fusion_Transform](https://github.com/mattsherar/Temporal_Fusion_Transform) repository.

[1]: https://arxiv.org/abs/1912.09363


Info for developers
-------------------

The source code of the project is available on [GitHub](https://github.com/PlaytikaResearch/tft-torch).

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
$ git clone https://github.com/PlaytikaResearch/tft-torch.git
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can install the library and the dependencies with one of the following commands:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
$ pip install .                        # install library + dependencies
$ pip install ".[develop]"             # install library + dependencies + developer-dependencies
$ pip install -r requirements.txt      # install dependencies
$ pip install -r requirements-dev.txt  # install developer-dependencies
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To create the file ``*.whl`` for the installation with ``pip`` run the following command (at the root of the
repository):

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
$ python -m build
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To create the HTML documentation run the following commands:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
$ cd docs
$ make clean
$ make html
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Run tests
---------

Tests can be executed with ``pytest`` running the following commands:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
$ cd tests
$ pytest                                      # run all tests
$ pytest test_testmodule.py                   # run all tests within a module
$ pytest test_testmodule.py -k test_testname  # run only 1 test
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~



License
-------

[MIT License](LICENSE)
