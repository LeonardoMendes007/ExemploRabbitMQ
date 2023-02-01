# ExemploRabbitMQ
Exemplo de producer e consumer utilizando RabbitMQ

## Para executar:
Criar e rodar um container RabbitMQ

docker run -d --name rabbitmq-exemplo -p 5672:5672 -p 5673:5673 -p 15672:15672 rabbitmq:3.8-management

Restaurar os pacotes das aplicações

dotnet restore .\Producer\
dotnet restore .\Consumer\

Executar o produtor e o Consumidor

dotnet run .\Producer\
dotnet run .\Consumer\
