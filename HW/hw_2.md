- Выберите для анализа один из двух временных рядов: [данные об осадках](https://disk.yandex.ru/d/mh1I7jRd0wRA4w) или [данные о продажах в онлайн-ритейлере](https://disk.yandex.ru/d/G2J7az05_TqlEw)
- Визуализируйте ряд и на основе его внешнего вида сделайте предположения о его компонентах (тренд, сезонность) и стационарности - **1 балл**
- Сделайте train/test split


### Бейзлайн

- Постройте бейзлайн в виде наивного прогноза или скользящего среднего - **2 балла**
- Визуализируйте результаты работы модели, произведите замеры качества бейзлайна с релевантной, на ваш взгляд, метрикой - **1 балл**

### Статистическая модель

- Проведите тест Дики-Фуллера и интерпретируйте результаты - **1 балл**
- Постройте графики ACF/PACF и проанализируйте их, сделайте предположения о наличии/отсутствии сезонности - **1 балл**
- Проведите необходимые на ваш взгляд преобразования для придания ряду стационарности (дифференцирование / сезонное дифференцирование) - **3 балла**
- Проверьте стационарность полученного ряда с тестом Дики-Фуллера и визуализацией ACF/PACF - **1 балл**
- Обучите модель ARIMA или SARIMA для прогнозирования значений ряда, подобрав оптимальные параметры - **5 баллов**
- Визуализируйте результаты работы модели, произведите замеры качества модели ARIMA (или SARIMA), сравните с бейзлайном - **1 балл**

### Классическая модель

- Используйте Feature-Engineering для создания признаков (лаги, скользящие статистики, признаки даты/времени, etc) - **5 баллов**
- На полученном наборе данных обучите случайный лес или градиентный бустинг - **2 балла**
- Визуализируйте результаты работы модели, произведите замеры качества модели, сравните с прошлыми экспериментами - **1 балл**

### Интерпретация

Проинтерпретируйте модель, полученную в шаге **Классическая модель** с помощью:
- permutation importance - **3 балла**
- LIME - **3 балла**
- SHAP - локальная интерпретация (для одного объекта) - **2 балла**
- SHAP - глобальная интерпретация (для всей модели целиком) - **2 балла**

Сделайте выводы о результатах интерпретации 


## Общее

- Обеспечена воспроизводимость решения: зафиксированы random_state, ноутбук воспроизводится от начала до конца без ошибок - **3 балла**
- Соблюден code style на уровне pep8 - **3 балла**
- Принимаемые решения обоснованы и прокомментированы в markdown ячейках (например, если считаете, что ряд стационарный, то написано, почему, и т.п.) - **10 баллов**
