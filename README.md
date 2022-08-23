# Shapr3D Homework assignment

## Setting up the environment

In order to execute the contents of the notebook, you need to setup the environment first.

```bash
pip install pipenv
PIPENV_VENV_IN_PROJECT=1 pipenv install
```

The built-in SQLite database did not support window functions, therefore a recent version was compiled and installed based on the instructions from [here](https://charlesleifer.com/blog/compiling-sqlite-for-use-with-python-applications/).

After setting up the environment, place the uncompressed datasets to the `data` folder.


## Repo structure
```
.
├── Pipfile           - Dependency management file
├── Pipfile.lock      - Lock of the dependency versions
├── README.md         - Main readme
├── data              - Folder for the input data
├── notebooks         - Notebook to reproduce results
├── reports           - Exported reports in html. Including the notebook results.
└── sqlite            - Source for the freshly compiled SQLite database 
```


## Dev notes

Use the following command to export notebook wihtout any code.
```bash
jupyter nbconvert ./notebooks/homework.ipynb --no-input --to html
```