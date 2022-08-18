# Probabilidad

# ¿Qué es la probabilidad?

La probabilidad es una creencia que tenemos sobre la ocurrencia de eventos elementales.

¿En qué casos usamos la probabilidad?

Intuitivamente, hacemos estimaciones de la probabilidad de que algo ocurra o no, al desconocimientoque tenemos sobre la información relevante de un evento lo llamamos incertidumbre.

El azar en estos términos no existe, representa la ausencia del conocimiento de todaslas variables que componen un sistema.

En otras palabras, la probabilidad es un **lenguaje** que nos permite **cuantificar** la incertidumbre

**AXIOMAS**:Es un conjunto de sentencias que no son derivables de algo más fundamental. Las damos por verdad y no requieren demostración.

- “A veces se compara a los axiomas con semillas, porque de ellas surge toda la teoría”

## **AXIOMAS DE PROBABILIDAD**

La probabilidad está dada por el número de casos de éxito sobre la cantidad total(teórica) de casos.

- $P=\frac{N°Sucesos-exitosos}{N°sucesos-totales}$
- **Suceso elemental**: Es una única ocurrencia, “Solo tienes una cara de la moneda como resultado”
- **Sucesos**: Son las posibilidades que tenemos en el sistema. Está compuesto de sucesos elementales,por ejemplo, “El resultado de lanzar un dado es par”, hay tres sucesos (2,4,6) que componen este enunciado.

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled.png)

**Escuela frecuentista**

“Toda variable aleatoria viene descrita por el espaci muestral que contiene todos los posibles sucesosde ese problema aleatorio.”

La probabilidad que se asigna como un valor a cada posible suceso tiene varias propiedades por cumplirse

PROPIEDADES AXIOMAS:

- 0 <= P <= 1
- Certeza: P = 1
- Imposibilidad P = 0
- Disyunción P(AuB) = P(A) +P(B)

# Probabilidad en Machine Learning

**¿Cuáles son las fuentes de incertidumbre?**

- Datos: Debido a que nuestros instrumentos de medición tienen un margen de error, se presentan datos imperfectos e incompletos, por lo tanto hay incertidumbre en los datos.
- Atributos del modelo: Son variables que representan un subconjunto reducido de toda la realidad del problema, estas variables provienen de los datos y por lo tanto presentan cierto grado de incertidumbre.
- Arquitectura del modelo: Un modelo en mates es una representación simplificada de la realidad y al ser así, por construcción, induce otra capa de incertidumbre, ya que al ser una representación simplificada se considera mucho menos información.

**Y claro, todo esta incertidumbre se puede cuantificar con probabilidad:**

**Ejemplo, un clasificador de documento de texto:**

[1-7f1c567a-ea6d-4cbd-b151-9eb21c655520.webp](Probabilidad%201979a1f06d414caf94bc421bbb517806/1-7f1c567a-ea6d-4cbd-b151-9eb21c655520.webp)

Entonces, el modelo asignara cierta probabilidad a cada documento y así de determinara la clasificación de los documentos.

Pero, ¿cómo funciona por dentro nuestro modelo de clasificación?

[2-84ba3506-44dd-46e8-8e3b-72d4330bf8e1.webp](Probabilidad%201979a1f06d414caf94bc421bbb517806/2-84ba3506-44dd-46e8-8e3b-72d4330bf8e1.webp)

**En dónde se aplica la probabilidad?**

Bueno, en realidad no todos los modelos probabilístico, a la hora de diseñarlo nosotros elegimos sui queremos que sea un modelo probabilístico o no.

