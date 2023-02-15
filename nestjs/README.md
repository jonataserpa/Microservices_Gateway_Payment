[<img src="../img/nestjs.svg" width="72"/>](Nest.js)

# Imersão Full Stack & FullCycle 5.0 - Fincycle - Back-end das ordens de pagamento

## Descrição

Repositório do back-end das ordens de pagamento feito com Nest.js

**Importante**: A aplicação do Apache Kafka e Golang deve estar rodando primeiro.

## Rodar a aplicação

### Configurar /etc/hosts

A comunicação entre as aplicações se dá de forma direta através da rede da máquina.
Para isto é necessário configurar um endereços que todos os containers Docker consigam acessar.

Acrescente no seu /etc/hosts (para Windows o caminho é C:\Windows\system32\drivers\etc\hosts):
```
127.0.0.1 host.docker.internal
```
Em todos os sistemas operacionais é necessário abrir o programa para editar o *hosts* como Administrator da máquina ou root.

Execute os comandos:

```
docker-compose up
```

Acessar http://localhost:3000. Use os arquivos `accounts.api` e `orders.api` para testar a API.

Quer configurar um ambiente de desenvolvimento produtivo? Veja o vídeo: [https://www.youtube.com/watch?v=nTlM4sd-W3E](https://www.youtube.com/watch?v=nTlM4sd-W3E) 

### Para Windows 

Siga o guia rápido de instalação: [https://github.com/codeedu/wsl2-docker-quickstart](https://github.com/codeedu/wsl2-docker-quickstart) 
