
# Limpando o docker


Limpando todos os containers e imagens do sistema:

```
docker stop $(docker ps -aq) && docker system prune -af
```

Limpando apenas os containers do sistema:

```
docker stop $(docker ps -aq) && docker container prune -f
```

Limpando apenas as imagens do sistema:

```
docker rmi -f $(docker images -aq)
```

Parando o serviço padrão do mysql na porta 3306 (Caso haja necessidade):

```
service mysql stop
```

Ativando serviço do mysql:

```
service mysql start
```


