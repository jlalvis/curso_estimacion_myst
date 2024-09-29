# Regresión lineal

**Authors:** Jorge López<sup>1</sup> \
**Affiliations:** <sup>1</sup>FI, UNAM \
**License:** CC-BY

**Resumen**

La regresión lineal es un método estadístico utilizado para modelar la relación entre una o más variables independientes (predictoras) y una variable dependiente (resultado). Su objetivo es encontrar una curva parametrizada que se ajuste mejor a un conjunto de puntos de datos. Cuando el modelo es lineal en sus parámetros, se clasifica como regresión lineal. Este proceso puede enmarcarse como un problema inverso lineal discreto, donde expresamos la relación usando un sistema lineal de ecuaciones representado por $Gm = d$, donde $G$ es una matriz $m \times n$, $m$ es un vector de parámetros y $d$ es un vector de observaciones {cite:p}`10.1016/B978-0-12-385048-5.00002-1`.

### Representación Matricial de Sistemas Lineales

En el contexto de la regresión lineal, la matriz $G$ contiene los coeficientes que relacionan las variables independientes con la variable dependiente. El sistema puede expresarse como:

$$
G = \begin{bmatrix}
1 & x_1 \\
1 & x_2 \\
\vdots & \vdots \\
1 & x_m
\end{bmatrix}, \quad m = \begin{bmatrix}
m_1 \\
m_2
\end{bmatrix}, \quad d = \begin{bmatrix}
d_1 \\
d_2 \\
\vdots \\
d_m
\end{bmatrix}
$$

Aquí, $m_1$ y $m_2$ son parámetros que representan la intersección y la pendiente de la línea, respectivamente. El objetivo es encontrar los valores de estos parámetros que minimicen la diferencia entre los valores observados y los predichos por el modelo.

### Solución de Mínimos Cuadrados

El método de mínimos cuadrados busca minimizar la suma de los cuadrados de los residuos (las diferencias entre los valores observados y predichos). El vector residual se define como:

$$
r = d - Gm
$$

Para encontrar la solución de mínimos cuadrados, minimizamos la norma 2 del vector residual:

$$
\|r\|^2_2 = (d - Gm)^T(d - Gm)
$$

Esto conduce a una solución dada por:

$$
m_{L2} = (G^TG)^{-1}G^Td
$$

Esta ecuación proporciona la estimación de mínimos cuadrados de los parámetros cuando $G$ tiene rango completo. Si los errores en los datos están distribuidos normalmente, esta solución de mínimos cuadrados también es estadísticamente óptima, lo que la convierte en un enfoque ampliamente utilizado en el análisis de regresión.


