# [Google-Isolated_Sign_Language_Recognition](https://www.kaggle.com/competitions/asl-signs/overview)
## Approximate project architecture

asl-signs-recognition/\
├── .pre-commit-config.yaml\
├── pyproject.toml\
├── uv.lock\
├── config/\
│   └── default.yaml\
├── data/\
│   ├── raw/                    # Original Kaggle data\
│   └── processed/              # Processed features\
├── notebooks/\
│   ├── 01_eda.ipynb\
│   └── 02_baseline.ipynb\
├── src/\
│   ├── __init__.py\
│   ├── data/\
│   │   ├── __init__.py\
│   │   ├── make_dataset.py    # Data loading\
│   │   └── preprocess.py      # Landmark processing\
│   ├── features/\
│   │   ├── __init__.py\
│   │   └── build_features.py  # Feature engineering\
│   ├── models/\
│   │   ├── __init__.py\
│   │   ├── model.py           # Model architecture\
│   │   └── train_model.py     # Training logic\
│   └── visualization/\
│       ├── __init__.py\
│       └── visualize.py       # Plotting functions\
└── tests/\
    ├── __init__.py\
    └── test_data.py\
