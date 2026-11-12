# sprint7-final-project
# Análisis ConnectaTel — Sprint 7
## 🎯 Objetivo del proyecto
Integrar, limpiar y analizar los datos de clientes de ConnectaTel, para identificar patrones de uso de llamadas y mensajes, detectar valores atípicos, crear segmentaciones de clientes y extraer insights comerciales accionables.

## 📂 Datasets utilizados
Se trabajó con tres conjuntos de datos:
- **Clientes / user_profile**: Datos demográficos: identificador de usuario, nombre, edad, ciudad, fecha de deserción.
- **Uso de servicios**: Registros de cantidad de llamadas, mensajes y minutos de llamada por cliente.
- **Planes**: Información del plan contratado por cada usuario.

## 📌 Etapas del análisis
1. **Integración y carga**: Importación de las tres fuentes y unión en un solo dataframe.
2. **Limpieza y validación**: Estandarización de tipos de datos, detección y corrección de valores centinela, nulos e inconsistencias como edades imposibles o cantidades negativas.
3. **Perfil estadístico**: Cálculo de métricas de uso por cliente y por segmentos demográficos.
4. **Detección de outliers**: Aplicación del método IQR y visualización con boxplots para identificar comportamientos atípicos.
5. **Segmentación de clientes**: Creación de grupos por rango de edad, plan contratado y nivel de uso (`grupo_uso`: bajo, medio y alto uso).
6. **Visualización e insights**: Comparación de segmentos, cálculo de distribuciones porcentuales y elaboración de recomendaciones comerciales.

## ▶️ Cómo ejecutar el notebook
### Opción 1: Google Colab
1. Sube los archivos `.csv` y el notebook al repositorio.
2. Abre el archivo `spring-final-proyect.ipynb` desde Colab.
3. Modifica las rutas de carga de los archivos si es necesario.
4. Ejecuta las celdas en orden.

### Opción 2: Entorno local
1. Clona el repositorio en tu computadora.
2. Instala las librerías necesarias:
   ```bash
   pip install pandas numpy matplotlib seaborn
