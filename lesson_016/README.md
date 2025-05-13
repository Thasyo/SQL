# RIGHT JOIN NO POSTGRESQL

## RIGHT JOIN

Usamos o comando RIGHT JOIN quando precisamos fazer um SELECT que busca os dados em mais de uma tabela.

## SINTAXE

```

SELECT * FROM tabela_a
RIGHT JOIN tabela_b ON condicao_juncao

```

## PRÁTICA

```
----------

EXEMPLO:

SELECT cursos.nome AS curso, professores.nome AS educador 
FROM cursos RIGHT JOIN professores ON professores.id = cursos.idprofessor;

- Neste exemplo, o select vai pegar todos os dados que tem relação entre as tabelas e também todos os dados que contém na tabela a direita do comando, no caso, a tabela professores. 

----------
```
