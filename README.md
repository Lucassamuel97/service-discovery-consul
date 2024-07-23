# Service Discovery e Consul

Este é um projeto de exemplo de funcionamento do `Service Discovery` utilizando a ferramenta `consul`.

- Oque é Service Discovery ?
    Service Discovery: Permite que serviços registrem sua localização e descubram outros serviços na rede. Quando um serviço é iniciado, ele pode se registrar no Consul, e outros serviços podem consultar o Consul para encontrar a localização do serviço registrado.

## Requisitos

- Docker
- Docker Compose

## Como iniciar o projeto

1. Clone o repositório:

```sh
git clone https://github.com/Lucassamuel97/service-discovery-consul.git
cd service-discovery-consul
```
2. Inicie o projeto:
```sh
    docker-compose up -d
```
Isso irá construir e iniciar o projeto utilizando Docker Compose.

3. Utilização: 

Você pode entrar nos containers executando o `docker exec it <nomeContainer> /bin/sh`, e como exemplo executar o `consul members` para visualizar a comunicação com os servidores.

```sh
docker exec -it consulclient02 /bin/sh
consul members
```
ou utilize a interface pelo navegador em 
`http://localhost:8500/ui/`

Consul Commands (CLI) 
<a href="https://developer.hashicorp.com/consul/commands" target="_blank">[Clique aqui para abrir mais comandos](https://developer.hashicorp.com/consul/commands)</a>