Por ejemplo si escogemos el modelo de Naive Vayes, luego de que escogemos el diseño ahora definimos el entrenamiento y este es básicamente que el modelo aprenda el concepto de distribución de probabilidad y es una manera que yo uso para saber que probabilidades le asigno una de las posibles ocurrencias de mis datos, de ahí sirgue el esquema MLE que es el estimador de máxima verosimilitud y luego de esto esta la calibración se configuran los hiper-parámetros, esto se entiende mas en redes neuronales artificiales en donde el numero de neuronas de una capa tiene 10 neuronas y cada una tiene sus propios pesos que conectan a las neuronas, entonces esos pesos los podemos ir calibrando para que el modelo sea cada vez mas pequeño. Sin embargo, hay parámetros están fuera del modelo y no se pueden calibrar y a esos parámetros les llamamos hiper-parámetros, porque están fuera de todo ese esquema de optimización. Al final se hace la optimización de los hiper parámetros. Y al final tenemos la interpretación, para interpretar hay veces que se tiene que saber el funcionamiento del modelo y aplicar conceptos de estadística para poder interpretarlo.

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%201.png)

# Tipos de probabilidad

- conjunt (joint)
- Marginal
- Condicional

[Ej1-35ebb925-624e-4cf6-b05d-4e2f8eeb5f7e.webp](Probabilidad%201979a1f06d414caf94bc421bbb517806/Ej1-35ebb925-624e-4cf6-b05d-4e2f8eeb5f7e.webp)

[Ej2-e254404d-f2a0-42fd-884c-9f9da0429002.webp](Probabilidad%201979a1f06d414caf94bc421bbb517806/Ej2-e254404d-f2a0-42fd-884c-9f9da0429002.webp)

[Ej3-463be177-e937-4f32-a28f-bbee45931335.webp](Probabilidad%201979a1f06d414caf94bc421bbb517806/Ej3-463be177-e937-4f32-a28f-bbee45931335.webp)

 

[TIPOS DE PROBABILIDAD-e7ed0c5b-080d-4403-a7ab-9c871523cd11.webp](Probabilidad%201979a1f06d414caf94bc421bbb517806/TIPOS_DE_PROBABILIDAD-e7ed0c5b-080d-4403-a7ab-9c871523cd11.webp)

# Correlaciones de eventos

**Correlación entre sucesos:**Decimos que dos sucesos están correlacionados si la ocurrencia de uno varía difectamente sobre la probabilidad del otro, pueden ser:

- Correlación positiva: la ocurrencia de un suceso incrementa la probabilidad de ocurrencia del otro
- Correlación negativa: la ocurrencia de un suceso disminuye la probabilidad de ocurrencia del otro

**Nota:**

- Dos elementos excluyentes no son independientes, todo lo contrario tienen correlación negativa

# ¿Qué es una distribución?

Una distribución de probabilidad es una función que toma una variable aleatoria y a cada uno de sus estados le asigna una probabilidad.

## Distribución discreta

### Distribución de Bernoulli

Permite distribuir ocurrencias binarias.

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%202.png)

### Distribución binomial

Secuencias repetitivas de eventos binarios tipo Bernoulli

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%203.png)

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%204.png)

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%205.png)

# Distribuciones continuas

## Distribución normal (gaussiana)

$$
P(X)=\frac{1}{\sigma\sqrt{2\pi}}\exp-\frac{1}{2}\left( \frac{X-\mu}{\sigma}\right)^2
$$

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%206.png)

# ¿Cómo estimar una distribución?

Distribución de probabilidad

a **estimacion paramétrica**
 consiste en suponer una función para la distribución y ajustar los parámetros de los datos a dicha distribución. Por otro lado, la **estimación no paramétrica**
 se aplica cuando los datos no se ajustan a ninguna distribución conocida.

Se basa realizar el cálculo de una distribución teórica, cuyos parámetros se basan en la información o en el conjunto de datos con el que estamos trabajando. En el ejemplo en clase, primero se calcula un conjunto de datos aleatorios, que sigue a una distribución normal, cuya media será 50 y el desvío estandar será de 5. Esto se genera a partir de la siguiente línea de código:

```python
sample = normal(loc = 50, scale = 5, size = 1000) #Donde loc es la media y scale el desvío estandar

```

Si graficamos el resultado, veremos algo como lo expuesto en la siguiente imagen, la cual tiene una forma de distribución normal:

