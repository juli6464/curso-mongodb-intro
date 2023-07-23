## Connect to container

``sh
docker-compose exec mongodb bash
``

``
winpty docker-compose exec mongodb bash
``

## Connect with mongosh

``sh

mongosh "mongodb://root:root123@localhost:27018/?tls=false&authMechanism=DEFAULT"

docker compose exec mongodb mongosh "mongodb://root:root123@localhost:27018/?tls=false&authMechanism=DEFAULT"

<!-- docker exec -it mongodb mongosh "mongodb://root:root123@localhost:27018/?tls=false&authMechanism=DEFAULT" -->

mongosh "mongodb://admin:eIpRHn44DALXKctV@ac-gqunrcr-shard-00-00.ohj3xzo.mongodb.net:27017,ac-gqunrcr-shard-00-01.ohj3xzo.mongodb.net:27017,ac-gqunrcr-shard-00-02.ohj3xzo.mongodb.net:27017/?replicaSet=atlas-8ohxen-shard-0&ssl=true&authSource=admin"

mongosh "mongodb+srv://admin:eIpRHn44DALXKctV@mongodb101.ohj3xzo.mongodb.net/"
``

``sh
show dbs
show collections
``

``sh
use("platzi_store")

db.products.find()
``
