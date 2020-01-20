# Kafka
Nous avons suivi exactement le Tuto d'Open Classroom

Dans un premier, nous allons voir le format des données qu'on le récupère à l'aide de cette commande : 
Grace à cette commande, nous avons la possibilité de voir les différentes données collectées à chaque station différente. 

curl https://api.jcdecaux.com/vls/v1/stations?apiKey=c56f0238cb88278094194fc982df9ee29f68f6b2 | python -m json.tool

On peut avoir le nombre d'emplacements pour stationner son vélo ainsi que le nombre de vélo disponible ou encore les données de la position de la station. 

Pour pouvoir 

$ ./bin/zookeeper-server-start.sh ./config/zookeeper.properties
$ ./bin/kafka-server-start.sh ./config/server.properties
$ ./bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic velib-stations
