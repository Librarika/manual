# Librarika

Librarika User Manual

## Contribute

This manual is created using MkDocs's Markdown files. You can easily contribute 
to enrich this documentation by forking this repository and updating the markdown 
files available under `docs` folder.

Once you are done adding your documentation, please submit pull request.

## Inital Installation

This repository has beeen initialized with following commands. This is just for 
the documentation purpose.

```bash
virtualenv .
source bin/activate
curl https://bootstrap.pypa.io/get-pip.py | python
pip install sphinx sphinx-autobuild recommonmark mkdocs
sphinx-quickstart
make html
pip freeze > requirements.txt
```

## Build

This documentation is built automatically from the code commits to the git master 
repository. 
