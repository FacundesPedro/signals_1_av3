# Letra B
Para encontrar uma função diferencial que represente o sistema, antes precisamos isolar a saída y(s) e efetuar a transformada inversa para encontrar seu valor no tempo;

Sendo a

$$ H(s) = {  y(s) \over x(s) } $$ 

em s, podemos afirmar que 

$$ y(s) = { H(s) * x(s) } $$

assim, 

$$ y(t) = Laplace^-1 ( y(s) ) $$ 

 Tendo a função de transfêrencia descrita como 
 
 $$ H(s) = {s^2 + 1 \over s^3 - 1/4*s} $$ 

 Achamos as raízes (0, +1/2, -1/2) do denominador para fatorá-lo, e facilitar sua transformada (transformada da soma é a soma das transformadas) e remodelamos o saída para 
 
 $$ y(s) = { A/s + B/(s+1/2) + C/(s-1/2) } $$

 Aplicando cada uns dos limites de cada polo (raiz) achamos que
 
 $$ A = -4 $$
 
 $$ B =  5/2 $$
 
 $$ C = 5/2 $$

 Aplicamos algumas transformadas já conhecidas 
 
 ### Laplace^-1
 
 $$  1/s  = t $$

 ### Laplace^-1
 
 $$ e^at = { 1 \over s-a } $$

Temos então que y(t) será soma de todas as transformadas

$$ y(t) = { (-4t) + (5/2 * e^t/2) + (5/2 * e-t/2) } $$ 

 Aplicando na entrada uma função conhecida como o degrau 
 
 $$ u(t) = 1 $$

 Temos então que
 
 $$ y(t) = -4t *1 + (5/2 * e^+t/2)*1 + (5/2 * e^-t/2)*1 $$
 
 *Degrau*

$$ h = {  y \over x } $$
