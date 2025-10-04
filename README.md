# [Google-Isolated_Sign_Language_Recognition](https://www.kaggle.com/competitions/asl-signs/overview)
## Approximate project architecture

asl-signs-recognition/\
├── src/                          # Исходный код проекта\
│   ├── asl_signs/               # Основной пакет\
│   │   ├── __init__.py\
│   │   ├── data/\
│   │   │   ├── __init__.py\
│   │   │   └── load_dataset.py  # Загрузка данных из parquet\
│   │   ├── features/\
│   │   │   ├── __init__.py\
│   │   │   └── landmarks.py     # Обработка ключевых точек\
│   │   └── models/\
│   │           ├─ __init__.py\
│   │           └─ train.py         # Обучение модели\
├── notebooks/                    # Исследовательские ноутбуки\
│   ├── 01_eda.ipynb             # Анализ данных\
│   └── 02_baseline.ipynb        # Базовое решение\
├── tests/                       # Тесты\
│   └── __init__.py\
├── data/                        # Данные (в .gitignore)\
│   ├── raw/                     # Исходные данные Kaggle\
│   └── processed/               # Обработанные данные\
├── pyproject.toml\
├── .pre-commit-config.yaml\
└── README.md\
