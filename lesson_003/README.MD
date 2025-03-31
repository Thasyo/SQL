# Criando Tabelas

## PgAdmin (Query Tool)

```
    create table professores (
        id integer,
        nome varchar(100),
        especialidade(255)
    )
```

## PgAdmin (manualmente)

- botão direito do mouse em tables >> create >> preencher informações da tabela >> enter

## SQL Shell

- Entrar no servidor

```
    create table professores (
        id integer,
        nome varchar(100),
        especialidade(255)
    ); 
```