# Zero-to-hero ML School 2022 Learnerpack

Repo to get Learners started with the material for the [Zero-to-hero ML School 2022](https://events.hifis.net/event/398).

# Software Required for the Course

The course uses Python 3 and some data analysis packages such as Numpy, Pandas,
scikit-learn, and matplotlib.


## (Recommended) Miniconda based installation

**This step is only necessary if you don't have conda installed already**:

- download the Miniconda installer for your operating system (Windows, MacOSX
  or Linux) [here](https://docs.conda.io/en/latest/miniconda.html)
- run the installer following the instructions
  [here](https://conda.io/projects/conda/en/latest/user-guide/install/index.html#regular-installation)
  depending on your operating system.
  
### Create conda environment

In this folder, do 
```sh
conda env create -f conda-environment.yml
```

To work in this conda environment, activate it:
```sh
conda activate scikit-learn-course
```


## (Optional Alternative) Bare-Python based

You are also free to follow the course in a bare python environment with built in python tools by using virtual environments and `pip`.

### Create virtual environment (as an alternative to conda)

In this folder, prepare a virual environment

```sh
python -m venv venv-sklearn-course --upgrade-deps
```

activate the environment we just created:

```sh
source venv-sklearn-course/bin/activate
```

install the required dependencies into this environment:
```sh
python -m pip install -r ./pip-requirements.txt
```

You can now work in this environment.

# Check your installation

To make sure you have all the necessary packages installed, we **strongly
recommend** you to execute the `check_env.py` script located at the root of
this repository:

```sh
python check_env.py
```

Make sure that there is no `FAIL` in the output when running the `check_env.py`
script, i.e. that its output looks similar to this:

```
Using python in /home/lesteve/miniconda3/envs/scikit-learn-course
3.9.1 | packaged by conda-forge | (default, Jan 10 2021, 02:55:42)
[GCC 9.3.0]

[ OK ] numpy version 1.19.5
[ OK ] scipy version 1.6.0
[ OK ] matplotlib version 3.3.3
[ OK ] sklearn version 1.1.1
[ OK ] pandas version 1.2.0
[ OK ] seaborn version 0.11.1
[ OK ] notebook version 6.2.0
[ OK ] plotly version 4.14.3
```

# Run Jupyter notebooks locally

Activate the environment you have created so far:
- using conda  
```sh
conda activate scikit-learn-course
```
- using `venv`  
```sh
source venv-sklearn-course/bin/activate
```

Once the environment has been activated, open a jupyter session:

```sh
jupyter notebook
```

All the Jupyter notebooks are located in the `notebooks` folder 
(and assume that the `datasets` folder is also available next to `notebooks`).


# LICENSE

If not stated otherwise, all material in this repo is licensed under CC-BY 4.0 and was taken from [this repository](https://github.com/INRIA/scikit-learn-mooc/tree/32cccc8b45d0ef23291fbcae505690151c7b2e97).


