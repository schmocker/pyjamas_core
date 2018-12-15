# Distribution
https://packaging.python.org/tutorials/packaging-projects/
## Generating distribution archives¶
```
python3 setup.py sdist bdist_wheel
```
This command should output a lot of text and once completed should generate two files in the dist directory:
```
dist/
  pyjamas_core-0.0.1-py3-none-any.whl
  pyjamas_core-0.0.1.tar.gz
```
## Uploading the distribution archives
```
twine upload --repository-url https://test.pypi.org/legacy/ dist/
```
You will be prompted for the username and password you registered with yPI.