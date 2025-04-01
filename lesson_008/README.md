# OPERADORES LÓGICOS NO POSTGRESQL

## OPERADORES LÓGICOS

Assim como os operadores de comparação, nós utilizamos esses operadores para melhorar as condições que usamos para filtrar resultados de uma consulta.

|  Sinal  |   valor   |
|---------|-----------|
|   AND   |     e     |
|   OR    |     ou    |


## PRÁTICA

```
SELECT * FROM professores WHERE dataadmissao >= '01/01/2020' AND dataadmissao <= '31/12/2020'; -- retorna todos os professores admitidos no ano de 2020.

SELECT * FROM professores WHERE dataadmissao >= '01/01/2021' AND dataadmissao <= '31/12/2021' AND inativo = false; -- retorna todos os professores admitidos no ano de 2021 e estão ativos.

SELECT * FROM professores WHERE especialidade = 'Java' OR especialidade = 'Angular'; -- retorna todos os professores especialistas em Java ou Angular.
```
