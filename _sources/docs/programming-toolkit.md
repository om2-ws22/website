# Programming toolkit

This section contains an overview about the programming toolkit you will need for our course. 

You will need to install:

1. the latest version of Anaconda (includes Python and some toolkits) 
2. Visual Studio Code (a code editor)
3. Git and create an acount at GitHub (for software development and version control)

Please read the following instructions.

---

(anaconda)=
## Anaconda

The open-source Anaconda Individual Edition is one of the easiest ways to get started with data science projects. It is a data science toolkit which already includes most of the data science modules we need.


### Uninstall your old version

To avoid compatibility problems with older versions of Anaconda, I recommend to uninstall Anaconda and install the latest version.

#### Windows


```{admonition} To do
:class: tip

1. Open the file explorer.
1. Delete your environment (anaconda3\envs) and package (anaconda3\pkgs) folders in your user folder.
1. Open Add or remove programs and uninstall your Anaconda installation.

```

#### macOS


> Open your terminal ([learn how to open your terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac))


````{admonition} To do
:class: tip

Remove your entire Anaconda directory with `rm -rf`. 

If you are not sure where anaconda is installed, simply enter all commands:

First try the opt folder:

```bash
rm -rf ~/opt/anaconda3
```

Then this location:

```bash
rm -rf anaconda3
```

Finally, enter:

```bash
rm -rf ~/anaconda3
```

````

### Install Anaconda

Install the latest version of the Anaconda Individual Edition:

```{admonition} To do
:class: tip

- [💾 Anaconda installation](https://www.anaconda.com/products/individual)

```


### Use conda-forge

Instead of the conda default package manager, we want to use the community-led alternative `conda-forge` to install Python modules.


> On *Windows* open the Start menu and open the "Anaconda Command Prompt". 


> On *macOS*: Open your terminal ([learn how to open your terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac))



````{admonition} To do
:class: tip

Type this in your terminal to add `conda-forge`:

```bash
conda config --add channels conda-forge
```

Then make `conda-forge` the priority channel: 

```bash
conda config --set channel_priority strict
```

````

---

(vscode)=
## Visual Studio Code 
 
Visual Studio Code is a code editor that can be used with a variety of programming languages including Python.


### VS Code installation

Install VS Code:

```{admonition} To do
:class: tip
- 💾 Install [VS Code](https://code.visualstudio.com/)
```

### Install extensions

VS Code extensions let you add tools to your installation to support your development workflow.


```{admonition} To do
:class: tip

- 💾 Install the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

- 💾 Install the [Live Share Extension Pack](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack)
```

Now close and restart VS Code.

### Jupyter Notebook extension

We usually work with Jupyter Notebook files in VS Code. 

```{admonition} To do
:class: tip

- 💾 Install the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

```

Now close and restart VS Code.

Open a Juptyer Notebook in VS Code:

```{admonition} To do
:class: tip
- Learn how to use [Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)
```

If you can't select a kernel (like the so called `base` kernel), try to close and restart VS Code once again.

---

(github)=
## Git and GitHub

Git is a version control system -- like the “Track Changes” features from Microsoft Word with many more additional features.

GitHub is a provider of internet hosting for software development and version control using Git. 



### Install Git


> On *Windows* open the Start menu and open the "Anaconda Command Prompt". 


> On *macOS*: Open your terminal.


````{admonition} To do
:class: tip

Type this in your terminal:

```bash
git --version
```

````

If you don't see the version, you need to install Git. *If you have **macOS**, the terminal may ask you if you want to install Git. Use this option to install Git right away*.  


```{admonition} To do
:class: tip


- 💾 Mac: 
  - Option 1: Install Git from your terminal after you have typed `git --version` in your terminal
  - Option 2: Install Apple's [XCode](https://apps.apple.com/us/app/xcode/id497799835?mt=12), which includes Git. 
  - Option 3: Install [Git with the help of homebrew](https://git-scm.com/download/mac).


- 💾 Windows: [Download Git](https://git-scm.com/download/win). You can follow [these instructions](https://www.heise.de/tipps-tricks/Git-auf-Windows-installieren-und-einrichten-5046134.html) to learn which options to choose during the installation process. When you are asked which editor you want to use, choose Visual Studio Code)


```


### GitHub account

You also need a free GitHub-account for our course. Please follow the instructions below (*in case you already have a GitHub account: please add your HdM-email address to your account*):

```{admonition} To do
:class: tip

- [Create a free GitHub account with your HdM-email](https://github.com/join)
- Verify your GitHub email
- 💾 Install [GitHub Desktop](https://desktop.github.com/) to synchronize your machine with GitHub
```


### VS Code GitHub extensions

Before you install the next extension, make sure you have the following prerequisites:

- An active GitHub account
- Git installed on your computer

```{admonition} To do
:class: tip

- 💾 Install the [VS Code GitHub extension](https://code.visualstudio.com/docs/editor/github)

- 💾 Install the [VS Code GitHub Classroom extension](https://marketplace.visualstudio.com/items?itemName=GitHub.classroom&ssr=false#overview)

```


---

