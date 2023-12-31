# Hello, concrexit!

Welcome to the mini-version of [concrexit](http://github.com/svthalia/concrexit). 
This is a small Django project that is used as a tutorial for new developers to get familiar with the actual [concrexit codebase](http://github.com/svthalia/concrexit).

This project contains a virtually empty website for Thalia. It is a starting point for 
new developers, to try adding a feature quickly, without the distraction and intimidation 
of a large codebase.

There is an example issue that you can try to implement in this project. It is a realistic
issue that could even one day be implemented in the real concrexit. You can find the issue
here: [#1](https://github.com/svthalia/hello-concrexit-tutorial/issues/1).


## Usage

The Technicie can help explain better, but here are some things you can do to get this
project running on your own computer. First ensure you have Python and 
[Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer) installed.
Then:

```
# If you haven't cloned this yet:
git clone git@github.com:svthalia/hello-concrexit-tutorial.git

# To install the dependencies:
poetry install

# Open a shell where the dependencies are installed:
poetry shell

# To create or update the database:
python website/manage.py migrate

# To create a (super)user:
python website/manage.py createsuperuser

# To run the server:
python website/manage.py runserver
```


## What I did to set up this project

> You do not have to do this yourself, this is just for reference.

```bash
mkdir hello-concrexit-tutorial
cd hello-concrexit-tutorial
git init

poetry init
poetry add Django
poetry add django-bootstrap5
poetry add --group dev black
poetry install

poetry shell

mkdir website
cd website
django-admin startproject miniconcrexit .
```