![https://static.platzi.com/media/user_upload/normal-be3702d2-5609-4369-9772-1d6c77487592.jpg](https://static.platzi.com/media/user_upload/normal-be3702d2-5609-4369-9772-1d6c77487592.jpg)

El siguiente paso es calcular una función teórica que se ajuste al conjunto de datos. En este caso se conoce la media y el desvío porque los colocamos nosotros para realizar la simulación, pero en una situación real, se debe calcular la media y el desvío tal como lo hizo el profe, y esto se ve en la siguiente línea de código:

```python
mu = sample.mean()
sigma = sample.std()

```

Con estos valores, se crea una instancia de un objeto cuyos parámetros son precisamente mu y sigma. Es decir, tenemos la base para aplicar la fórmula de la función de distribución Gauseana, pero nos fatan los valores sobre los cuales vamos a calcular esas probabilidades. Entonces primero se crea el objeto y luego se genera un array cuyo rango va a variar entre los extremos de los datos reales y calculamos las probabilidades. Todo esto se ejecuta en las siguientes líneas de código:

```python
dist = norm(mu, sigma)
values = [valueforvalueinrange(30,70)]
probabilidades = [dist.pdf(value)forvaluein values]

```

Si graficamos ahora solo la función teórica nos queda lo siguiente:

![https://static.platzi.com/media/user_upload/normal_teorica-d808cadc-8cdf-415c-bdc5-29be644d4bad.jpg](https://static.platzi.com/media/user_upload/normal_teorica-d808cadc-8cdf-415c-bdc5-29be644d4bad.jpg)

Finalmente, graficamos los datos y la curva teórica calculada y observamos que se asemejan.

![https://static.platzi.com/media/user_upload/curva_ajustada-98feda91-eaee-4cdb-b517-15f185117ded.jpg](https://static.platzi.com/media/user_upload/curva_ajustada-98feda91-eaee-4cdb-b517-15f185117ded.jpg)

<h4>Estimación No Paramétrica</h4>

Este proceso se aplica cuando los datos no se ajustan a una distribución conocida. Entonces no forzamos ajustar los datos a una única distribución, sino a un conjunto de distribuciones.En este ejemplo, el profe utiliza un método que ya viene incluído dentro de la librería de ScikitLearn, el cual se llama Kernel Density Estimation. Para ello, primero se simulan dos conjuntos de datos a través de dos funciones normales y se juntan en luego en una sola variable a través del método hstack(). Esto lo vemos en las siguientes líneas del código:

```python
sample1 = normal(loc = 20, scale = 5, size = 300)
sample2 = normal(loc = 40, scale = 5, size = 700)
sample = hstack((sample1, sample2))

```

El resultado lo vemos en la siguiente imagen:

![https://static.platzi.com/media/user_upload/dist_bimodal-7b9e35b7-9aa7-4310-bb85-ca3ddb788729.jpg](https://static.platzi.com/media/user_upload/dist_bimodal-7b9e35b7-9aa7-4310-bb85-ca3ddb788729.jpg)

Luego, una vez que tenemos los datos simulados, comienza el proceso de estimación, para ello se crea un objeto modelo, el cual se instancia a través de los parámetros bandwidth (parámetro de suavizado) y kernel (funciones de distribución que se usan para la estimación). Esto es equivalente al método anterior, donde teníamos la función normal teórica, y luego calculábamos las probabilidades, solo que ahora no tenemos solo una función de densidad de probabilidad, sino un conjunto de distribuciones. Una vez creado el objeto, se ajustan los datos a las necesidades del objeto, para esto se utiliza el método reshape, el cual los ordena en una matriz de 1000 filas y 1 columna y luego se ajusta el modelo a estos datos. Esto se hace con las siguientes líneas de codigo:

```python
model = KernelDensity(bandwidth = 2, kernel = 'gaussian')
sample =sample.reshape((len(sample), 1))
model.fit(sample)

```

Ahora, como dije antes, estamos ajustando el modelo a los datos, es como si estuvieramos calculando la media y el desvío estandar de una distribución normal pero nos faltan calcular los promodios para darle forma a la función teórica. Esto es lo que hacemos a continuación, se crea un array en el rango de los datos reales sobre cuales queremos estimar la función, y luego calculamos las probabilidades. Esto se hace en las siguientes líneas del código. Una aclaración, el cálculo de forma logarítimica tiene que ver con la complejidad algorítmica, es una cuestión de eficiencia. Luego a través de función inversa, la exponencial, obtenemos las probabilidades.

```python
values = np.asarray([valuefor valuein range(1, 60)])
values = values.reshape((len(values), 1))
probabilities = model.score_samples(values) #probabilidad logarítmica para facilitar los calculos
probabilities = np.exp(probabilities)  # inversión de probabilidad obtenemos el valor original

```

Esto nos devuelve la siguiente curva:

![https://static.platzi.com/media/user_upload/dist_bimodal_teorica-d0567bc7-6f92-4b81-b265-8c93719110e7.jpg](https://static.platzi.com/media/user_upload/dist_bimodal_teorica-d0567bc7-6f92-4b81-b265-8c93719110e7.jpg)

La cual, en conjunto con los datos finalmente queda de la siguiente forma:

![https://static.platzi.com/media/user_upload/curba_bimodal_estimacion-7c7ebf98-e0a3-4913-93b6-9b959151a8b6.jpg](https://static.platzi.com/media/user_upload/curba_bimodal_estimacion-7c7ebf98-e0a3-4913-93b6-9b959151a8b6.jpg)

# ¿Qué es MLE?

Estimación de máxima verosimilitud

Un framework para estimación de densidad de densidad de probabilidad.

**Elementos de MLE**

- Escoger la distribución:
    - Teniendo solo una muestra de los datos
- Escoger los parámetros de la distribución:
    - Que mejor ajustan la distribución a los datos.

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%207.png)

## MLE en Machine Learning

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%208.png)

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%209.png)

Tengo un conjunto de datos el cual quiero ajustar a un modelo lineal. Esta debe cumplir con $y=mx+b$

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%2010.png)

Suponemos que el “ruido” de los datos (la desviación con la recta) sigue una distribución gaussiana. 

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%2011.png)

Lo que se busca es minimizar la suma de todos los errores cuadráticos

**Métodos de mínimos cuadrados**

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%2012.png)

