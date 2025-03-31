# CRIANDO CHAVES PRIMÁRIAS NO POSTGRESQL

## CHAVE PRIMÁRIA (PRIMARY KEY)

A chave primária de uma tabela é a coluna que atua como um identificador único de cada registro.

## CRITÉRIOS

Não pode se repetir na mesma tabela. Ou seja, só pode existir uma coluna com a característica de PRIMARY KEY.

Não pode ter seu valor nulo. Ou seja, a coluna que tem como característica a PRIMARY KEY não vai aceitar valores nulos.

Detalhe: Se caso você queira adicionar a característica para que qualquer coluna não aceite valores nulos, é só adiciona a propriedade NOT NULL na coluna específica.

## PRÁTICA

```
SELECT * FROM cursos; -- seleciona todas as informações da tabela 'cursos'.

DROP TABLE cursos; -- Exclui a tabela 'cursos'.

CREATE TABLE cursos( -- cria uma tabela com o nome 'cursos'
	id SERIAL PRIMARY KEY, -- cria um campo chamado id e tipa ele como serial e adiciona a característica de primary key.
	nome VARCHAR(100) NOT NULL -- cria um campo chamado nome e tipa ele como VARCHAR(100) de 100 posições e adiciona a característica de not null (não aceita valores nulos).
)

INSERT INTO cursos (nome) VALUES ('Java') -- insere o valor 'Java' no campo nome da tabela 'cursos'.

-- -- -- -- -- -- -- -- -- -- -- -- -- -- -- --

SELECT * FROM professores; -- seleciona todas as informações da tabela 'professores'.

ALTER TABLE professores ADD PRIMARY KEY (id); -- esse comando altera a tabela 'professores' e adiciona a característica de PRIMARY KEY na coluna (id).
```
