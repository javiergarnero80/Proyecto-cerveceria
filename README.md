Geocodificación de Cervecerías
Este código en Python se utiliza para geocodificar cervecerías a partir de un archivo CSV que contiene el nombre de la cervecería y la ciudad correspondiente. Utiliza el servicio de geocodificación Nominatim para obtener las coordenadas de latitud y longitud de cada ciudad, así como el estado y el país asociados a esas coordenadas.

Requisitos
Python 3.x
Biblioteca geopy
Archivo CSV con el formato adecuado (nombre de cervecería y ciudad)
Instalación
Asegúrate de tener Python 3.x instalado en tu sistema.
Instala la biblioteca geopy utilizando el administrador de paquetes de Python, pip, ejecutando el siguiente comando:
Copy code
pip install geopy
Descarga el código fuente del repositorio.
Uso
Coloca el archivo CSV que contiene los datos de las cervecerías en la misma ubicación que el archivo geocodificacion_cervecerias.py.
Abre una terminal o línea de comandos en la ubicación donde se encuentra el archivo geocodificacion_cervecerias.py.
Ejecuta el siguiente comando para iniciar el programa:
Copy code
python geocodificacion_cervecerias.py
El programa leerá el archivo CSV, buscará la ubicación de cada ciudad y guardará los resultados en un archivo CSV de salida.
El archivo de salida contendrá el nombre de la cervecería, la ciudad, el estado, el país, la latitud y la longitud.
Personalización
Puedes personalizar el programa modificando las siguientes partes:

User Agent: En las funciones obtener_latitud_longitud y obtener_estado_pais, se utiliza el parámetro user_agent en la inicialización del objeto Nominatim. Puedes cambiar el valor de "tu_app" a un identificador único que te identifique.
Ruta del archivo CSV: En la función main, la variable archivo_csv contiene la ruta del archivo CSV de entrada. Asegúrate de proporcionar la ruta correcta al archivo que contiene los datos de las cervecerías.
Nombre del archivo de salida: En la función main, la variable archivo_resultados contiene el nombre del archivo CSV de salida. Puedes cambiarlo a tu preferencia. El programa generará un nombre de archivo único agregando un número de versión si el archivo ya existe.
