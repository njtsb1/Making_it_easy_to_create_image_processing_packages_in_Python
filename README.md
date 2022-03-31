# Project: Image Processing Package
## Project Author: Karina Kato
### Class: Coding Lab PRO - Digital Innovation One
[(clique aqui para ver o meu perfil na plataforma)](https://web.dio.me/users/njtsb1)
#### Tecnologia: Python
#### Data: 31/03/2022
-----------------------------------------
### Description
The "image_processing-test" package is used for:

- "Processing" module:
  - Histogram matching;
  - Structural similarity;
  - Resize image;

- Module "Utils":
  - Read image;
  - Save Image;
  - Plot image;
  - Graph result;
  - Plot histogram;
---------------------------------------------
## Configuration walkthrough to host a Python package in the Test Pypi test environment

- [x] Installation of the latest versions of "setuptools" and "wheel"

```
py -m pip install --user --upgrade setuptools wheel
```
- [x] Make sure the directory in the terminal is the same as the "setup.py" file

```
"C:\Users\NivaldoBeirão\source\image-processing-package> py setup.py sdist bdist_wheel
```

- [x] After completing the installation, verify that the folders below have been added to the project:
  - [x] build;
  - [x] dist;
  - [x] image_processing_test.egg-info.

- [x] Just upload the files, using Twine, to Test Pypi:

```
py -m twine upload --repository testpypi dist/*
```

- [x] After running the above command in the terminal, you will be asked to enter the username and password. Once this is done, the project will be hosted on Test Pypi. Host it on Pypi directly.

### Here the goal is not to use Karina's project to post on my personal Pypi profile, since the project is hers. I still don't have any projects that can be used as a package.

### However, keep in mind that Test Pypi, as its name implies, is just a test environment. In order for the project to be available as a package to be used publicly, it needs to be hosted on the official Pypi website.
-------------------------------------------------- --
## Local installation, after hosting on Test Pypi

- [x] Installation of dependencies
```
pip install -r requirements.txt
```

- [x] Package Installation

Use the package manager ```pip install -i https://test.pypi.org/simple/ image-processing-test ```to install image_processing-test

```bash
pip install image-processing-test
```
-------------------------------------------------
## How to use in any project

```python
from image-processing-test.processing import combination
combination.find_difference(image1, image2)
```
<img width="auto" src="https://github.com/njtsb1">

## Author (who hosted the project on Test Pypi)
Nivaldo Beirão

## License
[MIT](https://choosealicense.com/licenses/mit/)
