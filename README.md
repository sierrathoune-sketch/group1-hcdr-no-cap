# no-cap

Group 1 final project for I526 applied machine learning: home credit default risk (HCDR). We predict whether a loan applicant will have trouble repaying, using the Kaggle HCDR dataset.

## repo layout

```
data/        raw kaggle csvs, local only (git ignores everything but .gitkeep)
notebooks/   phase notebooks (phase1.ipynb, phase2.ipynb, ...)
```

## setup

We all use the class docker container (`jimiucb1/i526-aml`)

Packages that are not in the container (for example lightgbm) go in `requirements.txt` once we add one. Anything installed by hand inside the container is lost when the container is recreated.

## getting the data

The data is never committed. Each person downloads it once:

1. Download the HCDR files from the [kaggle competition page](https://www.kaggle.com/c/home-credit-default-risk/data) (or use the copy from the course folder if you have it).
2. Put the csv files directly in `data/`, for example `data/application_train.csv`.

## working together

- Pull before you start working and push when you stop.
- Never use `git add .` blindly; check `git status` first so data and large files do not get committed.

## project schedule

Phase 0: team registration on Canvas and pick project (due Friday of week 11). Groups of four.

Phase 1: project proposal (due Tuesday of week 12). Project description, data, metrics, baseline models, baseline pipeline and other planned pipelines. Phase leader plan and credit assignment plan, both as tables.

Phase 2: EDA and baseline pipeline (due Tuesday of week 13). Grab data, EDA, metrics, baseline models, brief report. Feature engineering and hyperparameter tuning in pipeline form. Update via a 2-minute video, slides and notebook on a Canvas discussion.

Phase 3: feature engineering and hyperparameter tuning (due Tuesday of week 15). Another round of feature engineering and tuning, additional feature selection, ensemble methods. Update via video, slides and notebook.

Phase 4: final submission (due Tuesday of week 16). Advanced model architectures and loss functions, final report. Update via video, slides and notebook.
