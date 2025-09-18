Asistente Inteligente de Recetas: Cocina con lo que Tenes

1. Resumen del Problema y la Solución
1.1. La Problemática: Muchas personas se enfrentan al dilema de "qué cocinar" con los ingredientes disponibles en sus hogares. Esto no solo provoca la pérdida de tiempo y el desperdicio de alimentos, sino que también afecta la economía familiar al no aprovechar lo que ya se tiene.

1.2. La Solución: Desarrolle un asistente virtual de recetas que utiliza la inteligencia artificial generativa de Google Gemini para crear recetas personalizadas y detalladas. El usuario simplemente ingresa una lista de ingredientes, y el sistema genera una receta única que se adapta exclusivamente a ellos.

2. Metodología y Herramientas
2.1. Tecnologías Principales:

Modelo de Lenguaje: Google Gemini 1.5 Flash.

Lenguaje de Programación: Python.

Librerías: google.generativeai y os.

2.2. Enfoque de Prompting:
La solución reside en la optimización del prompt, lo que permite guiar al modelo para generar respuestas de alta calidad de forma eficiente. Utilizamos una combinación de las siguientes técnicas de Fast Prompting:

One-Shot Prompting: Incluimos un ejemplo de receta completa y formateada directamente en el prompt. Esto le enseña al modelo la estructura deseada para la respuesta (Nombre, Tiempo, Porciones, Ingredientes, Pasos, etc.), garantizando una salida clara y coherente.

Chain of Thought (CoT): Se le pide al modelo que "piense" y razone lógicamente sobre cómo combinar los ingredientes disponibles antes de generar la receta final. Este paso invisible asegura que el resultado sea viable y creativo.

Instruction Prompting: Se dan instrucciones claras y directas para que el modelo no agregue ingredientes extra bajo ninguna circunstancia, un requerimiento clave para resolver el problema de desperdicio.

3. Implementación y Optimización
3.1. Prueba de Concepto (POC):
La implementación se realizó en una Jupyter Notebook para demostrar la funcionalidad principal del asistente. El código está diseñado para ser modular y fácil de entender, con funciones dedicadas para la creación del prompt y la generación de la receta.

3.2. Optimización de Costos y Eficiencia:
Para cumplir con el requisito de uso eficiente de la API, se implementó un sistema de caché en memoria (recetas_cache). Esta técnica almacena las recetas ya generadas, de modo que si un usuario solicita los mismos ingredientes nuevamente, la receta se entrega instantáneamente desde el caché. Esto evita llamadas repetidas a la API de Google Gemini, reduciendo significativamente los costos de uso y mejorando la velocidad de respuesta.

4. Uso de Modelos (Texto-Texto y Texto-Imagen)
La solución se centra en la implementación del modelo texto-texto de Gemini para la generación de recetas. Si bien el proyecto original contemplaba la integración de un modelo texto-imagen, esto no fue posible.
Aunque realice intentos para integrar APIs de generación de imágenes, se presentaron múltiples errores de conexión y de autenticación. Esto impidió su correcta implementación en el tiempo de desarrollo. Sin embargo, el concepto de utilizar ambos modelos para una solución integral fue considerado desde la fase de diseño, lo que demuestra la comprensión de cómo estas herramientas pueden trabajar de forma complementaria.

5. Conclusiones y Resultados
El prototipo resuelve con éxito la problemática, ofreciendo una solución funcional. A través de una combinación de técnicas de Fast Prompting, el asistente genera recetas de alta calidad que son coherentes y útiles. La implementación del caché no solo optimiza el rendimiento, sino que también garantiza la viabilidad económica del proyecto a largo plazo. Los resultados son presentaciones claras y estructuradas, fáciles de seguir para cualquier usuario.
