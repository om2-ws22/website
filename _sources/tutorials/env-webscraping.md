# Environment webscraping


We install some modules in a new Anaconda environment. We call this new environment `webscraping`. 

> On *Windows* open the Start menu and open the "Anaconda Command Prompt". 

> On *macOS*: Open a terminal ([leran how to open a terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac)) 


- Copy this code and run it in your terminal: 

```bash
conda create -n webscraping python=3.9 requests pandas jupyter beautifulsoup4 altair matplotlib seaborn --y
```