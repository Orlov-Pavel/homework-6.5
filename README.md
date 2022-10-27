# Домашнее задание к занятию "6.5. Elasticsearch"
1. Dockerfile можно найти [здесь](./dockerfiles/Dockerfile)  
   [Образ](https://hub.docker.com/repository/docker/pavelorlov1/netology-6.5) в dockerhub  
   Ответ ElasticSearch:  
   ![elastic](./pictures/elastic.PNG)
2. Список индексов:  
   ![indices](./pictures/indices.PNG)  
   Состояние кластера:  
   ![health](./pictures/health.PNG)  
   Некоторые шарды и кластер в состоянии yellow из-за того что не все шарды имеют достаточное кол-во реплик в связи с тем что кластер состоит только из одной ноды.
3. Запрос и результат:  
   ![snapshot](./pictures/snapshot.PNG)  
   Список индексов после создания индекса test:  
   ![indices 2](./pictures/indices%202.PNG)  
   Список файлов в директории со snapshot'ами:  
   ![snapshots](./pictures/snapshots.PNG)  
   Список индексов после удаления индекса test и создания индекса test2:  
   ![indices 3](./pictures/indices%203.PNG)  
   Запрос для восстановления и список индексов после восстановления:  
   ![indices 4](./pictures/indices%204.PNG)