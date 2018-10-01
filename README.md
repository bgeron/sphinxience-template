# Example project that uses Sphinxience.

Use this project to easily get started with Sphinxience. Download and unpack https://github.com/bgeron/sphinxience-template/archive/master.zip, or fork and clone this repository [on GitHub](https://github.com/bgeron/sphinxience-template). 

Then:

1.  Install [Poetry](https://poetry.eustace.io/), a Python dependency manager. If you have Python3 installed, you can usually do this by typing:

        pip3 install --user poetry

2.  Fill in some project name in the `name` field in `pyproject.toml`. This name helps Poetry identify the dependencies that you have installed for this project.

        ...

        # pyproject.toml

        name = "my new Sphinxience project"

        ...

3.  Use Poetry to download and install the dependencies into a virtual environment:

        poetry install

    This may take a minute or so. On Linux, the dependencies will be installed somewhere in `~/.cache/pypoetry/virtualenvs/`, but this is not important.

4.  Consider cleaning up your folder by removing the file you're reading now:

        rm README.md

5.  Consider putting this folder in version control with Git:

        git init
        git add .
        git commit -m 'Initial commit'

6.  Build HTML and PDF
    
        make html
        make latexpdf

    You can now find the generated files in `_build/html/index.html` and `_build/latex/my-sphinxience-project.pdf`. (The file name of the latter file is determined by `latex_documents` in `conf.py`.)

Enjoy!