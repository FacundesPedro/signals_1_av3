# Letra A
Para facilitar colocamos variáveis nas realimentações e analisamos o sistema

## Realimentação 1

$$ e1(s) = { x(s)*s^-1 + 1/4 * y(s) } $$

## Realimentação 2

$$ e2(s) = { e1(s)*s^-1 + x(s) } $$

## Saída

$$ y(s) = { e2(s)*s^-1 } $$ 

Aplicamos e1(s) em e2(s) para remover as variáveis que não precisamos


$$ e2(s) = { x(s)*s^-2 + 1/4*y(s)*s^-1 + x(s) } $$


E o aplicamos na saída y(s) 


$$ y(s) = { x(s)*s^-3+1/4*y(s)*s^-2+x(s)*s^-1 } $$


Isolamos x(s) e y(s) e obtemos nossa função de transfêrencia H(s)
```js
 y(s)(1 - 1/4*s^-2) = x(s)(s^-3 + s^-1);
```

Multiplamos ambos numerador e deminador por "s^3" para evitar problemas com a fração parcial que usaremos nas proximas letras, e por fim achamos: 

$$ H(s) = {1+s^2 \over s^3-1/4*s} $$
