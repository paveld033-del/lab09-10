# lab09-10

Лабораторные работы по ансамблевым методам машинного обучения.

| Ноутбук | Тема | Данные |
|---|---|---|
| `Ru_09_Bagging_Exercises.ipynb` | Бэггинг: Random Forest и Extra Trees, OOB-ошибка, метрики для несбалансированных классов, ROC и PR-кривые, важность признаков | `data/Orange_Telecom_Churn_Data.csv` |
| `Ru_10_Boosting_and_Stacking_Exercises.ipynb` | Бустинг и объединение моделей: Gradient Boosting, AdaBoost, подбор гиперпараметров `GridSearchCV`, логистическая регрессия, `VotingClassifier` | `data/Human_Activity_Recognition_Using_Smartphones_Data.csv` |

## Запуск

```bash
uv sync
uv run jupyter lab
```

Ноутбуки выполняются целиком из чистого ядра. Лаба 10 считается около 6-8 минут на 20 ядрах: в ней два поиска по сетке и `LogisticRegressionCV`. В лабе 10 используется Intel® Extension for Scikit-learn (`sklearnex`). JupyterLab устанавливается в то же окружение `.venv`, иначе ядро не найдёт DLL расширения.
