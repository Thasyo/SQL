# OPERADOR LIKE NO POSTGRESQL

## OPERADOR LIKE

O operador LIKE vai nos ajudar a criar consultas SQL com filtros em campos de TEXTO.

## PRÁTICA

```
SELECT * FROM professores WHERE nome LIKE 'Fer%'; -- retorna todos os professores que iniciam com 'Fer', independente do que vem depois.

SELECT * FROM professores WHERE nome LIKE '%nda'; -- retorna todos os professores que terminam com 'nda', independente do que vem antes.

SELECT * FROM professores WHERE nome LIKE '%nda%'; -- retorna todos os professores que contém a sequencia de caracteres 'nda', independente do que vem antes e depois.

SELECT * FROM professores WHERE nome LIKE '%o'; -- retorna todos os professores que terminam com 'o', independente do que vem antes.

SELECT * FROM professores WHERE nome LIKE '%t%'; -- retorna todos os professores que contém a letra 't', independente do que vem antes e depois.

SELECT * FROM professores WHERE lower(nome) LIKE '%t%'; -- transforma os nomes para minúsculo e retorna todos os professores que contém a consoante 't', independente do que vem antes e depois.
```