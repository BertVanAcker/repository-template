======================================
         PyPi build instructions
======================================


Howto distribute the  KB API (via PyPi)
--------------------------------------

in terminal -> cd C:pathh\to\package\PACKAGE

- py -m pip install build
- pip install pyparsing==3.0.5  !!pyparser downgrade needed!!
- py -m build --sdist
- twine check dist/*
- twine upload dist/*   -> username = see secrets PYPI_BUILD password = see secrets PYPI_BUILD

Auto-build + publisch in workflows
----------------------------------------

pypi-publish.yml will automatically build and publish pypi for this package



Installing the distribution
---------------------------
- pip install PACKAGENAME


See: https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#pure-python-wheel



