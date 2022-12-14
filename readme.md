# Проект "Отток клиентов"

Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.

Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Нам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.

Построим модель с предельно большим значением F1-меры. Нужно довести метрику до 0.59. Проверим F1-меру на тестовой выборке. Дополнительно будем измерять AUC-ROC, сравнивая её значение с F1-мерой.

## План работы

Загрузим и подготовим данные.
Исследуем баланс классов и обучим модель без учёта дисбаланса.
Улучшим качество модели, учитывая дисбаланс классов. Обучим разные модели (Логистическая регрессия, Дерево решений, Случайный лес) и найдем лучшую.
В конце проведем финальное тестирование.

## Вывод

Для финального теста выбрали модель "случайный лес". Обучили модель на общей большой выборке данных: тренировочные + валидационные. На тестовой выборке получили хорошие результаты метрик: f-score - 0.640 и roc-auc - 0.773.


------------------
Работа студента. Курс Специалист по Data Science плюс - Яндекс.Практикум.
Модуль - Обучение с учителем. Самостоятельный проект.