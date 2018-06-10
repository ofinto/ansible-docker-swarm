These roles create docker swarm cluster with load balancer (haproxy) on VM created vagrant. They deploy nginx, upgrade nginx and docker-ce.

1) git clone this repo :)
2) vagrant up
3) ansible-playbook create-swarm.yml -u ubuntu -i conf.d/hosts -s
4) ansible-playbook docker-service.yml -u ubuntu -i conf.d/hosts -s 
5) ansible-playbook upgrade-docker-ce.yml -u ubuntu -i conf.d/hosts -s