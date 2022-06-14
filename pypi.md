# Install twine
```sh
pip install twine
```
# Create folder dist
```sh
python setup.py sdist
```
# Publish package
```sh
twine upload dist/*
```