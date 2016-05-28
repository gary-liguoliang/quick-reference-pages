
### Building

#### woking locally in 'development' mode

```python
pip install -e .
```

`-e` is short for `--editable`, `.` refers to the current directory. it installs the current directory in editable model by creating a `.egg-link` in the deployment directory which links to your project.

#### packaging project


** source distribution**
a `source distribution` is not a built distribution, and requires a built step when installed by `pip`.

```python
python setup.py sdist
```

### Distributing to PyPI

before releasing to PyPI repo, you need [setup your account](http://python-packaging-user-guide.readthedocs.io/en/latest/distributing/#uploading-your-project-to-pypi)

#### Upload distribution

```python
twine upload dist/*
```
