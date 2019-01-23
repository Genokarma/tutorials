# Galaxy Australia training

Tutorials on how to use Galaxy Australia.

This repo was forked from sepsis-omics in 2018 and is now being updated for Galaxy Australia.

## Deployment

The tutorials have been deployed here: https://galaxy-au-training.github.io/tutorials/

## How to work on them locally

### 1. Brew install python, or skip to step 2

Make sure /usr/local/bin is the first thing in your $PATH

Remove everything in /usr/local/: `rm -rf /usr/local/* `  

Go to https://brew.sh/ and copy the code for installing homebrew. Paste into your terminal. 

Remove any python paths in your bash_profile (or bashrc)

Restart a fresh terminal. 

Check if brew is working with `brew install hello`

Install: `brew install r perl python@2 python ruby git`

### 2. Install the mkdocs tools
```
% pip3 install mkdocs markdown-include mkdocs-alabaster mkdocs-bootstrap mkdocs-material pymdown-extensions
```

### 3. Clone the repo
```
% git clone [repo name] [name of folder]
% cd [name of folder]
```

Or, you could fork the repo to your own Github, and clone locally from there. 

### 4. Edit

A useful editor is Atom: https://atom.io

In Atom, open up the folder and edit in here. 

In the terminal, open a new tab and serve the page (i.e. display in a browser tab) by: `mkdocs serve`

Open your web browser to http://127.0.0.1:8000/ and leave it open.
This will update automatically as you make changes to the documenation.

On the web, the contents (displayed in the left hand column) are determined by the mkdocs.yaml file. 

Add or delete topics (and their location) in this file. 

We have not grouped any topics into categories yet but this may be required if the page gets too big. 

The docs are in docs/modules

These are organised by topic. The main file in each topic is usually the index.md file but this isn't a requirement. 

Each topic usually has an images file also. 

Not all topics are currently displayed (i.e. they are not listed in the yaml file), as some of them are too old (content was copied over from sepsis-omics tutorials). 

We are using Markdown for formatting. https://en.wikipedia.org/wiki/Markdown

### 5. When you are happy, add it the repo
```
git add docs/dna/denovo/minia.md
git commit -m "Added minia" mkdocs.yml docs/dna/denovo/minia.md
git push
```
Your private local web version  http://127.0.0.1:8000/ will also update.

### 6. To deploy the whole lot to the *public* website
```
mkdocs gh-deploy --clean --message "Added minia"
```
This first builds a web HTML version of our Markdown hierarchy into the `site/` folder, then pushes it to a special
branch of the github repo called `gh-pages` which GitHub makes available at the public URL
[https://galaxy-au-training.github.io/tutorials/]
