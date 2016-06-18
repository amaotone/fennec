![build](https://travis-ci.org/amaotone/fennec.svg?branch=master)
[![Code Climate](https://codeclimate.com/github/amaotone/fennec/badges/gpa.svg)](https://codeclimate.com/github/amaotone/fennec)
[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)

# Fennec

Fennec is a simple data analysis toolbox with python.

## Installation

```bash
pip install --upgrade git+https://github.com/amaotone/fennec.git
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
