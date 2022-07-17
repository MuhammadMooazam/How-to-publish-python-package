Following are some steps to publish python package on pypi.org

1) Make a folder on Desktop (eg: package)
2) Make folder within package folder with the name of your package (eg: saylani-ds)
3) Make files of license.txt , readme.txt and setup.py within package folder
4) Make file named __init__.py within package folder which is saylani-ds
5) Write your whole code of library in __init__.py file
6) In setup.py write the below code
from setuptools import setup
setup(name="saylani-ds",
version="0.1",
description="this is a package",
long_description="this is a very very long description",
author = "Sir Qasim and Syed Muhammad Mooazam",
packages = ["saylani-ds"],
install_packages = [])
7) In the package folder install the following using cmd
pip install wheel
python setup.py bdist_wheel
python setup.py sdist bdist_wheel
8) After this there will be two folders automatically created in the package folder.
9) After every change in the python file must run the following command
python setup.py sdist bdist_wheel
10) Setup an account on https://pypi.org/
11) For publishing the package on pypi run the following command
pip install twine
twine upload dist/*
Then enter username and password of pypi account
12) Package uploaded.
