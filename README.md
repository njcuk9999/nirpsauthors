# Coauthors to tex

Quickly generate an author list from some linked googlespread sheets

- [Installation](#installation)
- [How to run](#how-to-run)
- [How to update the NIRPS author list](#how-to-update-the-nirps-author-list)



---

## Installation

### Step 1: Download the GitHub repository

```
git clone git@github.com:njcuk9999/coauthors2tex.git
```

if this doesn't work try instead:

```
git clone https://github.com/njcuk9999/coauthors2tex.git
```

### Step 2: Install python 3.X using conda

Using conda, create a new environment and activate it
Note you can also use a current conda environemnt or venv instead of conda

Below we use python 3.9

```
conda create --name coauthors-env python=3.9
```

```
conda activate coauthors-env
```

### Step 3: Install the coauthors2tex code

```
cd {COAUTHORS_ROOT}

pip install -U -e .
```

Note `{COAUTHORS_ROOT}` is the path to the cloned GitHub repository (i.e. `/path/to/coauthors2tex`)

---

## How to run

This is simple, in the command line just type:

```
conda activate coauthors-env
```

then you can run with the following command:

```
coauthors2tex
```

and follow the prompts on screen!

---

## How to update the NIRPS author list

- Open the googlespreadsheet [here](https://docs.google.com/spreadsheets/d/1hGPX_s_fUbEmjDtBbrWrlgwDFMC_Ek-63s1JCHnaIvA/edit?usp=sharing)
- Add to the list of papers in the "papers" sheet
- Add to the affiliations in the "affiliations" sheet
- Add to the authors in either the "nirps_authors" or "other_authors" sheet


Note if forking this project for a different spreadsheet one only needs to change the constants.py
(In future we may change this to a yaml file)

