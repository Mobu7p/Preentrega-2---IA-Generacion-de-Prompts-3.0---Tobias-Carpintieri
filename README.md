1. Introducción
El problema que este proyecto busca resolver es la dificultad que muchas personas enfrentan al momento de decidir qué cocinar con los ingredientes que tienen disponibles en su casa. Esto se convierte en una problemática relevante porque genera pérdida de tiempo, provoca desperdicio de alimentos y afecta la economía doméstica al no aprovechar lo que ya está disponible.

La solución propuesta es un asistente virtual que genere recetas personalizadas a partir de los ingredientes que el usuario tenga en su casa. El proyecto se apoya en modelos de lenguaje como Gemini, que permiten crear recetas coherentes y detalladas a partir de simples indicaciones escritas.

La viabilidad del proyecto es alta. Es técnicamente posible gracias a los modelos de lenguaje actuales y los recursos necesarios son mínimos (solo conexión a internet y el acceso gratuito a Gemini). El tiempo de desarrollo es rápido, ya que se enfoca en la creación y optimización de prompts.

2. Objetivos
Objetivo principal: Desarrollar un prototipo funcional de un asistente de recetas que genere sugerencias a partir de ingredientes dados por el usuario, optimizando el aprovechamiento de alimentos.

Objetivos específicos:

Diseñar y optimizar prompts efectivos para que el modelo de IA genere recetas coherentes y detalladas.

Implementar un script que se conecte a una API de IA para procesar las peticiones del usuario.

Optimizar la lógica del código para minimizar las consultas a la API y asegurar la rentabilidad del proyecto.

Evaluar la calidad y la utilidad de las recetas generadas por el asistente.

3. Metodología
 El proyecto se llevará a cabo a través de una metodología iterativa y de desarrollo ágil, centrada en la experimentación y la optimización de los prompts.

Diseño de prompts: Se crearán prompts base para los diferentes escenarios (receta única, menú semanal, etc.). Se probarán con un modelo de lenguaje para evaluar la calidad de las respuestas.

Iteración y refinamiento: Se analizarán las respuestas del modelo y se ajustará el prompt (por ejemplo, añadiendo instrucciones sobre el formato o el tono) hasta obtener el resultado deseado.

Desarrollo del código: Se escribirá un script en Python que gestione la interacción con la API. Este código será modular y bien indentado para facilitar su lectura y mantenimiento.

Optimización: Se implementarán estrategias para reducir las consultas a la API, como el almacenamiento en caché de respuestas frecuentes o la consolidación de peticiones.

Evaluación: Se realizarán pruebas para verificar que el asistente sea útil y las recetas sean viables.

4. Herramientas y tecnologías
Modelo de Lenguaje: Gemini.

Lenguaje de programación: Python.

Librerías: google.generativeai y os.

Técnicas de Prompting:

Instruction prompting: Se darán instrucciones claras y directas al modelo sobre lo que se espera.

Few-shot prompting: Se utilizará para incluir ejemplos que guíen al modelo a generar respuestas en un formato específico.

Chain of Thought (CoT): Se le pedirá al modelo que "piense" y justifique sus pasos, para asegurar que la receta sea lógica y coherente.
