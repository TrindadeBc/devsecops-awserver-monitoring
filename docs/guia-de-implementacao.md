# Guia de Implementação Técnica - DevSecOps Web Monitorado

## Etapa 1: Infraestrutura AWS

### 1. Criação da VPC
...

### 2. Sub-redes públicas e privadas
...

## Etapa 2: Configuração da EC2 com NGINX
...

## Etapa 3: Script de Monitoramento + Telegram

  ### Uso de variáveis sensíveis via .env

  O script de monitoramento utiliza o arquivo `.env` na raiz do projeto para carregar:

- `TELEGRAM_TOKEN`
- `TELEGRAM_CHAT_ID`

Certifique-se de que o `.env` foi criado antes de executar o script.


## Etapa 4: Testes de Falha + Logs
...

## Etapa 5: Automação (User Data ou CloudFormation)
...

## Considerações de Segurança
- Evitar tokens expostos
- Uso de `.gitignore

## Configuração do Arquivo .env

O projeto utiliza um arquivo `.env` na raiz para armazenar dados sensíveis que não devem ser versionados.

GIT_TOKEN="ghp_xxxxxxxxxxxxxxxxxxxxx"
TELEGRAM_TOKEN="xxxxxxx:xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
TELEGRAM_CHAT_ID="xxxxxxxxx"


Esse arquivo está protegido via `.gitignore` e deve ser criado manualmente ao configurar o ambiente.

