<img align="left" width="130" src="book/my24cell.jpg" alt="Advanced topics for high school math and science">

# [Advanced topics for math and science begginers](https://maojrs.github.io/topics_book/)

 A book introducing advanced topics for math and science beginners using Jupyter book.


## About
This is an interactive book on advance topics in mathematics and science at a level suitable for young students being initiated in the world of science. The book is aimed at the level of last year high school students and first years bachelor students with an interest in math and science. Each chapter consists of an interesting self-contained advanced topic that requires developing some mathematical/scientific concepts. The book illustrates and viualizes the concepts using code and interactive apps.

## Getting started
To get started just open the [book webpage](https://maojrs.github.io/topics_book/) and click on a chapter. 

The book is constructed as a collection of Jupyter notebooks, where each chapter corresponds to one notebook. The [Jupyter notebook](https://jupyter.org) is a free open-source web application that allows to create and share documents that contain live code, equations, visualizations and text. The notebooks are then gathered into one book using [Jupyter Book](https://jupyterbook.org). If you are interested in modifying the code or developing your own projects based on the book material, you have two options:

- Run the notebooks remotely on Binder: 
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/maojrs/topics_book/master?urlpath=tree/book/docs/index.ipynb)

- Run the Jupyter notebooks locally on your computer by following the instructions below.

## Run Jupyter notebooks locally
### Clone the repository
```
git clone https://github.com/maojrs/topics_book.git
cd topics_book
```

### Create a Conda environment
We recommend using the conda package manager to install all the dependencies required. The fastest way to start is to [install miniconda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) and then create a new environment. The requirements for the conda environment are provided in `environment.yml`, and the environment is created as follows:

1. `conda env create -f environment.yml`
2. `conda activate topics_book`

### Run Jupyter notebooks
To run the jupyter notebooks from your local copy of the book, do the following:
```
cd book/docs
jupyter notebook
```

## Building the Jupyter Book

You can also build the whole book from this repository. From the root folder, run the following command in your terminal:

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
