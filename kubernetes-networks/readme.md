# Hometask 

- Изменить readiness-пробу в манифесте deployment.yaml из
прошлого ДЗ на httpGet, вызывающую URL /index. html
- Необходимо создать манифест service.yaml, описывающий сервис
типа ClusterIP, который будет направлять трафик на поды,
управляемые вашим deployment
- Установить в кластер ingress-контроллер nginx
- Создать манифест ingress.yaml, в котором будет описан объект
типа ingress, направляющий все http запросы к хосту
homework.otus на ранее созданный сервис. В результате запрос
http://homework.otus/index.html должен отдавать код html
страницы, находящейся в подах

запустить curl -H "Host: homework.otus" http://homework.otus/index.html
добавить в /etc/hosts ingress ip
