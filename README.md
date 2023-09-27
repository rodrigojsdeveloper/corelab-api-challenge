<div align="center">
<h1>Corelab Challenge</h1>
<p>
CoreNote é um aplicativo da web que possibilita aos usuários a criação e administração de suas próprias listas de tarefas. O aplicativo compreende uma página da web responsiva com funcionalidades avançadas, complementada por uma API robusta para armazenamento e gerenciamento eficaz das listas de tarefas.
</p>
</div>

<br/>

## Tecnologias

Seguintes ferramentas foram usadas neste projeto:

- [Nodejs](https://nodejs.org/en/)
- [TypeScript](https://www.typescriptlang.org/)
- [Express](https://expressjs.com/)
- [PostgreSQL](https://www.postgresql.org/)
- [Jest](https://jestjs.io/pt-BR/)
- [Swagger](https://swagger.io/)

<br />

## Instalação do Projeto

Projeto desenvolvido em Node com TypeScript.

### 1. Instalação das dependencias

Execute a instalação das dependências executando `yarn` no terminal.

### 2. Configuração do .env

Crie um arquivo `.env` com base no arquivo `.env.example`.

#### Para sistemas Linux, você pode usar o seguinte comando:

```
cp .env.example .env
```

### 3. Iniciando o Projeto

Na raiz do projeto execute o seguinte comando:

```
yarn dev
```

Em seguida, faça uma requisição usando o Insomnia ou outra ferramenta similar.

#### Exemplo de requisição - POST

```
{
  "title": "John doe",
  "description": "Lorem Ipsum.",
  "is_favorite": false,
  "color": "#FFFFFF"
}
```

### 3. Iniciando o Projeto no Docker

```
# Construa a imagem Docker para a pasta atual e com `dockerized-node`

docker build . -t dockerized-node


# Verifique se a imagem foi criada

docker images | grep dockerized-node


# Execute a imagem no modo desanexado e mapeie a porta 3000 dentro do contêiner com 3000 no host atual

docker run -p 3000:3000 -d dockerized-node
```

A flag -d executa o projeto em segundo plano, liberando o terminal para outros usos.

### 4. Documentação

Com o projeto em execução, acesse http://localhost:3000/api/docs para visualizar a documentação.

<br/>
<p align="center">Feito por <a href="https://www.linkedin.com/in/rodrigo-de-jesus-silva/">Rodrigo Silva</a></p>