$$
max\{\sum_i\log P(y_i,x_i;h)\}=max\{\sum_i \log \left( \frac{1}{\sigma\sqrt{2\pi}} \exp(\frac{-1}{2} \left( \frac{(y_i-(mx_i+b))}{\sigma} \right)^2\right)\}
$$

[5-ea11996f-4c43-46dd-bb46-27843c1554ef.webp](Probabilidad%201979a1f06d414caf94bc421bbb517806/5-ea11996f-4c43-46dd-bb46-27843c1554ef.webp)

# Teorema de Bayes

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%2013.png)

**MAP (Maximum a Posteriori Probability)**De la misma manera que el algoritmo MLE consiste en maximizar la probabilidad para ajustarla mejor a los datos:P(h|D) = P(D|h)P(h)/P(D)→ max P(h|D) = max P(D|h)P(h)Eliminamos P(D) puesto que es el mismo valor para el conjuto de datos

**Nota:**

- Puesto que no podemos hallar la probabilidad de la verosimilitud de manera exacta (Lo que lllamaríamos un modelo Optimal Bayes) puesto que computacionalmente es muy complicado, simplificamos el modelo a la probabilidad de cada uno de los atributos (Modelo conocido como Naive Bayes):P(D|h) = P(X1,X2,…,Xn|h) = P(X1|h)P(X2|h)…P(Xn|h)

![Untitled](Probabilidad%201979a1f06d414caf94bc421bbb517806/Untitled%2014.png)

En MLE escogemos los parámetros de la distribución de manera que: