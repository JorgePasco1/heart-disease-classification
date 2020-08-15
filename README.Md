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

## Installation

This project uses conda as a environment/package manager. To easily run this project in your machine, you should have ananconda or miniconda installed (You might want to refer to [Conda documentation](https://docs.conda.io/en/latest/index.html)). Alternatively you can look at the environment.yml file and use your preferred method to install the required dependencies.

First, clone this repository to your machine:

```bash
git clone https://github.com/jorgepascoPE/heart-disease-classification.git
```

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
