---
layout: page

---

# How to upload to PyPI

This page is mostly intended for my own usage so I don't forget how to do this. 

## Directory

| <project_name>

| | [LICENSE](https://github.com/tulimid1/uploading2pypi/blob/main/LICENSE)

| | [pyproject.toml](https://github.com/tulimid1/uploading2pypi/blob/main/pyproject.toml)

| | [README.md](https://github.com/tulimid1/uploading2pypi/blob/main/README.md)

| | [setup.cfg](https://github.com/tulimid1/uploading2pypi/blob/main/setup.cfg)

| | | <project_name>

| | | | [__init__.py](https://github.com/tulimid1/uploading2pypi/blob/main/__init__.py)

| | | | project_name.py

## Terminal commands 

Go to the directory you just made

`cd <.../proejct_name>`

Build the project 

`pip install build --upgrade` and/or `python -m build`

* This should use the .toml to create some folders (e.g., /dist/ and /<project_name>.egg_info/

Upload dist/*.whl and *.tar.gz

`pip install twine --upgrade` and/or `twine upload dist/*`

