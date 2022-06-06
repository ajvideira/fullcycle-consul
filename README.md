docker-compose up -d

docker exec -it consul01 sh

consul agent -dev

docker exec -it consul01 sh

consul members

mkdir /var/lib/consul
mkdir /etc/consul.d

ip address

consul agent -server -bootstrap-expect=3 -node=consulserver01 -bind=172.20.0.2 -data-dir=/var/lib/consul -config-dir=/etc/consul.d
