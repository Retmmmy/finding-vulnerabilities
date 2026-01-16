**finding-vulnerabilities**

Проект по выявлению уязвимостей в C/C++ коде с использованием машинного обучения:
baseline‑модели (MLP/CNN/GRU/LSTM) и fine‑tuning трансформера **CodeBERT** на датасете BigVul

1. Подготовка данных
Используется датасет DynaOuchebara/BigVul
Разбиение на train/val/test, очистка кода и сокращение размера при необходимости

2. Baseline модели
Byte-level токенизация
Dataset/Dataloader
Модели: MLP, CNN, GRU, LSTM
Обучение и оценка с выводом метрик

3. CodeBERT
Токенизация кода с помощью AutoTokenizer
Fine-tuning с Trainer на train/val
Оценка на тестовом наборе
Сохранение результатов в CSV и JSON

4. Gradio интерфейс
Ввод кода в текстовое поле
Кнопки для примеров из тестового набора
