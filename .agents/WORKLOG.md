# WORKLOG

## 2026-04-05

- Инициализирован отдельный каталог `project/` как самостоятельный git-репозиторий.
- Добавлены базовые служебные файлы: `README.md`, `.gitignore`, `.agents/WORKLOG.md`.
- Добавлен `.agents/REFACTOR.md` с полным планом рефакторинга пайплайна:
  от EDA до экспериментальных ноутбуков и final submission для нетяжелых моделей.
- Создана локальная рабочая структура `project/notebooks/` для рефакторинга без правок
  исходных ноутбуков в корне репозитория.
- Добавлены новые ноутбуки:
  `01_prepare_eda.ipynb`, `02_mean_baseline.ipynb`, `04_tabular_baselines.ipynb`,
  `06_compare_models.ipynb`.
- Перенесены и переименованы существующие ноутбуки:
  `03_sarima_store_level.ipynb`, `05_catboost.ipynb`,
  `archive_02_sarima_solution.ipynb`.
- В `05_catboost.ipynb` базовый набор численных признаков очищен от `sales_sum`;
  добавлено разделение между безопасными submission-признаками и optional research features.
