# Data Reviews Online
# Deployment Instructions

## Deployment
### Centos 7
```console
yum -y update
yum -y install docker docker-compose
service docker start
```
 
### Ubuntu 16.04 (Xenial)
```console
apt-get update
apt-get install -y docker docker-compose
```

### Deploy Dareon
```console
git clone https://www.github.com/dareon-org/docker-dareon
cd docker-dareon/docker
docker-compose up -d --build
```

### Troubleshooting
#### docker commands
```console
docker-compose ps         # check processes
docker-compose logs web	  # check log of web process
docker-compose logs db	  # check log of db process
docker-compose down       # shutdown processes
docker-compose up -d      # start processes, without rebuild
```

#### check configuration file
```console
cat docker-compose.yml
```

### Test Users
| Username | Password |
| -------- | -------- |
| admin@dareon.org | admin |
| repoowner@rmit.edu.au | repoowner |
| dataowner@rmit.edu.au | dataowner |
