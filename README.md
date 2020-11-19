# Jmetter-Cluster
docker swarm init --advertise-addr master_ip:2377
docker stack deploy -c docker-compose.yml test
docker exec -it <master_container>
jmeter -n -t test1.jmx -l test1.jtl -R b260d7cf0c91,58cc668ca1de
