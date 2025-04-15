# CHAVES ESTRANGEIRAS NO POSTGRESQL

## CHAVES ESTRANGEIRAS

É uma coluna de uma tabela que faz referência a chave primária de outra tabela.

## SINTAXE

```
    FOREIGN KEY (nome_do_campo_tabela_atual) REFERENCES nome_da_tabela_extra (nome_do_campo_da_tabela_extra)
```

## CARDINALIDADE 1 x N

![1xN](1xN.png)

Nesse relacionamento, basicamente está sendo dito isso: 1 professor "dá aula em" MUITOS (N) cursos.

## CARDINALIDADE N x 1

![nX1](Nx1.png)

Nesse relacionamento, basicamente está sendo dito isso: vários cursos são dados por 1 professor.

## PRÁTICA

```
----------

EXEMPLO 01: CRIANDO TABELAS RELACIONADAS

CREATE TABLE professores (
	id serial PRIMARY KEY,
	nome varchar(100)
);

CREATE TABLE cursos (
	id serial PRIMARY KEY,
	nome varchar(100),
	idprofessor integer,
	FOREIGN KEY (idprofessor) REFERENCES professores(id)
);

----------

EXEMPLO 02: INSERINDO VALORES NAS DUAS TABELAS

INSERT INTO professores (id, nome) values (1, 'Sebastião');
INSERT INTO professores (id, nome) values (2, 'Josué');

SELECT * FROM professores;

INSERT INTO cursos (nome, idprofessor) VALUES ('PHP', 1);
INSERT INTO cursos (nome, idprofessor) VALUES ('C#', 2);

----------
```