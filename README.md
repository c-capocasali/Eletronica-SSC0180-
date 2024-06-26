## Projeto Fonte de Tensão Regulável

### Objetivo 
O objetivo principal do projeto foi construir uma fonte de tensão ajustável, que converte corrente alternada (AC) em correte contínua(DC), funcionando na faixa de 3 a 12 V e 100mA. 


### Teoria 

#### Tensão alternada e Transformador
Inicialmente a tensão varia ao longo do tempo na forma de uma senoide: 

(Mostrar gráfico); 

Ao passar pelo transformador, a tensão é reduzida, respeitando a relação 

$\frac{V_{E}}{V_{S}} = N1/N2$ (i); 

Ou seja, a amplitude da onda é reduzida. 



#### Ponte retificadora e Capacitor: 
A ponte retificadora é formada por 4 diodos. O principal objetivo dessa parte do circuito é converter a corrente alternada em corrente contínua. Ou seja, a tensão será sempre positiva. 

(Mostrar gráfico); 


Contudo, apesar de não ser negativa, a tensão ainda sofre uma variação muito significativa. Portanto, devemos deixar a tensão contínua. 

(Gráfico)


Para tal, utilizou-se o capacitor. Esse componente tem como objetivo diminuir a variação da tensão e da corrente em altas frequências. 

Ao calcular a difença entre o ponto mínimo da tensão e o ponto máximo, obtemos a chamada "tensão ripple" ($V_{r}$). A tensão Ripple será uma medida muito relevante futuramente para a resolução dos cálculos do circuito. 


(Mostrar o gŕafico Ripple)


#### Diodo Zener 
O papel do Zener é eliminar as pequenas variações remanascentes da tensão. Ou seja, torna o gráfico da tensão uma reta constante. 

#### Potenciômetro 
O potenciômetro é um resistor de resistência ajustável. No circuito, sua função consiste em regular o valor da tensão. No caso, o intervalo de variação será de 3 a 12V. 


### Cálculos 

#### Tensão de saída
Inicialmente, medimos com o auxílio de um multímetro o valor de saída $V_{S} \approx 18V$. 

Após passar pela ponte de diodos, há uma queda de tensão. Por serem compostos majoritariamente de silício, cada diodo usa, aproximadamente, 0.7V. Em cada ciclo, dois diodos são usados, portanto, a queda de tensão total é de 1,4V. Dessa forma, a nova tensão nos capacitores é de $V'_{S} = 16,6V$. 


#### Cálculo da capacitância 
A capacitância pode ser obtida através da seguinte função: 

C = \frac{I}{f*V_{ripple}}







