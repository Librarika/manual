# manual
Librarika User Manual


# Installation
```
virtualenv .
source bin/activate
curl https://bootstrap.pypa.io/get-pip.py | python
pip install sphinx sphinx-autobuild recommonmark
sphinx-quickstart
make html

pip freeze > requirements.txt

```