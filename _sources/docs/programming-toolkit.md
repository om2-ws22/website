# Programming toolkit

This section contains an overview about the programming toolkit you will need for our course. 

You will simply need to:

1. Install [Anaconda](anaconda) (includes Python and some toolkits)
2. Install [Visual Studio Code](vscode) (a code editor)
3. Create an acount at [GitHub](github) (for software development and version control)

Please read the following instructions about Anaconda and Visual Studio Code.

---


(anaconda)=
## Anaconda

The open-source [Anaconda Individual Edition](https://www.anaconda.com/products/individual) is one of the easiest ways to get started with data science projects. It already includes Python and the most important data science modules. 

:::{note}
Anaconda is a data science toolkit which already includes most of the data science modules we need.
:::


### Installation

You can skip the installation step if you already have Anaconda on your machine. If not, install the latest version of the Anaconda Individual Edition:

```{admonition} To do
:class: tip

- [Anaconda installation](https://www.anaconda.com/products/individual)

```

Follow the steps described in the next section.

### Anaconda environment

- On *Windows* open the Start menu and open the "Anaconda Command Prompt". 

- On *macOS*: [Open your terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac) 


Instead of the conda defaults channel, we want to use the community-led alternative `conda-forge` to install Python modules. 

Type this in your terminal to add `conda-forge`:

```bash
conda config --add channels conda-forge
```

Then make `conda-forge` the priority channel: 

```bash
conda config --set channel_priority strict
```


Now you can install the modules we need for our course in a new environment (we call this new environment `mr`). 

Copy this code and run it in your terminal (command prompt): 

```bash
conda create -n bigdata python=3.9 requests pandas jupyter tweepy networkx beautifulsoup4 altair vega_datasets matplotlib seaborn streamlit scikit-learn sqlalchemy psycopg2
```

When conda asks you: 

`Proceed ([y]/n)?` 

simply type `y` and press enter.

Now activate the new environment:

```bash
conda activate bigdata
```


### Troubleshooting

If you should have troubles with Anaconda, first make sure that you use the latest version (in our course, we use Python 3.9). In your terminal, type `python --version` to see which Python version you are using in your Anaconda base environment.

If you have an older version, I recommend to uninstall your current Anaconda environment from your machine and install the latest version: here a guide of how to [uninstall Anaconda](https://docs.anaconda.com/anaconda/install/uninstall/).


---

(vscode)=
## Visual Studio Code 


Visual Studio Code (also called Code) is a powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with a rich ecosystem of extensions for Python.

:::{note}
Visual Studio Code is a code editor that can be used with a variety of programming languages including Python.
:::

<br>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/KMxo3T_MTvY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br>

### Installation

Install VS Code:

```{admonition} To do
:class: tip
- [Install Code](https://code.visualstudio.com/)
```

### Install extensions

The features that Visual Studio Code includes out-of-the-box are just the start. VS Code extensions let you add languages, debuggers, and tools to your installation to support your development workflow.

Let's install some important extensions:

```{admonition} To do
:class: tip

- [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) 
```

### Jupyter Notebooks

We usually work with Jupyter Notebook files in VS Code:

```{admonition} To do
:class: tip
- [How to use Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)

```

### Optional tutorials

Here some resources to get familiar with VS Code:

- [Take a look at the intro videos](https://code.visualstudio.com/docs/getstarted/introvideos)

- [Data Science in VS Code tutorial](https://code.visualstudio.com/docs/datascience/data-science-tutorial)

- Pro tips: [25 VS Code Productivity Tips and Speed Hacks](https://www.youtube.com/watch?v=ifTF3ags0XI)


### Troubleshooting

If you have troubles to use Anaconda in Visual Studio Code, follow these instructions: 

- [Windows](https://stackoverflow.com/a/61937090/14796848)
- [Mac](https://stackoverflow.com/a/55203534/14796848)



---

(github)=
### Git and GitHub

[GitHub](https://github.com/) is a provider of internet hosting for software development and version control using Git. We will use GitHub as a platform for web hosting and collaboration.

:::{note}
Git is a version control system -- like the “Track Changes” features from Microsoft Word with many more additional features.
:::

- Git can be used to store content 
- Code can be changed and other developers can add code in parallel.
- Git has a remote repository which is stored in a server and a local repository which is stored in the computer of each developer.  

<br>

<iframe width="560" height="315" src="https://www.youtube.com/embed/w3jLJU7DT5E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  

<br>

You need a free GitHub-account for our course. Please follow the instructions below (*in case you already have a GitHub account: please add your HdM-email address to your account*):

```{admonition} To do
:class: tip

- [Create a GitHub account with your HdM-email](https://github.com/join)
- Verify your GitHub email
- You may also sign up fot the free [student developer pack](https://education.github.com/pack)  
- Install the [VS Code GitHub extension](https://code.visualstudio.com/docs/editor/github)
- [Install GitHub desktop to synchronize your machine with GitHub](https://desktop.github.com/)
```




---


## Fundamentals

### Python

Python is an object-oriented language (an object is an entity that contains data along with associated metadata and/or functionality).

One thing that distinguishes Python from many other programming languages is that it is interpreted rather than compiled. This means that it is executed line by line which is particular useful for data analysis, as well as the creation of interactive, executable documents like Jupyter Notebooks.

:::{Note}
Python is an interpreted language. The Python interpreter runs a program by executing one statement at a time.
:::

On top of this, there is a broad ecosystem of third-party tools and modules (like Jupyter Notebook) that offer more specialized data science functionality.

---

### Jupyter Notebook

[Jupyter Notebook](https://jupyter.org/) is an open-source application that allows you to create and share documents that contain code, equations, visualizations and narrative text. 

<br>

```{image} ../_static/img/jupyter.png
:alt: jupyter
:class: bg-primary mb-1
:width: 300px
:align: center
```

<br>

A notebook is basically a list of cells and the cells contain either

1. explanatory text (written in markdown)
1. executable code
1. code output

Note that we will use Jupyter Notebook inside the coding editor Visual Studio Code or Google Colab.

(colab)=
### Colab

Colaboratory, or “Colab” for short, is a free to use product from Google Research. Colab allows anybody to write and execute python code through the browser, and is especially well suited to perform data analysis and machine learning.

:::{note}
Colab is a free Jupyter notebook environment that requires no setup, and runs entirely on the Cloud.
:::

Watch this video to get a first impression of Colab:

<iframe width="560" height="315" src="https://www.youtube.com/embed/inN8seMm7UI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Let`s start your first Colab notebook to get an overview about some basic features:

```{admonition} Resources
:class: tip
- [Colab basic features overview](https://colab.research.google.com/notebooks/basic_features_overview.ipynb)
```

---

### Markdown

Markdown is one of the world’s most popular markup languages used in data science. Jupyter Notebooks use Markdown to provide an unified authoring framework for data science, combining code, its results, and commentary in Markdown. 

:::{note}
Markdown is a simple way to format text that looks great on any device.
:::

 Markdown files are designed to be used in three ways:

1. For communicating to decision makers, who want to focus on the conclusions, not the code behind the analysis.

2. For collaborating with other data scientists, who are interested in both your conclusions, and how you reached them (i.e. the code).

3. As an environment in which to do data science, as a modern day lab notebook where you can capture not only what you did, but also what you were thinking.

Review this site to learn more about Markdown:

```{admonition} Resources
:class: tip
- [Interactive Colab Markdown guide](https://colab.research.google.com/notebooks/markdown_guide.ipynb)

```

