# Machine Learning - Heart Disease Classification

In this project, we'll use a [heart disease dataset](https://www.kaggle.com/ronitf/heart-disease-uci) taken from Kaggle, to create a classification machine learning model that will predict the presence of a heart disease in a patient, given their condition of the following medical factors:

- age
- sex
- chest pain type (4 values)
- resting blood pressure
- serum cholestoral in mg/dl
- fasting blood sugar > 120 mg/dl
- resting electrocardiographic results (values 0,1,2)
- maximum heart rate achieved
- exercise induced angina
- oldpeak = ST depression induced by exercise relative to rest
- the slope of the peak exercise ST segment
- number of major vessels (0-3) colored by flourosopy
- thal: 3 = normal; 6 = fixed defect; 7 = reversable defect

Explore the [Jupyter notebook](https://github.com/JorgePasco1/heart-disease-classification/blob/master/heart-disease-classification.ipynb) with the finished project.

## Installation

This project uses conda as a environment/package manager. To easily run this project in your machine, you should have ananconda or miniconda installed (You might want to refer to [Conda documentation](https://docs.conda.io/en/latest/index.html)). Alternatively, you can use your preferred method to install the required dependencies (`jupyter`, `NumPy`, `Pandas`, `Matplotlib`, `scikit-learn`, `joblib` and `seaborn`); use the versions stated in the environment.yml file to reproduce the same environment used for this project..

First, clone this repository to your machine:

```bash
git clone https://github.com/JorgePasco1/heart-disease-classification.git
```
### Using conda

Then, create the environment folder with the dependencies within the project directory:

```bash
conda env create --prefix ./env -f ./environment.yml
```

Activate the environment, with:

```bash
conda activate ./env
```

And finally, if dependencies are correctly installed, you should be able to run:

```bash
jupyter notebook
```
### Troubleshooting

When creating the enviroment, you may encounter `ResolvePackageNotFound` problem:

```bash
ResolvePackageNotFound:
  - dependencies not found
```
To solve the problem, move the problematic dependecies under pip section in the .yml file, like:

```yml
dependencies:
  - appnope=0.1.0=py38_0
  - attrs=19.3.0=py_0
  - backcall=0.1.0=py38_0
  - blas=1.0=mkl
  - bleach=3.1.4=py_0
  - ca-certificates=2020.6.24=0
  - certifi=2020.6.20=py38_0
  - cycler=0.10.0=py38_0
  - dbus=1.13.14=h517e14e_0
  - decorator=4.4.2=py_0
  - defusedxml=0.6.0=py_0
  ** all dependencies, except those not found **
  - pip:
    - jedi=0.17.0=py38_0
    - jinja2=2.11.2=py_0
    - joblib=0.15.1=py_0
    - jpeg=9b=he5867d9_2
    - jsonschema=3.2.0=py38_0
    - jupyter=1.0.0=py38_7
    - jupyter_client=6.1.3=py_0
    - jupyter_console=6.1.0=py_0
    - jupyter_core=4.6.3=py38_0
    - kiwisolver=1.2.0=py38h04f5b5a_0
    - libcxx=10.0.0=1
    - libedit=3.1.20181209=hb402a30_0
    - libffi=3.3=h0a44026_1
    - libgfortran=3.0.1=h93005f0_2
    - libiconv=1.16=h1de35cc_0
    - libpng=1.6.37=ha441bb4_0
    *** All dependencies not found ***
```
