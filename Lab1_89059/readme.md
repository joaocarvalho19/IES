## Archetype

É um conjunto de ferramentas de modeling de um projeto Maven. Um archetype é definido como um padrão ou modelo original do qual todas as outras coisas do mesmo tipo são feitas.

## groupID e artifactId

O Maven usa um conjunto de identificadores groupID e artifactId:

    groupID: um nome de base exclusivo do grupo que criou o projeto.

    artifactId: um nome exclusivo do projeto.


## "Maven Goals"

Os Maven goals representam uma tarefa específica que contribui para a construção e gestão de um projeto.

--------------DOCKER----------------------

## List Docker CLI commands
docker
docker container --help

## Display Docker version and info
docker --version
docker version
docker info

## Execute Docker image
docker run hello-world

## List Docker images
docker image ls

## List Docker containers (running, all, all in quiet mode)
docker container ls
docker container ls --all
docker container ls -aq



## Resultado do comando: $ docker container ls -all:

	CONTAINER ID        IMAGE                    COMMAND             CREATED             STATUS                 PORTS        

    7952836483ff        portainer/portainer-ce   "/portainer"        6 days ago          Up Less than a second   0.0.0.0:8000->8000/tcp, 0.0.0.0:9000->9000/tcp   
    
    NAMES
    
    portainer


## Qual a relevância de configurar “volumes” quando se pretende preparar um container para servir uma base de dados?

O volume resolve questões de persistência de dados pois as informações armazenadas na camada do container são perdidas ao remover o container, ou seja, ao utilizar volumes temos maior garantia no armazenamento desses dados.