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
~~~

3º Execução aplicação banco de dados Postgress

~~~bash
kubectl apply -f imersao-devops-cloud-02/kube-news/k8s/database/deployment.yml
kubectl apply -f imersao-devops-cloud-02/kube-news/k8s/database/service.yml
~~~

![alt text](/kube-news/image_database.png)

4º Execução aplicação base

~~~bash
kubectl apply -f imersao-devops-cloud-02/kube-news/k8s/web/deployment.yml
kubectl apply -f imersao-devops-cloud-02/kube-news/k8s/web/service.yml
~~~

![alt text](/kube-news/image_servico.png)
![alt text](/kube-news/image_web.png)