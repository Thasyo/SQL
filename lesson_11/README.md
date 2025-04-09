# COMANDO UPDATE NO POSTGRESQL

## COMANDO UPDATE

É um comando simples SQL que usamos para atualizar os registros de uma tabela.

## SINTAXE

```
    UPDATE nome_da_tabela 
    SET nome_do_campo = novo_valor_do_campo 
    WHERE condição;
```

## PRÁTICA

```
Exemplo 01:

UPDATE cursos 
SET nome = 'SQL' 
WHERE id = 1;

----

Exemplo 02:

UPDATE cursos 
SET nome = 'Java e Spring' 
WHERE id = 2;

----

Exemplo 03:

UPDATE professores 
SET nome = 'Thasyo Peres', especialidade = 'PHP' 
WHERE id = 1;

----

Exemplo 04:

UPDATE professores 
SET salario = salario * 1.1 
WHERE dataadmissao <= '31/12/2018';
```

## IMPORTANTE

Sempre que for atualizar algo do banco, não esqueça do WHERE. Pois, se caso seja executado algum script de UPDATE sem WHERE, todos os dados da tabela em questão serão atualizar com o valor em questão.

## EXEMPLO

```
UPDATE cursos 
SET nome = 'Curso de PHP';
 
JAMAIS FAÇA ISSO.
```