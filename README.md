# ACI-postman
Repositorio criado para compartilhar endpoints utilizados para configuração em massa no Cisco ACI

# Automação de Configurações em Massa no Cisco ACI com Postman 

Este repositório contém um guia prático e arquivos de exemplo para aplicar configurações em massa no Cisco ACI utilizando o Postman. O objetivo é facilitar a automação e a execução em lote de configurações em ambientes ACI, otimizando o tempo e reduzindo a possibilidade de erros manuais.

## Visão Geral

O **Cisco ACI** é uma solução poderosa para gerenciar redes de data centers, mas a aplicação de múltiplas configurações pode ser trabalhosa sem uma automação adequada. Utilizando o **Postman** em conjunto com o função **Runner**, é possível enviar requisições em lote, aplicando configurações massivas de forma eficiente.

Este repositório cobre os seguintes tópicos:

- Criação Tenants
- Criação Bridge Domain
- Criação Bridge Domain com Subnet
- Vincular Physical Domain a EPG
- Criação Application Profile
- Criação EPG
- Static Bind EPG interface VPC
- Static Bind EPG interface individual

## Pré-requisitos

Antes de começar, certifique-se de que os seguintes pré-requisitos foram atendidos:

- **Cisco ACI** configurado e acessível via API.
- **Postman** instalado (versão 9.x ou superior).
- Acesso às credenciais de autenticação da API do Cisco ACI (usuário e senha, ou token de acesso).
- Conhecimento básico de JSON e APIs REST.

## Instalação

1. Clone este repositório para o seu ambiente local:

   ```bash
   git clone https://github.com/AllysonGaldino1997/ACI-postman.git
   cd aci-postman-runner

   Importe as Collections do Postman contidas na pasta collections:

Abra o Postman.
Clique em "Import" e selecione o arquivo .json (Cisco ACI - LAB.postman_collection) da collection.
Crie suas variaveis de ambiente username, password & hostname.

## Uso do Postman Runner
Com as collections e environment configurados no Postman, acesse a função Runner:

No menu inferior direito, clique em "Runner".
Selecione a collection que você deseja rodar em massa.
Escolha o environment correspondente ao seu ambiente de ACI.
Carregue um arquivo CSV contendo as variáveis que serão aplicadas nas requisições (exemplo incluído na pasta examples).
Clique em Run para executar as requisições em massa.

## Contribuições
Contribuições são bem-vindas! Se você tiver melhorias ou sugestões, sinta-se à vontade para abrir uma issue ou enviar um pull request.

