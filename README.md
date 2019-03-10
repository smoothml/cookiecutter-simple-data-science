# Simple Data Science Cookiecutter
A template data science project structure. This is a simplified version of the excellent [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science). Produces a project structure like:
```
├ Makefile              <- Makefile with helpful make commands.
├ README.md             <- Top-level README for project developers.
├ .env                  <- Secrets. DO NOT SOURCE CONTROL!
├ data
│   ├ external          <- Data from external sources.
│   ├ interim           <- Intermediate, transformed data.
│   ├ processed         <- Final, canonical data sets from modelling.
│   ├ raw               <- Original, immutable raw data sets.
│   └ results           <- Results of modelling and analysis.
├ models                <- Trained and serialized models, model predictions, or model summaries.
├ notebooks             <- Jupyter notebooks. Naming convention is a of the form
│                          <step>.<version>-<initials>-<description>.ipynb
│                          For example 01.0-PH-really-interesting-analysis.ipynb.
├ outputs               <- Generated outputs, such as figures or reports.
├ requirements.txt      <- Python requirements file for reproducing the analysis environment.
├ setup.py              <- Allows pip installation of src as a package.
└ src                   <- Source code for use in the project.
    └ __init__.py
```

## Assumptions
This project template makes certain assumptions. These are:
* Your data science project uses Python.
* You're working in a *nix environment. Cookiecutter will give you project structure in Windows, but some feateures of this template may not work.
* You're using AWS for data storage. Support for other cloud providers will be added at a later date.

## Requirements
* Python >= 3.5 or Python 2.7.
* [Cookiecutter](https://cookiecutter.readthedocs.io) >= 1.6.0

## Usage
To start a new project, run:
```
cookiecutter https://github.com/smoothml/cookiecutter-simple-data-science
```
You will be asked to provide the variables described below.

| Variable | Description |
| -------- | ----------- |
| `project_name` | Name of your project. |
| `repo_name` | Name of your repository. Defaults to lower case `project_name` with spaces and underscores replaced with hyphens. |
| `author_name` | Your name, or name of your project or organization. |
| `description` | A short description of your project. |
| `s3_bucket` | Name of Amazon S3 bucket for storing your data and models. If you're not using S3 leave this as the default value and never speak of it again! |
| `aws_profile` | Name of AWS profile for accessing the S3 bucket. Again, if you're not using S3 ignore this. |
| `python_interpreter` | Deafults to Python 3. Unless you have a _very specific_ reason for using Python 2, use Python 3. |
| `license` | A choice of several open source licenses. Choose "None" if your project is not open source. |
