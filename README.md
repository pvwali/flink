# flink

# create the flink services/containers config
- Create a docker-compose.yml file

# launch the cluster
- docker-compose up -d

# access the cluster 
http://localhost:8081/#/overview

# scale up/down the taskmgr
- docker-compose scale taskmanager=<N>
 
# access job manager containers
- docker exec -it $(docker ps --fliter name=jobmanager /bin/sh

# kill the cluster
- docker-compose down
