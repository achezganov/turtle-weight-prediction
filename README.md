
# Turtle Weight Prediction

## Overview
Данный проект реализует модель линейной регрессии для предсказания массы морских черепах на основе измерений, полученных с помощью системы компьютерного зрения. Цель — обеспечить точное и бесконтактное определение массы для снижения стресса животных и повышения эффективности реабилитации.

## Features
- Предобработка и очистка данных (включая исправление аномалий измерений)
- Исследовательский анализ данных (EDA)
- Обучение нескольких моделей линейной регрессии:
  - LinearRegression
  - Ridge
  - Lasso
  - SGDRegressor
- Оценка моделей по метрикам:
  - MAE (основная)
  - MSE
  - R²
  - MAPE
- Выбор лучшей модели на валидационной выборке
- Проверка на тестовой выборке
- Анализ важности признаков
- Функция предсказания массы

## Installation
```bash
git clone https://github.com/username/turtle-weight-prediction.git
cd turtle-weight-prediction
pip install -r requirements.txt
```

## Project Structure
```
turtle-weight-prediction/
│
├── data/
│   └── turtles.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── training.py
│   ├── evaluation.py
│   └── model.py
│
├── requirements.txt
└── README.md
```

## Configuration

Основные параметры:
- `test_size`: доля тестовой выборки (по умолчанию 0.2)
- `random_state`: фиксированное значение для воспроизводимости
- гиперпараметры моделей (регуляризация, learning rate и др.)
Настройка производится в коде обучения моделей.

**Возвращает:**
- Предсказанное значение массы (кг)

## License
MIT License
