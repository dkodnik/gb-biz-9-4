# python-flask-docker
Итоговый проект курса "Машинное обучение в бизнесе"

Стек:

ML: sklearn, pandas, numpy
API: flask
Данные: https://drive.google.com/file/d/1Si4EJ_RexI3Q7yZU8eLjgp4ORe_BXr4G/edit

Задача: Определение вероятности наличия сердечно-сосудистых заболеваний по данным первичного осмотра. Бинарная классификация

Модель: DecisionTreeClassifier

### Клонируем репозиторий и создаем образ
```
$ git clone https://github.com/dkodnik/gb-biz-9-4.git
$ cd gb-biz-9-4
$ docker build -t gb-biz-9-4 .
```

### Запускаем контейнер

Здесь Вам нужно создать каталог локально и сохранить туда предобученную модель (<your_local_path_to_pretrained_models> нужно заменить на полный путь к этому каталогу)
```
$ docker run -d -p 8180:8180 -p 8181:8181 gb-biz-9-4
```

### Переходим на localhost:8181
