# MNB Image Analysis Course Repo

This repo hosts materials and a website for the Image Analysis course offered by the Microscopy Network Basel (MNB).

The course introduces the fundamentals of (bio-)image analysis and focuses on Python-based workflows for its practical sessions.

## Building the jupyter book locally

The website is built using [Jupyter Book](https://jupyterbook.org/).

To build the jupyter book locally (e.g. to preview your changes to it), make sure you have `jupyter-book` installed. You can install it via pip:

```bash
pip install "jupyter-book<2"
```

Then, navigate to the root of this repository and run:

```bash
jupyter-book clean .
jupyter-book build . --all
```

The built book will be available in the `_build/html` folder. You can open the `index.html` file in your web browser to view it locally.

## Notebook testing

The repo includes a GitHub Actions workflow to automatically verify that the Jupyter notebooks listed in `testing/notebooks_to_test.txt` run through in combination with the `materials/environment.yml` conda environment. This as well as the computer setup instructions can be replaced by pixi based workflows.