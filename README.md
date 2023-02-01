# ExemploRabbitMQ
Exemplo de producer e consumer utilizando RabbitMQ

## Para executar:
Criar e rodar um container RabbitMQ

docker run -d --name rabbitmq-exemplo -p 5672:5672 -p 5673:5673 -p 15672:15672 rabbitmq:3.8-management

![image](https://user-images.githubusercontent.com/57539940/215933361-e66aad10-8522-4c54-8121-b0a68b147707.png)

Restaurar os pacotes das aplicações

dotnet restore .\Producer\
dotnet restore .\Consumer\

Executar o produtor e o Consumidor

dotnet run .\Producer\
dotnet run .\Consumer\
