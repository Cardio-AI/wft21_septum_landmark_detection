wft21_septum_landmark_detection
==============================

A short description of the project.

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like 'make environment' or 'make requirement'
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── metadata       <- Excel and csv files with additional metadata
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── predicted      <- Model predictions, will be used for the evaluations
    │   └── raw            <- The original, immutable data dump.
    │
    │
    ├── notebooks          <- Jupyter notebooks. 
    │   ├── Dataset        <- call the dataset helper functions, to analyze and slice the Dataset
    │   ├── Evaluate       <- See further below, reference to google-colab
    │   ├── Predict        <- Generate predictions for each fold
    │   ├── Train          <- Train a new model
    │
    ├── exp            <- Generated analysis as HTML, PDF, LaTeX, etc. Saved locally, if axes is needed , let us know
    │   ├── configs        <- Experiment config files as json
    │   ├── figures        <- Generated graphics and figures to be used in reporting
    │   ├── history        <- Tensorboard trainings history files
    │   ├── models         <- Trained and serialized models, model predictions, or model summaries
    │   ├── models.png     <- Model summary as picture
    │   └── tensorboard_logs  <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- Makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Helper functions that will be used by the notebooks.
        ├── data           <- create, preprocess and extract the nrrd files
        ├── models         <- Modelzoo, Modelutils and Tensorflow layers
        ├── utils          <- Metrics, callbacks, io-utils, notebook imports
        └── visualization  <- Plots for the data, generator or evaluations

Praktikum Data-Science in der Medizin
------------ 
We used Google-Colab for our Evaluation Script. In the `notebooks` folder you will find the main notebooks we used, in `src` you will find functions from the Code Base.
A huge thanks to Sven Köhler for his kind supervision, help and code. ✨ 🌟 💫
### Evaluation-Script for Interobserver Variability and Variability between Predictions and Ground-Truth
#### Link to Google Colab: https://colab.research.google.com/drive/1-wiDHzgGkPV13ZMaZLkvk5IYZSi6U5qm?usp=sharing
------------
### Link to Google Colab:


Setup native with OSX or Ubuntu
------------
### Preconditions: 
- Python 3.6 locally installed 
(e.g.:  <a target="_blank" href="https://www.anaconda.com/download/#macos">Anaconda</a>)
- Installed nvidia drivers, cuda and cudnn 
(e.g.:  <a target="_blank" href="https://www.tensorflow.org/install/gpu">Tensorflow</a>)

### Local setup
Clone repository
```
git clone %repo-name%
cd %repo-name%
```
Create a conda environment from environment.yaml (environment name will be foo)
```
conda env create --file environment.yaml
```

Activate environment
```
conda activate foo
```
Install a helper to automatically change the working directory to the project root directory
```
pip install --extra-index-url https://test.pypi.org/simple/ ProjectRoot
```
Create a jupyter kernel from the activated environment, this kernel will be visible in the jupyter lab
```
python -m ipykernel install --user --name foo --display-name "foo kernel"
```
