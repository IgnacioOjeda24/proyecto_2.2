# proyecto_2.2

Instrucción:
Huggingface Api
Proyecto 1 : Utilizando un api de hugginface de un modelo LLM crea una aplicación donde el usuario pueda realizar preguntas y el modelo le responda, en el readme especifica el modelo usado y los parámetros en la petición junto con un ejemplo de uso.

## Resumen del proyecto parte 2.

Este proyecto implementa una aplicación de chatbot, que el usuario haga cualquier pregunta con el modelo LLM que se llama openai-community/gpt2, responde de manera no exacta, pero funciona el código. Lo ideal que se haga preguntas en inglés, ya que tiene respuestas con más precisión respecto a los demás idiomas.

## Requisitos para la Ejecución.

1. **Python 3.8 a 3.10 independiente del sistema operativo que tenga el usuario como: Windows, Linux o Mac**.
2. **Visual studio instalado independiente del sistema operativo que tenga el usuario como: Windows, Linux o Mac.**
3. **Instalar el siguiente comando**
   
   ```bash
   pip install transformers torch requests

4. **Librerías instaladas en python**

   - `transformers: para interactuar con los modelos de Hugging Face`
   - `torch: para la ejecución de los modelos.`
   - `requests: para enviar peticiones HTTP si se decide utilizar la API de Hugging Face`

5. **Librerías importadas en foto**

   ![U20](https://github.com/user-attachments/assets/1de1414b-b5be-4c7b-89e6-8ce169a6f6e2)

6. **Antes de correr el programa, instalar los siguientes comandos:**

   Para crear el entorno virtual en visual studio code.

   ``` bash
   python -m venv nombre_propio_de_entorno virtual

   Ejemplo:

   ``` bash
   python -m venv env2

   Para activar el entorno virtual en visual studio code.

   ``` bash
   \nombre_propio_de_entorno virtual\Scripts\activate

   Ejemplo:

   ``` bash
   \env2\Scripts\activate


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
