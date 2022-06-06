docker-compose up -d

docker exec -it consul01 sh

consul agent -dev

docker exec -it consul01 sh

consul members
