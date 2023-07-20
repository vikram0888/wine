create env 

```bash
conda create -n wineq1 python=3.7 -y
```

activate env
```bash
conda activate wineq1
```

created a req file

install the req
```bash
pip install -r requirements.txt
```
download the data from 

https://drive.google.com/drive/folders/18zqQiCJVgF7uzXgfbIJ-04zgz1ItNfF5?usp=sharing

```bash
git init
```
```bash
dvc init 
```
if dvc does not intiate then downgrade the fsspec
``` bash
pip install fsspec==2022.1.0
```
```bash
dvc add data_given/winequality.csv
```
```bash
git add .
```
```bash
git commit -m "first commit"
```

oneliner updates  for readme

```bash
git add . && git commit -m "update Readme.md"
```
```bash
git remote add origin https://github.com/vikram0888/wine.git
git branch -M main
git push -u origin main
```
used to track the inputs and outputs of data science experiments, version your data, and collaborate
```bash
dvc repro
```
compare the metrics of two different versions of a data set
``` bash
dvc metrics diff
```
show metrics
```bash
dvc metrics show
```
tox command -
```bash
tox
```
for rebuilding -
```bash
tox -r 
```
pytest command
```bash
pytest -v
```

setup commands -
```bash
pip install -e . 
```

build your own package commands- 
```bash
python setup.py sdist bdist_wheel
```
