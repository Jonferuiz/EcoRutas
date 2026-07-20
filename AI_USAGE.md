# Documentación de Uso de IA Generativa (AI_USAGE)

## Herramientas Utilizadas
* ChatGPT
* Claude

## Registro de Uso Estructurado
* **Archivo afectado:** `routing_algorithm.py`
* **Prompt utilizado:** "Escribe una función en Python usando asyncio y heapq para encontrar la ruta más corta en un diccionario de grafos, priorizando la menor cantidad de paradas."
* **Cambios realizados al output:** Se refactorizaron los nombres de las variables para que coincidan con la nomenclatura general del repositorio (ej. cambiar `node` a `intersection_id`). Se añadió tipado estricto (Type Hints) y docstrings para cumplir con los estándares del equipo.
* **Justificación:** Se utilizó para acelerar la creación del algoritmo base (boilerplate de A*), permitiendo enfocar los recursos de desarrollo en la lógica de cálculo de huella de carbono y penalización de zonas residenciales.

## Política del Equipo sobre el Uso de IA
1. **Prohibición de Datos Sensibles:** Ningún prompt puede contener claves de API de mapas, credenciales de bases de datos, datos personales reales de usuarios ni información confidencial de la infraestructura.
2. **Revisión y Comprensión Obligatoria:** Todo código generado por IA debe ser leído, comprendido línea por línea y sometido a pruebas locales por el desarrollador antes de integrarlo al control de versiones (commit).
3. **Transparencia Activa:** Cualquier componente estructural, función crítica o diseño arquitectónico generado con asistencia de IA debe documentarse rigurosamente en este archivo para mantener la trazabilidad.
