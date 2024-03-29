
# Project

Este repositório contém dois projetos principais, um frontend desenvolvido em ReactJS (`front`) e um backend desenvolvido em NestJS (`back`).

## Estrutura do Repositório

O repositório está organizado da seguinte forma:

- `front`: Contém o código-fonte do projeto frontend desenvolvido em ReactJS.
- `back`: Contém o código-fonte do projeto backend desenvolvido em NestJS.

## Instruções de Acesso aos Projetos

### Frontend (ReactJS)

Para configurar e iniciar o projeto frontend, acesse a pasta `front` e siga as instruções no README específico dessa pasta. Você pode encontrar o README aqui: [README Frontend](front/README.md).

### Backend (NestJS)

Para configurar e iniciar o projeto backend, acesse a pasta `back` e siga as instruções no README específico dessa pasta. Você pode encontrar o README aqui: [README Backend](back/README.md).


# Instruções de Configuração do Banco de Dados

Para configurar o banco de dados necessário para este projeto, siga as instruções abaixo.

## Criação da Tabela `usuarios`

Execute o seguinte comando SQL para criar a tabela `usuarios` no banco de dados:

```sql
CREATE TABLE usuarios (
    id serial4 NOT NULL,
    nome varchar(100) NOT NULL,
    email varchar(100) NOT NULL,
    telefone numeric NOT NULL,
    coordenadas varchar(80) NULL,
    CONSTRAINT usuarios_pkey PRIMARY KEY (id)
);

INSERT INTO usuarios (nome, email, telefone, coordenadas)
VALUES ('empresa', 'empresa@empresa.com', 626262622, '-15.788371756563562,-47.90382385253907');

```

Esta tabela irá armazenar informações dos usuários, incluindo nome, email, telefone e coordenadas.

## Configuração Adicional

Certifique-se de que seu banco de dados esteja corretamente configurado e acessível pelos projetos front e back. Para detalhes específicos sobre a configuração do banco de dados nos projetos, consulte os READMEs individuais.
