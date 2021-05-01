# otus-microservices

## Создать минимальный сервис 
1. отвечает на порту 8000 + 
1. имеет http-метод GET /health RESPONSE: {"status": "OK"} + 
1. Cобрать локально образ приложения в докер. + 
1. Запушить образ в dockerhub + 
1. ссылку на github c манифестами. Манифесты должны лежать в одной директории, так чтобы можно было их все применить одной командой kubectl apply -f . + 
1. url, по которому можно будет получить ответ от сервиса (либо тест в postmanе). + http://arch.homework/health 
1. Задание со звездой* (+5 баллов): В Ingress-е должно быть правило, которое форвардит все запросы с /otusapp/{student name}/* на сервис с rewrite-ом пути. Где {student name} - это имя студента. + http://arch.homework/otusapp/samohin/health 