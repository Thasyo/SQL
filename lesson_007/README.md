# COMANDO SELECT NO POSTGRESQL

## COMANDO SELECT

É um comando simples SQL que usamos para visualizar os registros de uma tabela.

## SINTAXE

```
    SELECT nome_da_coluna FROM nome_da_tabela;
```

## PRÁTICA

```
SELECT * FROM professores; -- retorna os dados de todas as colunas da tabela professores.

SELECT nome, especialidade, datanascimento, dataadmissao FROM professores; -- retorna todos os dados das colunas nome, especialidade, datanascimento, dataadmissao da tabela professores.
```

## COMANDO SELECT COM WHERE

```
    SELECT nome_da_coluna FROM nome_da_tabela WHERE condição;
```

## PRÁTICA

```
SELECT * FROM professores WHERE especialidade = 'Java'; -- Retorna todos dados da tabela professores que tem a coluna especialidade igual a "Java".
```

## OPERADORES DE COMPARAÇÃO

|  Sinal  |   valor   |
|---------|-----------|
|    =    |   igual   |
| != ou <>| Diferente |
|    >    |   Maior   |
|    <    |   Menor   |
|   >=    | Maior ou Igual |
|   <=    | Menor ou Igual |

## PRÁTICA

```
SELECT * FROM professores WHERE inativo <> true; -- retorna todos os professores ativos na tabela.
SELECT * FROM professores WHERE inativo = true; -- retorna todos os professores inativos na tabela.

SELECT * FROM professores WHERE dataadmissao > '01/01/2021 00:00:00'; -- retorna todos os professores admitidos após a data 01/01/2021 00:00:00.
SELECT * FROM professores WHERE dataadmissao >= '01/01/2021 00:00:00'; -- retorna todos os professores admitidos a partir da data 01/01/2021 00:00:00.

SELECT * FROM professores WHERE salario < 3000; -- retorna todos os professores que tem o salario menor que 3000.
SELECT * FROM professores WHERE salario <= 3000; -- retorna todos os professores que tem o salario menor ou igual a 3000.
```
