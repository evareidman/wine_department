# РосВинТорг
Команда чемпионов: Рейдман Е.Р., Максимова С.А., Чернякова Д.М.


## Описание проекта
- Объект исследования: рынок вин 
- Цель исследования: найти возможные закономерности в данной нише
- Основа данных: [каталог SimpleWine](https://simplewine.ru/catalog/vino)


## Задачи проекта:
1. Спарсить данные для проекта из ([каталога SimpleWine](https://simplewine.ru/catalog/vino))
2. Предообработать данные:
* Заменить/удалить пропуски
* Изменить тип данных (например, перевести год из float в int)
* Удалить выбросы
3. Создать новые признаки
* Бинарная колонка с информацией о наличие отзывов у каждого товара
* Ценовая категория вин
* Соотношение цены и рейтинга
4. Исследовать данные, рассмотреть и визуализировать потенциальные зависимости между признаками:
* Количественных переменных друг от друга
* Цены от рейтинга
* Цены от года
* Цены от страны-производителя
* Рейтинга от страны-производителя
* Между количеством отзывов и рейтингом
* Тыка от пыка
5. Проверить гипотезы с помощью математической статистики на уровне значимости 5%:
* Средний рейтинг дорогих вин в среднем такой же, как и у дешевых и средних, против того, что у дорогих средний рейтинг выше
* Средняя цена старых вин такая же, как и у новых против того, что старые вина в среднем дороже (за старые возьмем вина старше 2010 года)
* Средняя стоимость восточноевропейских вин такая же, как у западноевропейских, против того, что западноевропейские вина дороже
* Средний рейтинг вин старого света такой же, как у вин нового света
* Доля Франции на российском рынке такая же, как у остальных стран в сумме
6. Применить машинное для:
* Создания модели, предсказывающей ценовую категорию на основе логистической регрессии и случайного леса (задача множественной классификации)
* Оценки качества модели через метрики Accuracy, Recall, Precision, F1, ROC AUC и Log Loss
