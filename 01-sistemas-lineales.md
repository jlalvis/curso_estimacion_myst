# Sistemas lineales

**Authors:** Jorge López<sup>1</sup> \
**Affiliations:** <sup>1</sup>FI, UNAM \
**License:** CC-BY

**Resumen**

Los sistemas lineales discretos y continuos son dos tipos fundamentales de modelos matemáticos utilizados en diversas áreas. A continuación se presenta una breve explicación de sus diferencias {cite:p}`10.1016/B978-0-12-385048-5.00001-X`:

## Sistemas Lineales Discretos

Los sistemas lineales discretos involucran un número finito de puntos de datos y parámetros. En este contexto, la relación entre los parámetros del modelo $m$ y los datos observados $d$ se puede expresar mediante un sistema de ecuaciones algebraicas lineales. La forma general de tal relación es:

$$
Gm = d
$$

Donde, $G$, es una matriz que representa el sistema, $m$, es un vector de parámetros y, $d$, es un vector de observaciones. Esta formulación permite la aplicación directa de técnicas de álgebra lineal para resolver, $m$, dado $d$.

## Sistemas Lineales Continuos

Por otro lado, los sistemas lineales continuos tratan con funciones definidas sobre variables continuas, como el tiempo o el espacio. En este caso, la relación a menudo se puede expresar como una ecuación integral, típicamente en la forma:

$$
\int_a^b g(x, \xi) m(\xi) d\xi = d(x)
$$

Aquí, $g(x, \xi)$ se conoce como el núcleo, y $m(\xi)$ representa la función del modelo que debe ser estimada a partir de los datos continuos $d(x)$. La linealidad en este contexto se demuestra por las propiedades de las integrales, que mantienen la superposición y el escalado.

## Resumen de las Principales Diferencias

- **Naturaleza de los Datos**:
  - Discreto: Puntos de datos finitos.
  - Continuo: Puntos de datos infinitos representados como funciones.

- **Representación Matemática**:
  - Discreto: Ecuaciones algebraicas lineales.
  - Continuo: Ecuaciones integrales.

- **Técnicas de Solución**:
  - Los sistemas discretos a menudo utilizan operaciones matriciales.
  - Los sistemas continuos pueden requerir métodos numéricos para aproximaciones integrales.


:::{tip}
Estas distinciones resaltan cómo diferentes marcos matemáticos se emplean dependiendo de si el problema involucra observaciones discretas o fenómenos continuos.
:::
