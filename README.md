# Shapr3D Homework assignment

## Setting up the environment

In order to execute the contents of the notebook, you need to setup the environment first.

```bash
pip install pipenv
PIPENV_VENV_IN_PROJECT=1 pipenv install
```

The built-in SQLite database did not support window functions, therefore a recent version was compiled and installed based on the instructions from [here](https://charlesleifer.com/blog/compiling-sqlite-for-use-with-python-applications/).

After setting up the environment, place the uncompressed datasets to the `data` folder.
