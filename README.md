# ForecastPowerEnergy_Tat2023
Jupyter Notebook with algoritm forecasting Power Consumption in Tatarstan 2024 (XGBoost only)

Проблемы в этой версии:
1) Обнаружены данные на субботу (weekday == 5)
2) Из валидационной выборки выпадают 27 и 28 февраля (из-за отсутствия погодных данных)
3) Необходимо добавить указание месяца в сигнатуру функции `def diff_predict_vs_fact(df_validate_boost)`

В этой версии:
1) Устранены пропуски данных (последний 24-й час в месяце начиная с ноября 2023 года)
2) Выполнена валидация на февраль 2024 года
