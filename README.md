# Womby

## Deploy URL
[Página de deploy](englishbot.streamlit.app)

## How to run it on your own machine

1. Install the requirements

   ```
   $ pip install -r requirements.txt
   ```

2. Add the api key on the root project directory in a .env file, in the same way as .env.example

3. Run the app

   ```
   $ streamlit run streamlit_app.py
   ```

## Agregar un nuevo Prompt
Para configurar nuevos Prompt, es necesario crear un archivo de python (.py) con nombre prompt_{nivel de curso de ingles}.py, con el texto del Prompt que se quiere configurar dentro de la variable PROMPT. A su vez el archivo python creado debe estar en la carpeta prompts (/static/prompts). El nombre de archivo de python es usado para configurar el prompt asociado al nivel seleccionado en la aplicación de interfaz de Womby. Para aplicar cambios es necesario hacer reboot de la aplicación desde Streamlit.

## Agregar preguntas, unidades y/o niveles
Para agregar preguntas, unidades y/o niveles de inglés se debe editar el archivo courses_info.json. En este se deben agregar los elementos deseados siguiendo el formato ya establecido en el mismo archivo. Es posible que sea necesario hacer reboot de la aplicación desde Streamlit para que se apliquen los cambios.
