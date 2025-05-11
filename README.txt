
# Proyecto: API Personal tipo WorldTimeAPI

## Descripción
Esta API replica el comportamiento de WorldTimeAPI. Está construida con FastAPI y puede desplegarse en plataformas como Render.com para ser usada desde Power BI.

---

## Archivos proporcionados
- `main.py`: Código principal de la API.
- `requirements.txt`: Dependencias necesarias.
- `start.sh`: Script para iniciar el servidor con Uvicorn.

---

## Instrucciones para desplegar la API

### 1. Subir a GitHub
1. Descomprime `worldtimeapi_clone.zip`
2. Abre una terminal en esa carpeta.
3. Ejecuta:
    git init
    git add .
    git commit -m "Primera versión"
4. Crea un nuevo repositorio en GitHub.
5. Conecta y sube:
    git remote add origin https://github.com/tu_usuario/tu_repositorio.git
    git branch -M main
    git push -u origin main

### 2. Crear el servicio en Render
1. Ve a https://render.com
2. Clic en "New > Web Service"
3. Elige tu repo
4. Configura:
    - Runtime: Python 3
    - Build Command: pip install -r requirements.txt
    - Start Command: ./start.sh
    - Instance type: Free
5. Espera que Render te dé una URL como:
    https://tu-api.onrender.com

---

## Uso desde Power BI

1. Ir a **Inicio > Obtener datos > Web**
2. Pegar URL como:
   https://tu-api.onrender.com/api/time/America/Bogota
3. Transformar datos en el editor de Power Query

---

## Recursos adicionales

Video guía:
https://www.youtube.com/watch?v=nOP8khZhjhk

