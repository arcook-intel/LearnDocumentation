# Overview

This repo contains the project the `calculator` project that is a toy module used in the
Real Python tutorial
[Build Your Python Project Documentation With MkDocs](
    https://realpython.com/python-project-documentation-with-mkdocs/).
Its aim is to give you a framework to build your
project documentation using Python, MkDocs,
mkdocstrings, and the Material for MkDocs theme.

Also, the tutorial for setting up versioned docs using mike was followed: [setting up versioning](https://squidfunk.github.io/mkdocs-material/setup/setting-up-versioning/)

The documentation follows the best practice for
project documentation as described by Daniele Procida
in the [Diátaxis documentation framework](https://diataxis.fr/)

## How to publish a new form of the documentation

Create a virtual env
```shell
python3.7.4 -m venv venv
source venv/bin/activate.csh
pip install  -i https://intelpypi.intel.com/root/pypi -r requirements.txt
# NOTE: If you want to test locally remove the --push option
mike deploy --push <major>.<minor>

# To see all versions deployed
mike list
```
