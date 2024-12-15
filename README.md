# ScreanMatch-API
Implementacion de peliculas steaming usando API


# 📽️ Página de Películas en Streaming - Java App

Este proyecto es una aplicación en Java que genera una página de películas en streaming al consumir datos de una **API de películas**. La aplicación maneja errores durante la ejecución y genera archivos con información relevante de las películas. El objetivo del proyecto es demostrar el uso de APIs, manejo de excepciones y escritura de archivos en Java.

## 🚀 Características

1. **Consumo de API**:
   - Recupera información actualizada sobre películas desde una API pública de películas en streaming.
   - Procesa y extrae datos como el título, la descripción, el género y la calificación.

2. **Manejo de Errores**:
   - Implementa una gestión robusta de errores para capturar problemas como:
     - Conexiones fallidas a la API.
     - Datos faltantes o mal formateados.
     - Problemas al escribir archivos.

3. **Generación de Archivos**:
   - Escribe los datos recuperados en un archivo `.txt` o `.html` para fácil visualización y almacenamiento.
   - Incluye opciones para personalizar el formato del archivo generado.

## 📂 Estructura del Proyecto

```plaintext
.
├── src
│   ├── Main.java         # Clase principal
│   ├── ApiClient.java    # Clase para consumir la API
│   ├── Movie.java        # Modelo para representar las películas
│   ├── FileWriter.java   # Clase para manejar la escritura de archivos
│   └── ErrorHandler.java # Clase para manejar errores
├── README.md             # Documentación del proyecto
├── movies-output.txt     # Archivo de salida con la información de películas
└── resources
    └── config.properties # Configuración (API Keys, URLs, etc.)
```

## 🛠️ Tecnologías Utilizadas

- **Lenguaje**: Java
- **HTTP Client**: `HttpURLConnection` (o bibliotecas como `OkHttp` o `HttpClient` de Apache)
- **Gestión de JSON**: `Gson` o `Jackson` para procesar la respuesta de la API
- **Manejo de Errores**: Bloques `try-catch`
- **Escritura de Archivos**: `BufferedWriter` y `FileWriter`

## 🔧 Configuración

1. Clona este repositorio:
   ```bash
   git clone https://github.com/tuusuario/pagina-peliculas-streaming.git
   cd pagina-peliculas-streaming
   ```

2. Configura la API en el archivo `resources/config.properties`:
   ```properties
   API_URL=https://api.example.com/movies
   API_KEY=tu_clave_api
   ```

3. Asegúrate de tener una conexión a Internet para consumir la API.

4. Compila el proyecto:
   ```bash
   javac src/*.java
   ```

5. Ejecuta el programa:
   ```bash
   java -cp src Main
   ```

## 📝 Uso

1. **Ejecutar la Aplicación**:
   Al ejecutar el programa, este:
   - Se conecta a la API configurada en `config.properties`.
   - Recupera una lista de películas con sus detalles.
   - Muestra las películas en la consola y las escribe en un archivo de salida.

2. **Archivo Generado**:
   - El archivo de salida `movies-output.txt` se generará automáticamente en el directorio raíz del proyecto.

3. **Ejemplo de Archivo Generado**:
   ```plaintext
   Título: Inception
   Género: Ciencia Ficción
   Calificación: 8.8
   Descripción: Un ladrón que roba secretos corporativos utilizando tecnología de sueños...
   ```

## 🎯 Funcionalidades Futuras

- Agregar soporte para varias APIs de películas.
- Crear una interfaz gráfica con JavaFX.
- Añadir opciones de filtrado por género, calificación, o año de estreno.
- Generar archivos en formatos adicionales como PDF o JSON.

## 🐞 Manejo de Errores

El programa captura y gestiona varios tipos de errores:
- **Errores de red**: Falla al conectar a la API.
- **Errores de datos**: Datos mal formateados o faltantes en la respuesta de la API.
- **Errores de archivos**: Problemas al crear o escribir en el archivo de salida.

## 📚 Recursos y Aprendizajes

Este proyecto me permitió:
- Aprender a consumir y procesar APIs REST con Java.
- Mejorar mi manejo de excepciones y depuración de errores.
- Practicar la escritura de archivos y la manipulación de datos estructurados.

## 👏 Agradecimientos

A las comunidades de programación y a los recursos en línea que me ayudaron a entender APIs, manejo de excepciones y buenas prácticas en Java.

## 🏷️ Etiquetas

`#Java` `#API` `#Backend` `#Desarrollo` `#Proyectos`

