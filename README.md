# proyecto_2.2

Instrucción:
Huggingface Api
Proyecto 1 : Utilizando un api de hugginface de un modelo llm crea una aplicación donde el usuario pueda realizar preguntas y el modelo le responda, en el readme especifica el modelo usado y los parámetros en la petición junto con un ejemplo de uso.

## Resumen del proyecto parte 2.

Este proyecto implementa una aplicación de chatbot que utiliza un modelo de lenguaje (LLM) de Hugging Face, específicamente GPT-2, para responder preguntas en tiempo real. El modelo está entrenado en inglés, pero también puede generar respuestas en otros idiomas, como el español, aunque con menor precisión.

## Requisitos para la Ejecución.

1. Python 3.6 o superior.
2. Pip para la instalación de dependencias.
3. Bibliotecas necesarias:

   - `transformers: para interactuar con los modelos de Hugging Face`
   - `torch: para la ejecución de los modelos.`
   - `requests: para enviar peticiones HTTP si se decide utilizar la API de Hugging Face`
   - `comando:`
  
      ```bash
      pip install transformers torch requests

## Requisitos para la Ejecución.
1. Clonar el proyecto con el siguiente comando.
2. Instalar dependencias: Ejecuta el siguiente comando en tu terminal para instalar las dependencias necesarias:
3. Ejecutar la aplicación: Para iniciar la aplicación de chatbot, ejecuta:
4. Salir de la aplicación: Si deseas salir de la aplicación, simplemente escribe salir y presiona Enter.

## Ejemplos de Ejecución.

1. Al ejecutar el script, verás una interfaz de línea de comandos donde puedes escribir tus preguntas. Ejemplo de ejecución:
  
   ![u7](https://github.com/user-attachments/assets/cacdc693-78eb-46de-b3c5-ee81989569fc)
   
# Modelo USADO.

## GPT-2

El modelo utilizado en este proyecto es GPT-2 de Hugging Face, que es un modelo de lenguaje autoregresivo basado en la arquitectura de transformadores. Este modelo ha sido entrenado con grandes cantidades de texto en inglés y es capaz de generar texto coherente y relevante a partir de un prompt dado.

#### Parámetros utilizados en la generación:

1. max_length: 150 caracteres máximo en la respuesta.
2. num_return_sequences: 1 secuencia de respuesta generada.
3. temperature: 0.6 (ajuste para respuestas más coherentes).
4. top_k: 10 (limitación del top-k para mejorar la coherencia de las respuestas).
5. top_p: 0.9 (probabilidad acumulada para la diversidad).
6. no_repeat_ngram_size: 2 (previene la repetición de n-gramas).
7. do_sample: True (habilita el muestreo para generar respuestas más diversas).
