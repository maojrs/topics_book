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

This book is an interactive book on advance topics in mathematics and science at a level suitable for young students being initiated in the world of science. The book is aimed at the level of last year high school students and first years bachelor students interested in math and science. However each chapter is self-contained and develops different topics with a different focus, so it might as well be suitable for other levels and disciplines. Each chapter consists of an interesting self-contained advanced topic that requires developing some mathematical/scientific concepts. It also uses python computer code to illustrate and viualize the concepts (see [Section on computer code](intro:computer_code)). 

The goal of this book is to introduce the topics in an accessible and fun way, with a computational and visual approach in mind. It is not intended to be a textbook nor to develop the concepts in all their rigor and detail. Another goal of the book is to serve as inspiration for class or personal projects. Each chapter constructs the fundamental theory and code implementations so the student can develop his or her own project. This could be from a simple extension of the topic presented to an and implementation of some of the suggested projects.

The interactive book is constructed as a collection of Jupyter notebooks, where each chapter corresponds to one notebook. The [Jupyter notebook](https://jupyter.org) is a free open-source web application that allows to create and share documents that contain live code, equations, visualizations and text. The Jupyter notebooks are then unified into one interactive book using the [Jupyter Book project](https://jupyterbook.org). The book is intended to be read as the full unified interactive book. However, the individual chapters can be downloaded and ran locally to modify the code (see [Section on Jupyter notebooks](intro:jupyter)).

To get started with the book, go directly to the [Section on getting started](intro:getting_started).

## Outline of chapters
Each chapter in the book introduces a topic, and it follows this basic outline:

1. **Brief introduction:** a brief introduction to the topic, which likely uses some audiovisual media to illustrate the relevance and interesting aspects of the topic.
2. **The topic presentation:** this is the main content of each chapter, where all the required concepts are presented through explanantions, visuals and interactive. This will likely contain several sections.  
3. **Historical background and broader context:** a brief explanantion of the historical and current relevance of the concepts introduced is given, so the student can understand the broader context and impact of the topic discussed. 
4. **Suggested projects:** a list of suggested projects. Each suggested project contains a small description that serves as a guideline, and each one is given a difficulty level from one to five stars. The difficulty level is just a guideline, but it will differ greatly depending on the backgroun of the student.
5. **References:** relevant references to the text and for the student to investigate the topic further.

(intro:getting_started)= 
## Getting started

To get started with the book is as simple as opening the [webpage](./index.ipynb) of the book and clicking on your chapter of choice. If you are interested modifying the notebooks in these book or developing your own projects using Jupyter notebooks, there are a couple of possibilities:

- Run a web-based version of the notebooks using (binder)[https://mybinder.org/]. Simply follow the instructions in the [section on Binder](intro:binder). This will run the notebooks remotely and requires being connected to the internet.
- Install Jupyter notebook following the instructions in the [Jupyter notebooks section](intro:jupyter). This will allow you to run the notebooks directly on your computer and offline. 

(Still need to add more specific instructions...)

(intro:computer_code)= 
## Computer code
Throughout the book we use code snippets that produce output in the form of numerical values, plots or interactive plots. The programming language used in the book is python. To run the code interactively, we use Jupyter notebooks, a web-based interface for python (see [Section on jupyter notebooks](intro:jupyter)). Some notebooks will require additional python libraries: numpy and scipy for calculations; pandas and scikit learn for data manipulation; pyTorch for neural networks; matplotlib for static plots; and bokeh for interactive plots. If you run the interactive book online, this is not relevant to you. If you run the notebooks locally, all these libararies will be installed by following the instructions in the [Jupyter notebooks section](intro:jupyter).

The code snippets in the interactive book are self-contained. This means that if you copy the code snippet and run it in another notebook it should run without requiring any other piece of code (except for the imported libraries). These code snippets are meant to be simple to understand for beginners in computer programming. More advance code snippets, such as the code to generate interactive plots, is hidden to avoid cluttering the presentation of the topic at hand. Nonetheless, for the interested reader, these can be accessed by click the plus sign on the right hand side. 


(intro:jupyter)= 
## Jupyter notebooks
[Jupyter](http://jupyter.org/) notebooks are one of the many possible
ways to interact with the Python language and the scientific libraries.

They use a *browser-based* interface to Python with

-   The ability to write and execute Python commands.
-   Formatted output in the browser, including tables, figures,
    animation, etc.
-   The option to mix in formatted text and mathematical expressions.

Because of these features, Jupyter is now a major player in the
scientific computing ecosystem.

{numref}`Figure %s <jp_demo>` shows the execution of some code (borrowed from
[here](http://matplotlib.org/examples/pylab_examples/hexbin_demo.html))
in a Jupyter notebook

```{figure} /_static/lecture_specific/getting_started/jp_demo.png
:scale: 50%
:name: jp_demo

A Jupyter notebook viewed in the browser
```

Next we will show how to install Jupyter notebooks on your computer. The easiest way is to install a python distribution called anaconda, which already has everything you need.

### Installing Anaconda

To install Anaconda, [download](https://www.anaconda.com/download/) the
binary and follow the instructions.

Important points:

-   Install the latest version!
-   If you are asked during the installation process whether you\'d like
    to make Anaconda your default Python installation, say yes.

### Starting the Jupyter Notebook

Once you have installed Anaconda, you can start the Jupyter notebook.

Either

-   search for Jupyter in your applications menu, or
-   open up a terminal and type `jupyter notebook`
    - Windows users should substitute \"Anaconda command prompt\" for \"terminal\" in the previous line.

If you use the second option, you will see something like this

```{figure} /_static/lecture_specific/getting_started/starting_nb.png
:scale: 50%
```

The output tells us the notebook is running at `http://localhost:8888/`

-   `localhost` is the name of the local machine
-   `8888` refers to [port number](https://en.wikipedia.org/wiki/Port_%28computer_networking%29)
    8888 on your computer

Thus, the Jupyter kernel is listening for Python commands on port 8888 of our
local machine.

Hopefully, your default browser has also opened up with a web page that
looks something like this

```{figure} /_static/lecture_specific/getting_started/nb.png
:scale: 50%
```

What you see here is called the Jupyter *dashboard*.

If you look at the URL at the top, it should be `localhost:8888` or
similar, matching the message above.

Assuming all this has worked OK, you can now click on `New` at the top
right and select `Python 3` or similar.

Here\'s what shows up on our machine:

```{figure} /_static/lecture_specific/getting_started/nb2.png
:scale: 50%
```

The notebook displays an *active cell*, into which you can type Python
commands.

### Notebook Basics

Let\'s start with how to edit code and run simple programs.

#### Running Cells

Notice that, in the previous figure, the cell is surrounded by a green
border.

This means that the cell is in *edit mode*.

In this mode, whatever you type will appear in the cell with the
flashing cursor.

When you\'re ready to execute the code in a cell, hit `Shift-Enter`
instead of the usual `Enter`.

```{figure} /_static/lecture_specific/getting_started/nb3.png
:scale: 50%
```

(Note: There are also menu and button options for running code in a cell
that you can find by exploring)

#### Modal Editing

The next thing to understand about the Jupyter notebook is that it uses
a *modal* editing system.

This means that the effect of typing at the keyboard **depends on which
mode you are in**.

The two modes are

1.  Edit mode
    -   Indicated by a green border around one cell, plus a blinking cursor
    -   Whatever you type appears as is in that cell
2.  Command mode
    -   The green border is replaced by a grey (or grey and blue) border
    -   Keystrokes are interpreted as commands --- for example, typing `b` adds a new cell below the current one

To switch to
-   command mode from edit mode, hit the `Esc` key or `Ctrl-M`
-   edit mode from command mode, hit `Enter` or click in a cell

The modal behavior of the Jupyter notebook is very efficient when you
get used to it.

(intro:binder)= 
## Binder
 -- to be written ...


