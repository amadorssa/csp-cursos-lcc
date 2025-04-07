# Constraint Satisfaction Problem (CSP)

## Modelo simplificado
### Variables

Sea $X$ el conjunto de variables, donde cada variable $x_i$ representa un curso.

$X = \{ x_1, x_2, ..., x_n \}$

Por ejemplo:
- $x_1 = Inteligencia \ Artificial$
- $x_2 = Algoritmos$
- $x_3 = Estructura\ de\ Datos$
- $x_4 = Programación\ Avanzada$

### Dominio
Sea $A$ el conjunto de aulas, $H$ el conjunto de horas.

El dominio de cada variable $x_i$ es el conjunto de pares $(a,h)$, donde $a$ es un aula y $h$ es una hora.

$D(x_i) = A \times H$
Por ejemplo:
- $D(x_1) = \{ (A1, 8), (A1, 9), (A2, 8), (A2, 9) \}$
- $D(x_2) = \{ (A1, 8), (A1, 9), (A2, 8), (A2, 9) \}$


### Restricciones

Definiremos $C$ como el conjunto de restricciones.

#### Modelo simplificado:
- Cada curso tiene una duración de una hora.
- Todas las aulas son iguales.
- Un curso solo puede ser impartido por un profesor.
- Un curso se imparte todos los días a la misma hora.


**Dos cursos no pueden ser impartidos en la misma aula a la misma hora.**
$$\forall x_i, x_j \in X, i \neq j: \quad x_i \neq x_j$$


### Modelo completo:

Para extender el modelo consideraremos ademas, los siguientes elementos:
- $P$: conjunto de profesores.

