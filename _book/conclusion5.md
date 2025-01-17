# Prompting de Cadena de Pensamiento

<style>
  .figure {
    text-align: center;
  }
  .figure .caption {
    text-align: center;
  }
</style>

<div class="justificar-texto">

## Introducción al Prompting de Cadena de Pensamiento

El prompting de cadena de pensamiento es una técnica que requiere que los modelos de lenguaje presenten una serie de pasos de razonamiento referidos como pensamientos antes de proporcionar una respuesta final. En otras palabras, los modelos de lenguaje deben explicar cómo llegaron a una conclusión. Esta técnica es particularmente valiosa al tratar tareas de razonamiento complejo. Además, ayuda a reducir errores del modelo ya que el razonamiento ocurre paso a paso.

## Ejemplo de Uso del Prompting de Cadena de Pensamiento

Para entender el poder de los prompts de cadena de pensamiento, comparemoslos con los prompts estándar usando un problema matemático. Supongamos que queremos determinar cuántos libros tiene una persona, dados su número existente de libros y sus decisiones de préstamo y compra. Si pedimos al modelo que muestre la respuesta, nos dará un número. Sin embargo, no podemos estar seguros de su corrección sin saber cómo se generó este número. Para tratar esto, usamos un prompt de cadena de pensamiento pidiendo al modelo que proporcione esta explicación paso a paso. Ahora el modelo resuelve el problema un paso a la vez antes de dar la respuesta final. Desglosando la solución en cinco pasos. En la Figura \@ref(fig:CURSO-35) se pueden ver todos los pasos y no solo la solución con lo cual estamos seguros de que la respuesta es correcta.


<div class="figure" style="text-align: center">
<img src="FIG35.jpg" alt="Ejemplo de prompting de varios pasos." width="60%" />
<p class="caption">(\#fig:CURSO-35)Ejemplo de prompting de varios pasos.</p>
</div>

## Uso de Prompting de Varios Disparos para Cadena de Pensamiento


Podemos usar prompts de varios disparos para obtener razonamientos de cadena de pensamiento. En lugar de instruir explícitamente al modelo para que genere pasos de razonamiento, proporcionamos ejemplos de lo que deben contener las respuestas. Por ejemplo, consideremos la tarea de evaluar si un grupo de números impares suma un número par. Proporcionamos una pregunta y respuesta de ejemplo para el modelo. La respuesta aclara los pasos requeridos, encontrando los números impares y luego sumándolos para determinar si la afirmación es verdadera o falsa. Luego proporcionamos una nueva pregunta y dejamos una A para que el modelo responda. Combinamos el ejemplo y la pregunta para obtener el prompt final. Como podemos ver, el modelo sigue una lógica similar para generar su respuesta. Ver Figura \@ref(fig:CURSO-36).

<div class="figure" style="text-align: center">
<img src="FIG36.jpg" alt="Ejemplo de prompting Varios Disparos para Cadena de Pensamiento." width="60%" />
<p class="caption">(\#fig:CURSO-36)Ejemplo de prompting Varios Disparos para Cadena de Pensamiento.</p>
</div>

## Diferencias entre Prompting de Varios Pasos y Cadena de Pensamiento

Estudiemos la diferencia entre los prompts de varios pasos y los prompts de cadena de pensamiento. Con los prompts de varios pasos, los diversos pasos de la tarea están directamente incorporados en el prompt mismo, guiando el comportamiento del LLM. Los prompts de cadena de pensamiento adoptan un enfoque diferente al instruir al modelo para que genere pasos intermedios o pensamientos en su salida mientras resuelve el problema. Esto ayuda a obtener información sobre la toma de decisiones del modelo. Una limitación del prompting de cadena de pensamiento es que un pensamiento con razonamiento defectuoso llevará a un resultado fallido.



<div style="text-align: center;">
<h3 style="font-weight: bold; text-align: center;">Video Tutorial: Prompting de cadena de pensamiento</h3>
  <iframe width="500" height="400" src="https://www.youtube-nocookie.com/embed/0Ay0bKDG3Jk?rel=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

</div>

