# Juego de Roles en Chatbots

<style>
  .figure {
    text-align: center;
  }
  .figure .caption {
    text-align: center;
  }
</style>

<div class="justificar-texto">

## Introducción al Juego de Roles en Chatbots

Un aspecto importante que discutir al hablar del desarrollo de chatbots son los prompts de juego de roles. Veamos qué son estos. Los prompts de juego de roles indican al chatbot que juegue un papel específico al responder a las preguntas de los usuarios. Imagina el chatbot como un actor en una obra; un prompt de juego de roles es como darle al actor un personaje para interpretar. Así como el actor se sumerge en la mentalidad, personalidad y contexto del personaje que está interpretando, el chatbot adopta un enfoque similar ajustando su tono, vocabulario y comportamiento para cumplir con los requisitos del rol. Esto significa que el chatbot adapta su lenguaje y contenido para ajustarse a la persona en lugar de proporcionar respuestas genéricas. El juego de roles garantiza interacciones más efectivas, especialmente en chatbots específicos de dominio como salud, fitness, educación y finanzas. Nótese que el chatbot aprende a interpretar estos roles basándose en sus datos de entrenamiento.


## Ejemplo Simbólico de Juego de Roles

Primero pasaremos por un ejemplo simbólico para comprender mejor los prompts de juego de roles y luego aprenderemos cómo implementarlos. Imagina que estamos desarrollando un chatbot para una empresa que ofrece productos técnicos complejos. Un cliente pregunta sobre las especificaciones técnicas de un producto determinado. Hemos definido 3 roles para el chatbot: agente de soporte al cliente, gerente de producto e ingeniero de ventas. ¿Cómo respondería cada uno de estos roles? El agente de soporte al cliente proporciona una guía general, dirige a los clientes al sitio web para obtener más detalles y ofrece asistencia. El gerente de producto destaca los beneficios estratégicos, enfocándose en cómo el producto se alinea con los objetivos y necesidades profesionales. El ingeniero de ventas profundiza en los detalles técnicos, discutiendo detalles del procesador, características y seguridad. De este ejemplo podemos ver cómo el rol de un chatbot puede afectar cómo responde.


## Implementación del Juego de Roles

Ahora que entendemos qué son los prompts de juego de roles, es hora de aprender cómo implementarlos. Debemos decirle al modelo que actúe como un rol específico, sin importar cuál sea ese rol. Por ejemplo, podemos pedirle al modelo que actúe como un analista financiero experto y luego pedirle que ofrezca ideas sobre la planificación de la jubilación para personas que se acercan a la edad de jubilación. Vemos cómo la respuesta se moldea como si un verdadero experto en análisis financiero la proporcionara, destacando varias consideraciones a tener en cuenta al planificar su jubilación. Los prompts de juego de roles implican más que solo asignar un rol. Encierran requisitos específicos dentro de ese rol. Por ejemplo, aunque dos periodistas pueden compartir puntos en común, son diferentes. Es por eso que, además del rol mismo, es esencial incorporar rasgos como personalidad y experiencia. Por ejemplo, podemos instruir al chatbot para que encarne la persona de un periodista de tecnología especializado en una investigación y análisis exhaustivos de la industria tecnológica. Luego podemos preguntar sobre el impacto de la IA en el mercado laboral (Figura \@ref(fig:CURSO-64)).  


<div class="figure" style="text-align: center">
<img src="FIG64.jpg" alt="Ejemplo del uso de juego de roles." width="60%" />
<p class="caption">(\#fig:CURSO-64)Ejemplo del uso de juego de roles.</p>
</div>

Aquí podemos ver cómo el modelo responde como un periodista adecuado, ya que formateó la respuesta como un artículo. Además, proporcionó un análisis detallado del tema.




<div style="text-align: center;">
<h3 style="font-weight: bold; text-align: center;">Video Tutorial: Implementación del Juego de Roles</h3>
  <iframe width="500" height="400" src="https://www.youtube-nocookie.com/embed/MHhwIsrZz5o?rel=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>




## Combinación de Juego de Roles y Directrices

Como nota final, debemos tener en cuenta que el juego de roles no elimina la necesidad de especificar otros requisitos como las pautas de comportamiento o de respuesta. Por ejemplo, en el escenario del chatbot periodista, si queríamos que manejara exclusivamente preguntas relacionadas con la tecnología. Modificamos el prompt para probar esta condición y dejar que muestre un mensaje apropiado si no se cumple. Si un usuario pregunta sobre un tema como la literatura catalana, el chatbot aclarará su especialización en tecnología. (Figura \@ref(fig:CURSO-65)).


<div class="figure" style="text-align: center">
<img src="FIG65.jpg" alt="Ejemplo del uso de juego de roles añadiendo más requerimientos." width="60%" />
<p class="caption">(\#fig:CURSO-65)Ejemplo del uso de juego de roles añadiendo más requerimientos.</p>
</div>



<div style="text-align: center;">
<h3 style="font-weight: bold; text-align: center;">Video Tutorial: Combinación de Juego de Roles y Directrices</h3>
  <iframe width="500" height="400" src="https://www.youtube-nocookie.com/embed/MqdMYAyWr2Q?rel=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>


</div>

