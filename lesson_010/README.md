# COMANDO DELETE NO POSTGRESQL

## COMANDO DELETE

É um comando simples SQL que usamos para deletar os registros de uma tabela.

## SINTAXE

```
    DELETE FROM nome_da_tabela where condição_do_delete;
```

## PRÁTICA

```
DELETE FROM professores WHERE id = 1

DELETE FROM professores WHERE inativo = true

DELETE FROM professores WHERE especialidade = 'HTML'
```

## IMPORTANTE

Sempre que for deletar algo do banco, não esqueça do WHERE. Pois, se caso seja executado algum script de DELETE sem WHERE, todos os dados da tabela em questão serão removidos.

## EXEMPLO

```
DELETE FROM professores -- JAMAIS FAÇA ISSO. 
```