# moodle_lrs
Moodle + Xapi + LRS em container Docker

## Repositórios usados
https://github.com/michzimny/learninglocker2-docker

https://github.com/bitnami/bitnami-docker-moodle

## Instruções

1- configurar .env

2- build images ./build-dev.sh

3- configurar docker-compose e nginx.conf.template  

4- sudo docker-compose up --build, momento de paciência pois a instalação do moodle pode demorar

5- moodle default porta 80 e learning locker na 8080

6 -Criar usuario no learning locker:  docker-compose exec api node cli/dist/server createSiteAdmin [email] [organisation] [password] . O usuário padrao do moodle é user e senha bitnami.

7- instalar o plugin logstore xapi (site administration -> plugins -> install plugins)
https://moodle.org/plugins/logstore_xapi
