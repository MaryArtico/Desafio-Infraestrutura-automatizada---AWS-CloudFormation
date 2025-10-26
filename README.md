# 🌀 Desafio Infraestrutura automatizada - AWS CloudFormation

## 📘 Iniciando o Desafio

Este projeto faz parte do Bootcamp do Samtander junto d DIO e tem como objetivo consolidar o meu conhecimento adiquirido em aula utilizando **AWS CloudFormation**

## 🎯 Objetivo

Construir uma infraestrutura automatizada  com AWS CloudFormation, aplicando os conceitos aprendidos e documentando a experiência.  

## ⚙️ Estrutura do Projeto

AWSTemplateFormatVersion: '2010-09-09'
Description: Template de exercicio para criar EC2 e S3

Resources:
  MeuBucketS3:
    Type: AWS::S3::Meu primeiro-bucket
    Properties:
      BucketName: meu-bucket-exercicio

  MinhaInstanciaEC2:
    Type: AWS::EC2::Instance
    Properties:
      InstanceType: t2.micro
      ImageId: ami-0c02fb55956c7d316 
      KeyName: minha-chave-ec2      

Já pelo Bash utilizei o comando:
aws cloudformation create-stack
Para criar a a Stack.

Feito esse processo, fiz a consulta do status pelo comando: aws cloudformation describe-stacks --stack-name minha-stack

E para fazer a exclusão: aws cloudformation delete-stack --stack-name minha-stack

## Experiência e resumo da CloudFormation

- Diferente do desafio anterior que foi criado um passo a passo da criação de uma Stack pelo console da AWS.
Nesse novo desafio conheci mais uma ferramente nova o VScode, e tive uma nova experiência para criar a Stack usando uma ferramenta local, sem precisar acessar o console.
- O processo por meio das ferramentas locais, me deram mais segurança para compilar as informações e fazedndo os comandos mais rápidos que do que se tivesse efetuado pelo o console. 

## Notas

Embora tenha encontrado dificuldades de iniciante para utilizar o VScode e até o Bash que já estou me habituando mais, gostei porque ter a possbilidade de fazer em outra ferramenta e identificando que a AWS registra e cria tudo. 