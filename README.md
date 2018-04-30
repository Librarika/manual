# Librarika

Librarika User Manual

## Contribute

This manual is created using MkDocs's Markdown files. You can easily contribute 
to enrich this documentation by forking this repository and updating the markdown 
files available under the `docs` folder.

Once you are done adding your documentation, please submit pull request.

## Inital Installation

This repository has beeen initialized with following commands. This is just for 
the documentation purpose.

```bash
virtualenv .
source bin/activate
curl https://bootstrap.pypa.io/get-pip.py | python
pip install mkdocs
pip freeze > requirements.txt
mkdocs serve
```

## Build

The final documentation is built automatically from each commit to the master branch of this git 
repository. Final documentation is available at https://librarika-manual.readthedocs.io.
