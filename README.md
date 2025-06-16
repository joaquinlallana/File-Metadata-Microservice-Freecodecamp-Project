# File Metadata Microservice

Este es un proyecto de microservicio para analizar metadatos de archivos, desarrollado como parte de los proyectos de APIs y Microservicios de freeCodeCamp.

## Descripción

La aplicación permite a los usuarios subir un archivo y recibir como respuesta un objeto JSON con el nombre, tipo y tamaño (en bytes) del archivo subido.

## Uso

1. Abre la aplicación en tu navegador.
2. Selecciona un archivo usando el formulario.
3. Haz clic en "Upload".
4. Recibirás una respuesta JSON con los metadatos del archivo:

```json
{
  "name": "nombre_del_archivo.ext",
  "type": "tipo/mime",
  "size": 12345
}
```

## Instalación

1. Clona este repositorio:
   ```bash
   git clone <url-del-repositorio>
   cd boilerplate-project-filemetadata
   ```
2. Instala las dependencias:
   ```bash
   npm install
   ```
3. Inicia el servidor:
   ```bash
   npm start
   ```
4. Abre [http://localhost:3000](http://localhost:3000) en tu navegador.

## Endpoints

- `POST /api/fileanalyse`  
  Envía un archivo en el campo `upfile` del formulario.  
  Responde con un JSON que contiene el nombre, tipo y tamaño del archivo.

## Tecnologías utilizadas

- Node.js
- Express
- Multer
- freeCodeCamp boilerplate

## Estructura del proyecto

```
/routes/api.js        # Lógica de la API y manejo de archivos
/views/index.html     # Página principal con el formulario
/public/              # Archivos estáticos (CSS, imágenes, etc.)
index.js              # Archivo principal del servidor
```

## Créditos

Proyecto basado en el boilerplate de freeCodeCamp.

---
