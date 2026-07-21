# Documentación de Sostenibilidad (GREEN)

El proyecto EcoRutas está diseñado desde su núcleo para ser una herramienta de mitigación del cambio climático. Sin embargo, el software en sí mismo consume energía. Por ello, se han aplicado principios de "Green Software" para garantizar que la plataforma opere con la máxima eficiencia energética posible.

## Criterios para Diseño de software con eficiencia energética

A continuación, se identifican las oportunidades implementadas en la arquitectura de EcoRutas para reducir su impacto ambiental:

| No | OPORTUNIDAD IDENTIFICADA | IMPACTO ESPERADO |
| :--- | :--- | :--- |
| 1 | **Implementación de Caché Espacial (Redis):** Almacenar en memoria temporal las rutas más consultadas en zonas de alto tráfico. | Reduce las consultas a la base de datos y la ejecución de algoritmos de grafos complejos, ahorrando hasta un 35% de ciclos de CPU en el servidor backend. |
| 2 | **Sondeo dinámico y compresión de carga útil (Batching):** Agrupar las coordenadas GPS del cliente y enviarlas cada 10-15 segundos en lugar de cada segundo. | Disminuye drásticamente el uso de la red (antenas móviles) y reduce el consumo de batería del dispositivo del usuario. |
| 3 | **Procesamiento Asíncrono (I/O no bloqueante):** Utilización de `asyncio` en Python para manejar las peticiones a la API y la base de datos sin bloquear los hilos principales. | Maximiza la utilización del hardware existente, permitiendo procesar más usuarios concurrentes sin necesidad de adquirir nuevos servidores (reduciendo el carbono incorporado). |

## Obsolescencia del Hardware

El diseño arquitectónico de EcoRutas asume una gran responsabilidad frente a la problemática de la basura electrónica (e-waste). El software no requiere hardware de última generación para funcionar de manera óptima. Se ha adoptado un modelo de "cliente ligero" (Thin Client) para la aplicación móvil y web, donde todo el procesamiento pesado (como el cálculo de emisiones de CO2 y el algoritmo de enrutamiento) se ejecuta exclusivamente en la nube. 

El dispositivo del usuario únicamente se encarga de renderizar el mapa y enviar coordenadas empaquetadas. Esto garantiza una total compatibilidad con teléfonos móviles inteligentes más antiguos, evitando exigir grandes cantidades de memoria RAM o procesadores modernos. Como desarrolladores, tenemos la responsabilidad ética de no inflar el software con procesos en segundo plano o animaciones innecesarias que fuercen al usuario a desechar un equipo funcional. Al mantener los requisitos técnicos al mínimo, EcoRutas fomenta activamente la extensión de la vida útil del hardware, promoviendo un consumo tecnológico circular y responsable en la sociedad.
