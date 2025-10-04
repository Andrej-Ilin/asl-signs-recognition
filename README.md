# [Google-Isolated_Sign_Language_Recognition](https://www.kaggle.com/competitions/asl-signs/overview)
## Approximate project architecture

asl-signs-recognition/

├── .pre-commit-config.yaml  # Конфиг для pre-commit хуков\
├── pyproject.toml           # Зависимости и конфиги (Ruff, black)\
├── uv.lock                  # Lock-файл для воспроизводимости\
├── data/\
│   ├── raw/                 # Исходные данные с Kaggle\
│   └── processed/           # Обработанные данные\
├── notebooks/               # Исследовательские ноутбуки\
│   ├── 01_eda.ipynb\
│   └── 02_model_prototyping.ipynb\
├── src/                     # Основной код проекта (пакет)
│   ├── __init__.py\
│   ├── data/\
│   │   ├── __init__.py\
│   │   ├── make_dataset.py  # Загрузка и предобработка\
│   │   └── preprocess.py    # Аугментации и т.д.\
│   ├── features/\
│   │   ├── __init__.py\
│   │   └── build_features.py # Инженерия признаков\
│   ├── models/\
│   │   ├── __init__.py\
│   │   ├── model.py         # Архитектура модели\
│   │   └── train_model.py   # Логика обучения\
│   └── visualization/\
│       ├── __init__.py\
│       └── visualize.py     # Функции для графиков\
└── tests/                   # Модульные тесты\
    ├── __init__.py\
    └── test_data.py\
