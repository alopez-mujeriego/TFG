# Generación y Explicación de Código

<style>
  .figure {
    text-align: center;
  }
  .figure .caption {
    text-align: center;
  }
</style>

<div class="justificar-texto">

## Introducción a la Generación y Explicación de Código

Las últimas aplicaciones comerciales que cubriremos son la generación y explicación de código. Veamos cómo generar y explicar fragmentos de código con prompts efectivos. La generación de código crea automáticamente código que resuelve un problema dado. Es esencial en cualquier dominio que utilice soluciones de software. Sin embargo, se recomienda precaución al usar LLMS para generar código ya que una comprensión sólida del código generado es esencial para su uso práctico.


## Generación de Código

Para generar código, debemos incluir en el prompt la descripción del problema, el lenguaje de programación objetivo y el formato del código generado, como script, función o clase. Por ejemplo, pedimos al modelo que escriba una función en Python que calcule el promedio de ventas por trimestre dado una lista de ventas trimestrales. El modelo genera una función llamada promedio_ventas_timestrales que recibe una lista de ventas trimestrales. Los elementos de la lista se suman y se dividen por la longitud de la lista para calcular su promedio. Finalmente, se devuelve el promedio de ventas (Figura \@ref(fig:CURSO-57)).


<div class="figure" style="text-align: center">
<img src="FIG57.jpg" alt="Generación de una función en Python dada la especificación por el usuario." width="60%" />
<p class="caption">(\#fig:CURSO-57)Generación de una función en Python dada la especificación por el usuario.</p>
</div>



## Ejemplos de Entrada y Salida para Generación de Programas

En lugar de descripciones explícitas de problemas, a veces tenemos ejemplos de entrada y salida y queremos generar un programa que los mapee. Supongamos que tenemos los siguientes ejemplos de entrada y salida. Sabemos que las entradas son listas de ventas trimestrales de cuatro números cada una, pero necesitamos entender cómo se generan las salidas basadas en estas entradas. Pedimos al modelo que escriba un programa en Python que haga esto. Como podemos ver, el modelo primero establece la conexión entre las entradas y salidas al descubrir que una función de promedio mapeará cada entrada dada a la salida correspondiente. Luego, proporciona la función correspondiente y muestra cómo se aplica a los ejemplos (Figura \@ref(fig:CURSO-58)).


<div class="figure" style="text-align: center">
<img src="FIG58.jpg" alt="Generación de una función en Python dados unos ejemplos." width="60%" />
<p class="caption">(\#fig:CURSO-58)Generación de una función en Python dados unos ejemplos.</p>
</div>



## Modificación de Código Existente

En lugar de pedir al modelo que genere código desde cero, podemos pedirle al modelo que modifique el código según algunos requisitos. Por ejemplo, este script en Python calcula las ventas totales a partir de una lista de ventas trimestrales y imprime la salida. Pedimos al modelo que transforme el script en una función que podamos llamar para calcular las ventas totales. El modelo genera la función solicitada que calcula las ventas totales y el script modificado que la llama en una lista de ventas trimestrales en la Figura \@ref(fig:CURSO-59).  


<div class="figure" style="text-align: center">
<img src="FIG59.jpg" alt="Modificar el script delimitado {} a una función para que se pueda llamar para calcular las ventas totales dadas las ventas trimestrales." width="60%" />
<p class="caption">(\#fig:CURSO-59)Modificar el script delimitado {} a una función para que se pueda llamar para calcular las ventas totales dadas las ventas trimestrales.</p>
</div>

Podríamos incluir múltiples modificaciones en un solo prompt. Usando el mismo script que teníamos, pediríamos al modelo que permita a los usuarios ingresar parámetros de manera interactiva y verificar si son positivos, devolviendo un mensaje de error si no lo son. 


## Explicación de Código

Algunos fragmentos de código pueden volverse muy difíciles de interpretar, especialmente si son largos. Los LLMS pueden usarse para explicar un fragmento de código dado. Al pedir al modelo que explique un código específico, debemos dar orientación sobre nuestras expectativas para la longitud de esta explicación. Por ejemplo, podemos pedir al modelo que explique lo que hace el código en una oración y, en consecuencia, el modelo nos dará una explicación de alto nivel del propósito del código, que calcula el promedio de ventas por trimestre. También podemos pedir al modelo que explique el código en detalle. En este caso, usamos un prompt de cadena de pensamiento pidiendo al modelo que piense paso a paso. Aplicamos este prompt para el mismo código que teníamos anteriormente. El modelo tomará un fragmento de código a la vez y explicará su funcionalidad. Explica en la Figura \@ref(fig:CURSO-60) paso a paso lo que ocurre en cada parte, comenzando con la definición de la función, pasando al cálculo y luego devolviendo el resultado. Finalmente, resume el propósito del código.


<div class="figure" style="text-align: center">
<img src="FIG60.jpg" alt="Explicar el código delimitado entre  {} dado en el Sistema de Prompt." width="60%" />
<p class="caption">(\#fig:CURSO-60)Explicar el código delimitado entre  {} dado en el Sistema de Prompt.</p>
</div>



<div style="text-align: center;">
<h3 style="font-weight: bold; text-align: center;">Video Tutorial: Generación y Explicación de Código</h3>
  <iframe width="500" height="400" src="https://www.youtube-nocookie.com/embed/14ZKE8gMsQ4?rel=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>


</div>

