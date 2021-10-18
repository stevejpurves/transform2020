# Welcome to the Fatiando Transform 2020 tutorial

This is a simple small book to demonstrate the setup process, using the ipynb from Transform 2020

```{note}
This is a quick book build to demonstrate a the juptyerbook setup
```

```{code-block} bash
conda env create -f environment.yml
conda activate t20-thu-verde
```

## Steps to build this book

- checkout the repo
- create local conda environment
  ```{code-block} bash
  conda env create -f environment.yml
  conda activate t20-thu-verde
  ```
- install extras
  ```{code-block} bash
  pip install jupyter-book ipykernel
  ```
- create a jupyter kernel with the expected name
  ```{code-block} bash
  python -m ipykernel install --user --name conda-env-t20-thu-verde-py
  ```
- add book files
  - `_config.yml`
  - `_toc.yml`
  - `index.rst`
- add some more book files and update `_toc.yml`
- build the book
  ```{code-block} bash
  jupyter-book build .
  ```
