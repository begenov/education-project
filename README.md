# Руководство по проекту

Это репозиторий, содержащий три микросервиса, разработанных на языке Go и использующих следующие технологии: HTTP, Redis, Gin, Kafka, Swagger и Docker Compose. В этом README файле вы найдете информацию о запуске каждого из микросервисов, а также об их функциональности.

## Клонирование репозиториев

Для начала вам необходимо склонировать все репозитории. Вы можете воспользоваться следующими командами для каждого из репозиториев:

```
git clone https://github.com/begenov/admin-service.git
git clone https://github.com/begenov/student-service.git
git clone https://github.com/begenov/courses-service.git
```

## Микросервисы

Проект состоит из трех микросервисов: admin-service, student-service и courses-service. Ниже представлены инструкции по запуску каждого из них.

### admin-service

1. Перейдите в каталог admin-service после клонирования репозитория.

2. Запустите следующую команду для запуска контейнера Docker:

```
docker-compose up
```

3. После успешного запуска контейнера Docker, выполните следующую команду для запуска микросервиса:

```
go run cmd/main.go
```

### student-service

1. Перейдите в каталог student после клонирования репозитория.

2. Запустите следующую команду для запуска контейнера Docker:

```
docker-compose up
```

3. После успешного запуска контейнера Docker, выполните следующую команду для запуска микросервиса:

```
go run cmd/main.go
```

### courses-service

1. Перейдите в каталог course после клонирования репозитория.

2. Запустите следующую команду для запуска контейнера Docker:

```
docker-compose up
```

3. После успешного запуска контейнера Docker, выполните следующую команду для запуска микросервиса:

```
go run cmd/main.go
```

 ## Функциональность

 Проект предоставляет функциональность для работы с администраторами (admin), студентами (student) и курсами (course) с использованием HTTP запросов. Дополнительно, проект использует Apache Kafka для обработки сообщений и получения информации о курсах, на которые подписаны студенты, а также о студентах, зарегистрированных на определенный курс.

Для получения дополнительной информации о доступных HTTP
продалжи 
ChatGPT

запросах и эндпоинтах, вы можете обратиться к документации Swagger


## Swagger Documentation

Swagger предоставляет документацию для API проекта, описывая доступные эндпоинты, методы запросов и параметры. Чтобы получить доступ к Swagger документации, выполните следующие шаги:

### Admin Service

http://localhost:8080/swagger/index.html#/

### Student Service

http://localhost:8001/swagger/index.html

### Course Service

http://localhost:8000/swagger/index.html

Чтобы получить доступ к Swagger документации, вам необходимо сначала запустить каждый микросервис, следуя инструкциям, указанным в руководстве выше, а затем перейти по соответствующим ссылкам.

## Заключение

От моего имени я хотел бы сказать, что этот проект стал для меня ценным источником знаний и опыта. В ходе его разработки и использования технологий, таких как Golang, HTTP, Redis, Gin, Kafka, Swagger и Docker Compose, я смог изучить множество новых концепций и расширить свои навыки в области разработки микросервисов.

Этот проект не только помог мне лучше понять, как работает взаимодействие между различными компонентами, но и дал мне практический опыт в создании и развертывании масштабируемых приложений. Я также научился использовать Apache Kafka для обработки сообщений и узнал о важности документации API с помощью Swagger.