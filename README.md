# Docker Infrastructure

Simple development set up which allows to run all projects from the single entry point.

Folder structure must be the following:
```
|_identity-app
|_identity-faucet
|_ether-fuel-service
```

**Clone the repository in their respective folders**

To run project in dev mode:
```bash
$ cd docker_infrastructure
$ sudo docker-compose up --build
```

identity app listen on : 
```
localhost:8080 or {docker_public_ip}:8080
```

identity facuet Service listen on : 
```
localhost:4000 or {docker_public_ip}:4000
```

ether fuel Service listen on : 
```
localhost:5000 or {docker_public_ip}:5000
```

testrpc listen on : 
```
localhost:8545 or {docker_public_ip}:8545
```

to get the docker network bridge IP
```
docker inspect {container_name} | grep 'IPAddress'
```