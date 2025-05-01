# INNER JOIN NO POSTGRESQL

## COMANDO INNER JOIN

Usamos o comando inner join quando precisamos criar um select que busca os dados em mais de uma tabela.

## SINTAXE

SELECT * 
FROM nome_tabela_01 
INNER JOIN nome_tabela_02 ON condicao_para_juncao

## PRÁTICA

```
----------

EXEMPLO 01:

SELECT *
FROM cursos 
INNER JOIN professores ON cursos.idprofessor = professores.id;

- Traz todos os registros das tabelas CURSOS e PROFESSORES onde a coluna idprofessor da tabela CURSOS é igual a coluna id da tabela PROFESSORES.

----------

EXEMPLO 02:

SELECT
	cursos.nome as curso,
	professores.nome as professor
FROM cursos 
INNER JOIN professores ON cursos.idprofessor = professores.id;

- Traz os mesmos registros da consulta anterior, só que com um layout mais amigável e legível.

----------
```

