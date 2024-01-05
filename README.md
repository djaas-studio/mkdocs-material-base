[![CI/CD](https://github.com/djaas-swamp/mkdocs-material-base/actions/workflows/ci.yaml/badge.svg)](https://github.com/djaas-swamp/mkdocs-material-base/actions/workflows/ci.yaml)

# MkDocs Project Starter
This is a template project for creating new documentation projects that uses [MkDocs](https://www.mkdocs.org/) with the [Material Theme](https://squidfunk.github.io/mkdocs-material/).

## Requirements
* Python 3.11
* pre-commit hooks

## Local Setup
1. Clone this repository to your local machine.
```
git clone https://github.com/djaas-swamp/mkdocs-material-base.git
```
2. Inside the project root directory, create (and activate) a virtual environment to install your Python dependencies.
```
python3 -m venv venv
source venv/bin/activate
```
3. Using `pip`, install the Python dependencies from the `requirements.txt` file.
```
python -m pip install -r requirements.txt
```
4. Install pre-commit hooks to your project.
```
pre-commit install
```
5. Run the MkDocs built-in server. Navigate to http://127.0.0.1:8000 and you should see the project's home page.
```
mkdocs serve
```

## How to Install Packages
1. To install a new Python package, add your package name and version to the `requirements.in` file.
```
# requirements.in file
foo==1.0.1
```
2. Run `pip-compile` to generate the corresponding `requirements.txt` file. Make sure your Python virtual environment is activated.
```sh
source venv/bin/activate
pip-compile
```
3. Using `pip`, install the new Python package from the `requirements.txt` file.
```sh
python -m pip install -r requirements.txt
```
