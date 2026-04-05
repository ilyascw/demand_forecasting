# project

Отдельный воспроизводимый репозиторий для экспериментов по прогнозированию спроса.

## Структура

- `data/raw/` — только сырые входные таблицы Kaggle.
- `artifacts/` — все воспроизводимые результаты прохода ноутбуков.
- `notebooks/` — основной исполняемый пайплайн.
- `.agents/REFACTOR.md` — план рефакторинга и методологические замечания.

## Порядок запуска

1. `notebooks/01_prepare_eda.ipynb`
2. `notebooks/02_mean_baseline.ipynb`
3. `notebooks/03_sarima_store_level.ipynb`
4. `notebooks/04_tabular_baselines.ipynb`
5. `notebooks/05_catboost.ipynb`
6. `notebooks/06_compare_models.ipynb`

## Принцип воспроизводимости

- ноутбуки читают только `data/raw/` или ранее созданные файлы из `artifacts/`;
- все промежуточные результаты сохраняются в явные каталоги внутри `artifacts/`;
- в репозитории не хранится содержимое производных артефактов, только их структура;
- итоговые таблицы из `artifacts/reports/` можно использовать в README и в тексте ВКР.
