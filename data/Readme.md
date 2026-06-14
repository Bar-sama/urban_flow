
## Sprint 3 - Conclusión

En este sprint se perfeccionó la solución incorporando persistencia
relacional con SQLAlchemy y busqueda semántica con ChromaDB y OpenCLIP.
Además, se implementó un sistema de control de versiones de datos para
gestionar de manera eficiente los archivos grandes y asegurar la trazabilidad
y la integridad de los datos.
El modelo relacional (Vehículo, Radar, Multa, Evidencia) permitiÓ migrar
los datos del CSV a una base SQLite manteniendo las relaciones entre
entidades y facilitando consultas agregadas como: top patentes, radares activos,
reincidentes por periodo y porcentaje de evidencia visual.
La integración con la base vectorial habilitó busquedas por similitud de
imagen: dada una foto de patente fue posible recuperar todos los datos del vehículo
más cercano sin necesidad de OCR, lo que mejoró robustéz ante imágenes de
baja calidad o no tan nítidas.
