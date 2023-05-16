## Определение цены автомобиля по имеющимся характеристикам

### Стек инструментов

Предобработка данных: обработка пропусков и дубликатов, изменение типа данных, группировка таблиц;  
Применение моделей градиентного бустинга: sklearn, LigtGBM, XGBoost, CatBoost;  
Валидация моделей.

### Вводные данные

Сервис по продаже поддержанных автомобилей разрабатывает мобильное приложение. Алгоритм определяет стоимость выставляемой на продажу машины.  
Модель должна выдавать максимально точную цену, быстро обучаться и иметь минимальное время предсказания.  

### Цель 

Создание модели, которая предсказывает цену автомобиля на основании определенных принаков.

Имеются размеченные данные: характеристики автомобилей и цена продажи.

### Структура проекта 

1. Загрузка и обработка данных: заполнение пропусков, группировка по признакам, поиск дубликатов, визуализация результатов;
2. Обучение моделей градиентного бустинга, анализ скорости обучения;
3. Валидация моделей и выбор лучшей для запуска в прод.  

### Общий вывод  

В исследовании приняли участие 4 модели : 'LightGBM', 'Catboost', 'Gradient_Boosting', 'xgboost'
Основной метрикой тестрирования стала метрика RMSE.

На первом этапе исследования был произведен анализ данных и заполнены пропущенные значения.

На втором этапе кейса было протестировано, в общей сложности, 5 моделей (4 описанных выше и дамми болванка, для сравнения адекватности работы моделей.)

Наилучшей и рекомендованной к использованию моделью признана LightGBM - со значением RMSE на тестовой выборке = 1767.1,  временем обучения = 2,5 минуты, временем предсказания 2,5 сек на учебном сервере.
