---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.12
    jupytext_version: 1.9.1
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

(introduction)=

# Introduction

This book is an interactive book on advance topics in mathematics and science at a level suitable for young students being initiated in the world of science. The book is aimed at the level of last year high school students and first years bachelor students with an interest in math and science. However, given the diversity of topics, it might be suitable for other levels and disciplines. Each chapter consists of an interesting self-contained advanced topic that requires developing some mathematical/scientific concepts. The book illustrates and viualizes the concepts using python computer code and interactive apps. When additional basic mathematical concepts are required for a given a topic, the text refers to specific sections of the **basic concepts** part of the book. 

The goal of this book is to introduce the topics in an accessible and fun way, with a computational and visual approach in mind. It is not intended to be a textbook nor to develop the concepts in all their rigor and detail. Another goal of the book is to serve as inspiration for class or personal projects. Each chapter constructs the fundamental theory and code implementations so the student can develop his or her own project. This could be from a simple extension of the topic presented to an and implementation of some of the suggested projects within each chapter.

The interactive book is constructed as a collection of Jupyter notebooks, where each chapter corresponds to one notebook. The [Jupyter notebook](https://jupyter.org) is a free open-source web application that allows to create and share documents that contain live code, equations, visualizations and text. The Jupyter notebooks are then unified into one interactive book using the [Jupyter Book project](https://jupyterbook.org). The book is intended to be read as the full unified interactive book. However, the individual chapters can be downloaded and ran locally to modify the code (see {ref}`Jupyter notebooks section <intro:jupyter>`).

To get started with the book, go directly to the {ref}`getting started <intro:getting_started>` section.

## Outline of chapters
Each chapter in the book introduces a topic, and it follows this basic outline:

1. **Introduction:** a brief introduction to the topic, which likely uses some audiovisual media to illustrate the relevance and interesting aspects of the topic. It might also include some historical context. 
2. **The topic presentation:** this is the main content of each chapter, where all the required concepts are presented through explanantions, visuals and interactive apps. This will likely contain several sections.  
3. **Concluding remarks:** this contains a brief summary of what was done in the notebook. It might also include additional historical context and the current relevance of the concepts introduced. The goal of this section is to show the student the broader context and impact of the topic discussed. 
4. **Suggested projects:** a list of suggested projects. Each suggested project contains a small description that serves as a guideline, and each one is given a difficulty level from one to five stars. The difficulty level is just a guideline, but it will differ greatly depending on the background of the student.
5. **References:** relevant references to the text and for the student to investigate the topic further.

(intro:getting_started)= 
## Getting started

To get started with the book is as simple as opening the [book webpage](./index.ipynb) and clicking on your chapter of choice. If you are interested modifying the notebooks in these book or developing your own projects using Jupyter notebooks, there are a couple of possibilities:

- Run a web-based version of the notebooks [on Binder](https://mybinder.org/v2/gh/maojrs/topics_book/master?urlpath=tree/book/docs/index.ipynb). This will run the notebooks remotely and requires being connected to the internet.
- Install Jupyter notebook following the instructions in the {ref}`Jupyter notebooks section <intro:jupyter>`. This will allow you to run the notebooks directly on your computer and offline. 

(Still need to add more specific instructions...)

[](intro:getting_started)

(intro:computer_code)= 
## Computer code
Throughout the book we use code snippets that produce output in the form of numerical values, plots or interactive plots. The programming language used in the book is python. To run the code interactively, we use Jupyter notebooks, a web-based interface for python (see [Section on jupyter notebooks](intro:jupyter)). Some notebooks will require additional python libraries: numpy and scipy for calculations; pandas and scikit learn for data manipulation; pyTorch for neural networks; matplotlib for static plots; and bokeh for interactive plots. If you run the interactive book online, this is not relevant to you. If you run the notebooks locally, all these libararies will be installed by following the instructions in the [Jupyter notebooks section](intro:jupyter).

The code snippets in the interactive book are self-contained. This means that if you copy the code snippet and run it in another notebook it should run without requiring any other piece of code (except for the imported libraries). These code snippets are meant to be simple to understand for beginners in computer programming. More advance code snippets, such as the code to generate interactive plots, is hidden to avoid cluttering the presentation of the topic at hand. Nonetheless, for the interested reader, these can be accessed by click the plus sign on the right hand side. 

To copy code to your own notebook, we recommend to first copy the required libraries for the give chapter. These are accesible on the top of every chapter by clicking the plus sign. Once they are copied, make sure you run them by pressing shift + enter. After these are copied, any other code snippet that you copy from that chapter should run smoothly.


(intro:jupyter)= 
## Jupyter notebooks
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

```{code-cell} ipython3

```
