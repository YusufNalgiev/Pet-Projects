# Множественная классификация комментариев в Samokat.tech

## Задача
Предоставить модель классификации обратной связи от пользователей по множеству затронутых в тексте тематик. [Клик](https://github.com/YusufNalgiev/Pet-Projects/blob/main/Samokat_NLP/rubert%20(3).ipynb)

## Описание проекта
Команда машинного обучения пользовательского контента занимается внедрением ML-сервисов как для модерации контента, который публикуют пользователи, так и для генерации нового контента на карточках товара.
В основном работаем с текстовыми данными. Для решения поставленных задач используем различные методы, начиная от rule-based подходов, заканчивая обучением крупных языковых моделей (LLM).
Здесь предлагается решить задачу множественной классификации текстов для определения всех классов, к которым можно отнести каждый экземпляр.

В задании представлены ответы на опрос, состоящий из части с выбором ответа из списка и расширенного комментария с произвольным текстом. Необходимо для каждого ответа из 50 различных меток классов выбрать все затронутые.


## Навыки и инструменты
- Python
- Pandas
- Matplotlib
- PyTorch
- Transformers
- RuBERT
- Scikit-learn
## Вывод
Лучшей предобученной моделью для этой задачи оказалась RuBERT от DeepPavlov, количество батчей 16, количество эпох 10. Метрика Accuracy на валидационном датасете показала 0.70, F1 - 0.61.

Рекомендации заказчику:

увеличить выборку;
избавиться от дисбаланса классов;
возможно дополнительная информация помимо оценки и тегов.
