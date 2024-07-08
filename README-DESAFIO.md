# Informações do desafio

Você foi contratado como engenheiro DevOps na empresa "FilmReviews Inc." e vai participar do desenvolvimento e entrega do principal produto da empresa, o "Review de Filmes".

Esse projeto é uma aplicação desenvolvida em C# e vocês estão em processo de prova de conceito, onde deve ser testado o deploy da aplicação em um ambiente Kubernetes.

## Documentação do Projeto

### kube-news

1º Contrução da imagem e tagamento de versão

~~~bash
docker build -t danncastro/kubenews:v1 . 
~~~

2º Envio da imagem para o repositorio do Docker

~~~bash
docker push danncastro/kubenews:v1
~~~~
