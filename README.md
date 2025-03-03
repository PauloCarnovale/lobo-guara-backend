# Lobo-Guará Backend

## Requisitos

- Node.js v22.14.0  
- Yarn  
- Docker e Docker Compose  

## Instalação

Clone o repositório:

```sh
git clone 
cd lobo-guara-backend
```

## Instale as dependências:

```sh
yarn install
```

## Configuração do Banco de Dados

### Suba o container do banco de dados com Docker Compose:

```sh
docker-compose up -d
```

### Crie o arquivo .env na raiz do projeto e configure as variáveis de ambiente:

DATABASE_HOST=
DATABASE_PORT=
DATABASE_USER=
DATABASE_PASSWORD=
DATABASE_NAME=

## Executando o Projeto

### Rode as migrações do banco:

```sh
yarn prisma migrate deploy
```

## Inicie a aplicação:

```sh
yarn start:dev
```

#A API estará disponível em http://localhost:3000/docs.

## Caso queira usar Postman ou similares para fazer as requisições HTTP 
    http://localhost:3000/