# Docker Infrastructure

Simple development set up which allows to run all projects from the single entry point.

Folder structure must be the following:
```
|_identity-app
|_identity-faucet
|_ether-fuel-service
|_ipfs-network
|_shamir-service
|_testrpc-network
```

**Clone the repository in their respective folders**

To run project in dev mode:
```bash
$ cd docker_infrastructure
$ sudo docker-compose up --build
```

identity app listen on : 
```
localhost:8000 or {docker_public_ip}:8000
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

IPFS Web UI listen on : 
```
localhost:5001/webui or {docker_public_ip}:5001/webui
```

to get the docker network bridge IP
```
docker inspect {container_name} | grep 'IPAddress'
```
