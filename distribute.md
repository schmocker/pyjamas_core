# Distribution
https://packaging.python.org/tutorials/packaging-projects/
## 1. Rename old version
Change ```version``` in ```setup.py```.

## 2. Remove old version
Remove the following folders:
- ```build```
- ```dist```
- ```pyjamas_core.egg-info```

## 3. Generating distribution archives
```
python3 setup.py sdist bdist_wheel
```
This command should output a lot of text and once completed should generate two files in the dist directory:
```
dist/
  pyjamas_core-0.0.1-py3-none-any.whl
  pyjamas_core-0.0.1.tar.gz
```
## 4. Uploading the distribution archives
```
twine upload dist/*
```
You will be prompted for the username and password you registered with yPI.