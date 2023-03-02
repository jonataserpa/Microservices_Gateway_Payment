# Microserviços de Gateway de pagamento


## Ordem recomendada de execução

* Apache Kafka
* Golang
* Back-end Nest.js
* Front-end Next.js

## Diagrama C4 da solução
![Diagrama C4](img/c4.png)


## Conectar no kafka producer
kafka-console-producer --bootstrap-server=localhost:9092 --topic=transactions

## Conectar no kafka consumer
kafka-console-consumer --bootstrap-server=localhost:9092 --topic=transactions_result

## Exemplo de mensagem kafka para rejeição

{"id":"12345","account_id":"1","credit_card_number":"1111111111111","credit_card_name":"Exemplo jhow","credit_card_expiration_month":12,"credit_card_expiration_year":2024,"credit_card_expiration_cvv":122,"amount":1200}

## Exemplo de mensagem kafka para aprovação 
{"id":"12345","account_id":"1","credit_card_number":"5307499680703280","credit_card_name":"Exemplo jhow","credit_card_expiration_month":12,"credit_card_expiration_year":2024,"credit_card_expiration_cvv":122,"amount":900}
