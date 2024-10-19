# resumen-archivos-drive

## Carpetas Locales Propuestas
1. /project_root/: Carpeta raíz del proyecto.
2. /project_root/scripts/: Carpeta donde se almacenan los scripts de Python. Busca separar los códigos por funcionalidades y mantener todo ordenado.
3. /project_root/downloads/: Carpeta donde se descargarán los archivos desde Google Drive.
4. /project_root/summaries/: Carpeta donde se guardarán los archivos con los resúmenes generados.
5. /project_root/logs/: Carpeta destinada a guardar los archivos de logs del proceso.

## Archivos Clave
1. /project_root/main.py: archivo principal que integra todo el flujo de automatización. Contiene la importación de todos los módulos y scripts, así como la ejecución de la secuencia completa.
2. /project_root/scripts/drive_monitor.py: script encargado de la integración con Google Drive, usando la API de Google. Detecta nuevos archivos y los descarga en /downloads/.
3. /project_root/scripts/AI_interaction.py: script que maneja la interacción con la IA usando Selenium. Incluye desde que se abre el navegador hasta que se tiene la respuesta, pasando por la autenticación y la consulta.
4. /project_root/scripts/file_manager.py: script encargado de manejar archivos locales, incluyendo el guardado de resúmenes en la carpeta /summaries/. Se encarga de crear, escribir y mover los archivos de texto con los resúmmenes, nombrándolos de forma clara y cronológica.
5. /project_root/scripts/utils.py: script con funciones utilitarias comunes a todo el proyecto, como manejo de errores o generación de logs.
6. /project_root/config.yaml: archivo de configuración donde se almacenan detalles importantes, como la carpeta de Google Drive a monitorear, las rutas locales para guardado de archivos, credenciales, etc.
7. /project_root/requirements.txt: archivo que lista las dependencias necesarias para el proyecto (como Selenium, Google API, etc.). Sirve para instalar todo con pip.
8. /project_root/logs/error_log.txt: archivo de logs donde se registrarán errores o eventos importantes del sistema.

## Nomenclatura de Archivos Generados Automáticamente

### Archivos Descargados (de Google Drive)
- Formato: nombre_original.ext
- Ejemplo: documento_importante.pdf.
- Descripción: Mantener el nombre original del archivo para facilitar la identificación del contenido.

### Resúmenes Generados por IA
- Formato: resumen_nombre_original_fecha.txt
- Ejemplo: resumen_documento_importante_2024-10-18.txt.
- Descripción: Los resúmenes incluirán el nombre del archivo original y la fecha en que se generó el resumen.
