# Домашнее задание к занятию 11.3 "ELK" - "Лабазов Александр"

---

### Задание 1. Elasticsearch. 

Установите и запустите elasticsearch, после чего поменяйте параметр cluster_name на случайный. 

	
```
curl -X GET 'localhost:9200/_cluster/health?pretty'
```
![Elasticsearch custom cluster_name](./images/elasticsearch-1.jpg)
---

### Задание 2. Kibana.

Установите и запустите kibana.
*Приведите скриншот интерфейса kibana на странице http://<ip вашего сервера>:5601/app/dev_tools#/console, где будет выполнен запрос GET /_cluster/health?pretty*
```
Правильный URL:
http://<ip вашего сервера>:5601/app/kibana#/dev_tools/console
```
![Kibana Console](./images/kibana-1.jpg)

---

### Задание 3. Logstash.

Установить и запустить Logstash и Nginx. С помощью Logstash отправить access-лог nginx в Elasticsearch. 
*Приведите скриншот интерфейса kibana, на котором видны логи nginx.*
![Kibana Logstash Nginx](./images/kibana-logstash-nginx.jpg)

---

### Задание 4. Filebeat. 

Установить и запустить Filebeat. Переключить поставку логов Nginx с Logstash на Filebeat. 
*Приведите скриншот интерфейса kibana, на котором видны логи nginx, которые были отправлены через Filebeat.*
![Kibana Filebeat Nginx](./images/kibana-filebeat-nginx.jpg)


