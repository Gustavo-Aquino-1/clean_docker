
# Limpando o docker 🐋


Limpando todos os containers e imagens do sistema:

```
docker stop $(docker ps -aq) && docker system prune -af
```

``` "docker stop" requires at least 1 argument``` ➢ quer dizer que não há containers docker em sua maquina!

Limpando apenas os containers do sistema:

```
docker stop $(docker ps -aq) && docker container prune -f
```

``` "docker stop" requires at least 1 argument``` ➢ quer dizer que não há containers docker em sua maquina!

Limpando apenas as imagens do sistema:

```
docker rmi -f $(docker images -aq)
```

``` "docker rmi" requires at least 1 argument``` ➢ quer dizer que não há imagens docker em sua maquina!

Parando o serviço padrão do mysql na porta 3306 (Caso haja necessidade):

```
service mysql stop
```

Ativando serviço do mysql:

```
service mysql start
```


