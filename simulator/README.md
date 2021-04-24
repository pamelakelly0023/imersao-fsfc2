Imersão Full Stack & FullCycle - Codelivery
Descrição

Repositório do front-end feito com Golang (Backend)

Importante: A aplicação do Apache Kafka deve estar rodando primeiro.
Configurar /etc/hosts

A comunicação entre as aplicações se dá de forma direta através da rede da máquina. Para isto é necessário configurar um endereços que todos os containers Docker consigam acessar.

Acrescente no seu /etc/hosts (para Windows o caminho é C:\Windows\system32\drivers\etc\hosts):

127.0.0.1 host.docker.internal

Em todos os sistemas operacionais é necessário abrir o programa para editar o hosts como Administrator da máquina ou root.
Rodar a aplicação

Execute os comandos:

docker-compose up -d
# Entrar no container
docker-compose exec app bash
# Rodar a aplicação Golang
go run main.go
