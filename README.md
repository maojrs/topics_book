<img align="left" width="120" src="book/my24cell.jpg" alt="Advanced topics for high school math and science">

# Advanced topics for high school math and science

A book on advanced topics for high school and first year bachelor math and science using Jupyter Book.

This book is an interactive book on advance topics in mathematics and science at a level suitable for young students being initiated in the world of science. The book is aimed at the level of last year high school students and first years bachelor students with an interest in math and science. Each chapter consists of an interesting self-contained advanced topic that requires developing some mathematical/scientific concepts. The book illustrates and viualizes the concepts using code and interactive apps.

## Getting started
To get started with the book is as simple as opening the [book webpage](./index.ipynb) and clicking on your chapter of choice. 

The interactive book is constructed as a collection of Jupyter notebooks, where each chapter corresponds to one notebook. The [Jupyter notebook](https://jupyter.org) is a free open-source web application that allows to create and share documents that contain live code, equations, visualizations and text. The Jupyter notebooks are then unified into one interactive book using the [Jupyter Book project](https://jupyterbook.org). If you are interested in modifying the code in these book or developing your own projects using Jupyter notebooks, you can clone this repository and run the Jupyter notebooks directly on your computer.

## Run Jupyter notebook locally
### Clone the repository
```
git clone https://github.com/maojrs/topics_book.git
cd topics_book
```

### Creating a Conda environment
We recommend using the conda package manager to install all the dependencies required. The fastest way to start is to [install miniconda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) and then create a new environment. The requirements for the conda environment are provided in `environment.yml`, and the environment is created as follows:

1. `conda env create -f environment.yml`
2. `conda activate topics_book`

### Running the Jupyter notebooks
To run the jupyter notebooks from your local copy of the book, do the following:
```
cd book/docs
jupyter notebook
```

## Building the Jupyter Book

From the root folder, run the following command in your terminal:

```bash
jb build book/
```

If you would like to work with a clean build, you can empty the build folder by running:

```bash
jb clean book/
```

If jupyter execution is cached, this command will not delete the cached folder. 

To remove the build folder (including `cached` executables), you can run:

```bash
jb clean --all book/
```

## Publishing this Jupyter Book

This repository is published automatically to `gh-pages` upon `push` to the `master` branch.
