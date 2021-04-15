# NLP-Toxicity-of-Comments
# NLP Токсичность комментариев
Задача: классифицировать комментарии на позитивные и негативные для целей модерации.

Для получения эмбеддингов используется 2 модели Bert и модель tf-idf.
Затем обучаются регрессионные модели, выбираются наилучшие. Искомая метрика f1.
Лучшие значения метрики для моделей bert дает логистическая регрессия, для моделей tf-idf - градиентный бустинг и случайный лес.
Составлен ансамбль из трех лучших моделей. Произведено тестирование.
Библиотеки torch, transformers, pymystem3, nltk, sklearn, lightgbm.