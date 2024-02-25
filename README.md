# Docker_Demo: iris-mail
The OEX package just uses a modest IRIS instance in Docker     
It is built using the small [Mini-Docker-Template](https://github.com/rcemper/mini-docker)    
### Prerequisites
Make sure you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Docker desktop](https://www.docker.com/products/docker-desktop) installed.
### Installation
Clone/git pull the repo into any local directory
```
$ git clone https://github.com/rcemper/DK_iris-mail.git
```
To build and start the container run:
```
$ docker compose up -d && docker compose logs -f
```
To open IRIS Terminal do:
```
$ docker-compose exec iris iris session iris
USER>
```
or using **WebTerminal**
```
http://localhost:42773/terminal/
```
To access IRIS System Management Portal
```
http://localhost:42773/csp/sys/UtilHome.csp
```
### How to use it
This presents OEX package [iris-mail](https://openexchange.intersystems.com/package/iris-mail) using the actual IPM module    
All user documentation is found there in the [original repo](https://github.com/oliverwilms/iris-mail/blob/main/README.md)  
Touch the production here [http://localhost:42773/csp/user/EnsPortal.ProductionConfig.zen?PRODUCTION=dc.iris.mail.Production](http://localhost:42773/csp/user/EnsPortal.ProductionConfig.zen?PRODUCTION=dc.iris.mail.Production)
