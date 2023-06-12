## La dirección en la que besamos

Hay un [artículo]([/guides/content/editing-an-existing-page](https://www.nature.com/articles/s41598-017-04942-9)) publicado en nature en 2017 y 2023 que estudia 
si los humanos tendemos a inclinar la cabeza en una dirección preferente cuando nos besamos. Aprovecharemos este estudio titulado: "The right way to kiss: directionality bias in head-turning during kissing" (2017), "Adult persistence of head-turning asymmetry A neonatal right-side preference makes a surprising romantic reappearance later in life" (2003).



## preguntas que nos podemos hacer inicialmente
- ¿Tenemos una preferencia por la dirección en la que inclinamos nuestra cabeza? Hay estudios en infantes que reportan que los infantes tienen una tendencia a inclinar más su cabeza a la derecha que hacia la izquierda.

## Planteamiento del problema
Sea p  la proporción de las parejas que inclinan su cabeza hacia la derecha al besar. Buscamos estimar p partiendo de datos que nos describen la dirección en la que besan n parejas besandose.
Para responder a la pregunta: ¿Los humanos, tenemos una dirección preferencial en la que inclinamos la cabeza al besarnos en pareja?

## Modelado
Modelaremos este problema con una distribución binomial, pensando en cada beso como un experimentos de Bernoulli anotando con {1} si la pareja besa a la izquierda y con {0} si besa a la derecha. 

## Datos
De 124 parejas besándose, 80 (64.5%) inclinaron su cabeza a la derecha and 44 (35.5%)
se inclinaron a su izquierda.

Sea $R_i \in {0,1}$ el resultado de la i-ésima medición. Definiremos el estimador de la proporción p como la media muestral:

$$  \hat p = \frac{1}{n}  \sum_{i=1}^n R_i$$

$$\hat p = 80/124 =64.5% $$


## Suposiciones
1. Cada $R_i$ es una variable aleatoria del tipo de Bernoulli con parametro p.
2. Las mediciones $R_1, R_2 ,...,R_n$ son mutuamente independientes.
## ¿Tienen sentido estas suposiciones?
1. Estamos modelando con variables aleatorias nuestra falta de información de lo que sucede en la cabeza de las parejas. Este experimento al tener dos posibles resultados es una variable aleatoria de Bernoulli, Sin embargo es una *fuerte* suposición decir que todas los experimentos mantienen el mismo parámetro p. ¿Podemos justificar que nuestras mediciones provienen del mismo proceso?
2. La independencia es razonable, ya que las mediciones se realizaron en distinos lugares y tiempos.


## Análisis.
Utilizaremos la Ley de números grandes, que dice que si tenemos una sucesión de variables aleatorias con el mismo valor esperado y la misma varianza su promedio converge en probabilidad a su valor esperado.

y el teorema central del límite, que nos dice que la distribución de medias muestrales sigue una distribución normal tal que

- $E[x] = \mu$, entonces $E[\bar{x}]=\mu$
- $Var[x] = \sigma^{2}$, entonces $Var[\bar{x}]=\frac{Var[x]}{N}$
- implicando$\sigma [\bar{x}]=\frac{\sigma[x]}{\sqrt(N)}$ 

El intervalo de confianza para la estimación de una proporción p, puede estimarse utilizando el teorema central del límite. La distribución de la media muestral se distribuye normalmente. El intervalo de confianza para una proporción p es:

$$ P \left( \hat p - Z_{1- \alpha /2} \sqrt{\frac{\hat p (1- \hat p)}{n}} \leq p \leq \hat p + Z_{1- \alpha /2} \sqrt{\frac{\hat p (1- \hat p)}{n}} \right)  = 1-\alpha $$

El cual calculamos con un nivel de confianza de 95%, para obtener una

cota inferior = 0.5542
cota superior = 0.7290

Con este resultado podemos concluir con 95% de confianza que más de la mitad de la población se inclina hacia la derecha al besar.



