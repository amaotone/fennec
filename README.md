[![PyPI](https://img.shields.io/pypi/v/fennec.svg?maxAge=2592000)](https://pypi.python.org/pypi/fennec)
![Python Versions](https://img.shields.io/badge/python-3.4%2C%203.5-blue.svg)
[![Build Status](https://travis-ci.org/amaotone/fennec.svg?branch=master)](https://travis-ci.org/amaotone/fennec)
[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)

# Fennec

Fennec is a simple toolbox for statistical analysis with python.

## Dependencies

- Minimal
    - Python 3.4, Python 3.5
- Workspace
    - pytz
- Testing
    - py.test
    - tox

## Installation

```bash
pip install fennec
```

## Usage

### Import

```python
import fennec as fn
```

### Workspace

`fennec.Workspace` will make `./results/category/[timestamp]_name` folder for workspace.

This class enable us to put results in the same folder with time stamp for each trial.
It prevend results from vanishing or overwriting.


```python
import fennec as fn

# make workspace
workspace = fn.Workspace("category/name")

# logging
workspace.log("hello world")

# get path
print(workspace())
print(workspace("result.log"))
```

## License

MIT license (see `LICENSE` file)
