---
layout: distill
title: Rates of Change
description: Brief notes about Rates of change.
date: 2021-05-22

authors:
  - name: Camilo E. Davila
    url: "https://en.wikipedia.org/wiki/Albert_Einstein"
    affiliations:
      name: IAS, Princeton

bibliography: 2018-12-22-distill.bib

# Optionally, you can add a table of contents to your post.
# NOTES:
#   - make sure that TOC names match the actual section names
#     for hyperlinks within the post to work correctly.
#   - we may want to automate TOC generation in the future using
#     jekyll-toc plugin (https://github.com/toshimaru/jekyll-toc).
toc:
  - name: What is a Rate of change?
  - name: Example 1
    # if a section has subsections, you can add them as follows:
    # subsections:
    #   - name: Example Child Subsection 1
    #   - name: Example Child Subsection 2
---

## What is a Rate of change?

#### Nota general

- Razon de cambio = derivada.

#### Conceptualizacion

La estrategia consiste en encontrar una relacion matematica en donde se relacionen las funciones
que aparezcan en el contexto del problema.

Posteriormente se deriva la expresion matematica mencionada y se obtiene una relacion de funciones y razones de cambio (las que se conocen con las que no se conocen).

Por ultimo se despeja la razon de cambio deseada que estara en terminos de las otras razones de cambio.

**Nota:** En este tipo de problemas es de vital importancia tener muy claro, _que es lo que se pide en el problema?_ asi como, _que es lo que se sabe en el problema_. Teniendo claro lo que se pide y lo que se ssabe, procedemos a matematizar el problema.

## Example 1

#### Enunciado

Al arrojar una piedra a un estanque de agua tranquila se forman ondas circulares concentricas cuyos radios aumentan de longirud al paso del tiempo. Cuando la onda exterior tiene un radio de 3 $$ m $$, este aumenta a una rapidez (velocidad) de $$ 50 cm/s $$. A que rapidez (velocidad) aumenta el area del circulo formado por dicha onda?

- **Que se pide en el problema?:**

Se pide calcular la rapidez (velocidad) a la que esta aumentando el area de un circulo, cuando su radio mide 3 $$ m $$ y la longitud de este aumenta a razon de $$ 0.5 m/s $$. Es decir, si consideramos un circulo que (en cierto instante $$ t $$) tiene un radio $$ r(t) $$ y un area $$ A(t) $$, entonces lo que se desea es calcular la velocidad con que cambia (razon de cambio) el area $$ A(t) $$, cuando el radio $$ r(t) $$ es de $$ 3 m $$ y la razon de cambio del radio es de $$ 0.5 m/s $$. Esto es, se pide calcular la derivada $$ \frac{dA}{dt} $$ cuando $$ r = 3 $$ y cuando $$ \frac{dr}{dt} = 0.5 $$.

El area del circulo es $$ A = \pi\ r^2 $$. La razon de cambio de $$ A $$ con respecto al tiempo de $$ t $$ se obtiene derivando ambos miembros con respecto al tiempo:

$$
\frac{dA}{dt} = \frac{d}{dt}\left[\pi\ r^2(t)\right] = 2\pi\ r(t) \left(\frac{dr}{dt} \right)
$$

En el caso particular en que $$ r(t) = 3m $$ y $$ \frac{dr}{dt} = 0.5 m/s $$:

$$
\frac{dA}{dt} = 2\pi\ r(t) \left(\frac{dr}{dt} \right) = 2\pi\ (3m)(0.5 m/s) = 3\pi\ m^2/s \Rightarrow \frac{dA}{dt} = 3\pi\ m^2/s \approx 9.4248 m^2/s
$$

Esto es, en el preciso instante en que el radio es de $$ 3m $$, este tiene un cambio de $$ 0.5 m/s $$ y el area tiene un cambio de  $$ 3\pi\ m^2/s \approx 9.4248 m^2/s $$.
