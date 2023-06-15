
# О проекте

Проект представляет собой API для возможности взаимодействия с Nosql базой данных mongodb.

### Технологии

* MongoDB
* FastAPI
* pydantic (для построения моделей данных)
* [motor_asyncio (коннектор к базе данных)](https://motor.readthedocs.io/en/stable/tutorial-asyncio.html)
* Docker

### Описание проекта

[Программа, имитирующую работу реестра домашних животных.](src) В программе должен быть реализован следующий функционал:

* Завести новое животное
* Определять животное в правильный класс
* Увидеть список команд, которое выполняет животное
* Обучить животное новым командам
* [Счетчик который](src/utils/counter.py) показывает сколько животных было создано

![](./images/img.png)

### Запуск проекта

Выполнить команду

В корне проекта создать файл .env

```dotenv
MONGO_USER=root
MONGO_PASS=password
MONGO_DB=rootDB
MONGODB_URL=mongodb://root:rootDB@mongodb/?retryWrites=true&w=majority
```

Запустить проект в докере

```docker
docker-compose up -d --build
```