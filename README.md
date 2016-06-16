# Fennec 

Fennec is a simple data analysis toolbox in python.

## Installation

```bash
pip install --upgrade git+https://github.com/amaotone/fennec.git
```

## Usage

### Import
```python
import fennec as fn
```

### Workspace Manager

`fennec.Workspace` will make `./results/category/[timestamp]_name` folder for workspace.

```python
workspace = fn.Workspace("category/name")
```

This class enable us to put results in the same folder with time stamp for each trial.
It prevend results from vanishing or overwriting.

#### Logging
Add log to the workspace.

```python
workspace = fn.Workspace("category/name")
workspace.log("hello world")
```

#### Get Path
When you call `fennec.Workspace`, you'll get absolute path
to the file in the workspace.

```python
import fennec as fn
workspace = fn.Workspace("category/experiment")
print(workspace())
print(workspace("result.log"))
```

## License

MIT license (see `LICENSE` file)