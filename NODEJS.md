# Node.js

Página para estudo de Node.js.

## __Modules__
## _Assert_
O módulo `Assert` fornece um conjunto de funções de afirmações para verificar inváriáveis.

## Modo strict
No modo _strict_ métodos *non_strict* tem o mesmo comportamento dos métodos _strict_ correspondentes.
Ex.:
No código abaixo irá lançar um erro do tipo _AssertionError_, pois '3' é diferente de 3.
```
const assert = require('assert').strict;
assert.deepEqual([[[1, 2, 3]], 4, 5], [[[1, 2, '3']], 4, 5]);
```

Já no exemplo abaixo, não irá lançar o erro, pois não está no modo _strict_:
```
const assert = require('assert');
assert.deepEqual([[[1, 2, 3]], 4, 5], [[[1, 2, '3']], 4, 5]);
```
É recomendado usar o modo _strict_ para não causar resultados surpreendentes.