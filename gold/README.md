# Исследование технологического процесса очистки золота

### Цели проекта

- Подготовить модель машинного обучения для предскаазания коэффициента восстановления золота из золотосодержащей руды. Доступны данные с параметрами добычи и очистки. Модель необходима для оптимизации производства.  

### Задачи проекта

1. Подготовка Данных  
    1.1 Изучение данных  
    1.2 Проверка расчётов эффективности обогащения  
    1.3 Анализ признаков, недоступных в тестовой выборке  
    1.4 Предобработка данных  
2. Анализ данных  
    2.1 Анализ изменения концентрации металлов (Au, Ag, Pb)  
    2.2 Сравнение распределений размеров гранул сырья  
    2.3 Исследование суммарных концентраций веществ  
3. Построение модели  
    3.1 Подготовка метрики итоговой sMAPE  
    3.2 Обучение и оценка качества моделей
        -  DecisionTreeRegressor
        -  RandomForestRegressor
        -  LinearRegression
        -  Обучение и сравнение моделей. Вывод  
    3.3  Проверка лучшей модели на тестовой выборке

### Итоги
- Проанализированы концентрации металлов (Au, Ag, Pb), а также суммарные концентрации веществ на всех стадиях очистки.  
- Проверена гипотеза о равенстве размера гранул на тренировочной и тестовой выборках  
- Обучены модели  LinearRegression, DecisionTreeRegressor и RandomForestRegressor. Лучший результат показала модель RandomForestRegressor  
- sMAPE на тестовой выборке RandomForestRegressor:7.15.  
- Произведено сравнение с результами работы константной модели, показывающее адекватность работы модели RandomForestRegressor


   
### Используемый стек инструментов

- python
- pandas
- numpy
- sklearn
- scipy
- matplotlib
- seaborn
