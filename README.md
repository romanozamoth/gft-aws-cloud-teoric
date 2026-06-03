# Desafio DIO - AWS CloudFormation

## Descrição

Este repositório foi desenvolvido como parte do laboratório da DIO com foco em AWS CloudFormation.

O objetivo da prática foi compreender como utilizar Infraestrutura como Código (Infrastructure as Code - IaC) para provisionar recursos na AWS de forma automatizada, padronizada e reproduzível.

---

# Objetivos do Laboratório

* Compreender os conceitos de Infrastructure as Code.
* Criar uma Stack utilizando AWS CloudFormation.
* Utilizar Templates para definição de recursos.
* Automatizar o provisionamento de infraestrutura.
* Documentar os conhecimentos adquiridos durante a prática.

---

# O que é AWS CloudFormation?

AWS CloudFormation é um serviço que permite modelar e provisionar recursos da AWS através de arquivos de configuração chamados Templates.

Com ele é possível criar ambientes completos utilizando código, garantindo padronização, controle de versão e facilidade de manutenção.

---

# Conceitos Fundamentais

## Infrastructure as Code (IaC)

Abordagem que permite definir infraestrutura utilizando arquivos de código ao invés de configurações manuais.

Benefícios:

* Reprodutibilidade
* Automação
* Controle de versão
* Redução de erros humanos
* Facilidade de manutenção

---

## Template

Arquivo escrito em YAML ou JSON que descreve os recursos que serão criados.

Exemplos:

* Instâncias EC2
* Security Groups
* Buckets S3
* Bancos de Dados
* Redes VPC

---

## Stack

Uma Stack representa o conjunto de recursos criados a partir de um Template.

Ao criar uma Stack, o CloudFormation provisiona automaticamente todos os recursos definidos.

---

# Atividades Realizadas

## 1. Acesso ao AWS CloudFormation

Foi realizado o acesso ao serviço CloudFormation através do Console AWS.

---

## 2. Criação do Template

Foi desenvolvido um template contendo a definição dos recursos necessários para o laboratório.

---

## 3. Validação do Template

Utilização das ferramentas de validação do CloudFormation para garantir que a sintaxe estava correta.

---

## 4. Criação da Stack

Após a validação, foi realizada a criação da Stack.

Durante essa etapa foram observados:

* Eventos de criação
* Recursos provisionados
* Status da execução

---

## 5. Monitoramento

Acompanhamento dos eventos gerados durante o provisionamento dos recursos.

Principais estados observados:

* CREATE_IN_PROGRESS
* CREATE_COMPLETE
* UPDATE_IN_PROGRESS
* UPDATE_COMPLETE
* DELETE_COMPLETE

---

# Exemplo de Template

Exemplo simplificado de criação de uma instância EC2:

```yaml
AWSTemplateFormatVersion: '2010-09-09'

Resources:
  MinhaInstancia:
    Type: AWS::EC2::Instance
    Properties:
      InstanceType: t2.micro
      ImageId: ami-xxxxxxxx
```

---

# Benefícios Observados

* Criação rápida de ambientes
* Padronização da infraestrutura
* Facilidade para replicar ambientes
* Menor risco de erros manuais
* Melhor rastreabilidade das alterações

---

# Insights Pessoais

Durante o laboratório foi possível compreender como o CloudFormation simplifica o gerenciamento de infraestrutura em ambientes AWS.

A utilização de templates torna a criação de recursos mais segura e repetível, permitindo aplicar boas práticas de DevOps e automação.

Também ficou evidente a importância do conceito de Infrastructure as Code para projetos que necessitam de escalabilidade e padronização.

---

# Conclusão

O laboratório permitiu compreender os fundamentos do AWS CloudFormation e sua aplicação prática na criação automatizada de recursos em nuvem.

A experiência reforçou conceitos importantes de automação, versionamento de infraestrutura e boas práticas utilizadas em ambientes modernos de Cloud Computing.
