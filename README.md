# Drift meta learning

Master's thesis in Computer Science at the University of Brasília ([PPGI](http://ppgi.unb.br)).

The objective is to perform drift detection using meta learning by predicting the performance of a base model (regression or classification) with unknown target.

## 1. To Do
- [x] Offline stage MetaLearner implementation
- [x] Online stage MetaLearner implementation
- [x] Meta model incremental learning
- [x] Statistical meta features implementation
- [x] Clustering meta features implementation
- [x] PSI implementation
- [x] Domain classifier implementation
- [x] Meta/base model hyperparameter tuning
- [x] TimeSeries cross validation usage
- [x] Different base model metrics (meta labels) experiments
- [x] Target delay experiments
- [x] Different base model experiments
- [x] Meta base dimensionality reduction experiments
- [x] Other drift metrics implementation
- [x] Other databases experiments
- [x] Measure elapsed time
- [ ] Meta feature selection experiments
- [x] Baseline
- [x] Evaluation metrics for meta model vs baseline
- [ ] Drift alert definition
- [ ] Drift alert configuration
- [x] Code documentation
- [ ] Readme
- [x] Experiments notebooks adjustments to fit new MetaLearner structure

## 2. Running
To work on this project is important to read the git good practive guide first, [here](https://github.com/rubensmchaves/drift-meta-learning.feamelo/blob/main/git_good_practice.md). For the following steps we consider that you are using a Linux like shell. 

1. Clone this github project.
2. Set a local environment, using `venv` module. Check the W3School tutorial [here](https://www.w3schools.com/python/python_virtualenv.asp).
3. Install the required libraries.
4. Run the project locally.

### 2.1 Clone the project
It is important to note that, if you are using Windows this project has files with special character like ":" in its name. So, if you use the WSL (Windows Subsystem for Linux), otherwise you are going to have problem to checkout the project.

The checkout command:

```$ git clone [git_project_url]```

### 2.2 Local environment
Setting your local environment using the module `venv`. Execute only once, when you set your project for the first time. We suggest to name you local enviroment as `myenv`.

```$ python -m venv myenv```

Once it is done, verify the prefix `myenv` (your local environment name) at the command prompt, something like:

```(myenv) feamelo@my_computer:/$```

If it is not there, start your environment with the command:

```$ source myenv/bin/activate```

### 2.3 Required libraries
Installing the required libraries through the file `requeriments.txt`. At you project root type:

```$ pip install -r requirements.txt```

### 2.4 Executing 
