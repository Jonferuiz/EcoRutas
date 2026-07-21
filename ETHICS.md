# Decisiones Éticas del Equipo (ETHICS)

**1. ¿Qué herramientas de IA se usaron en el proyecto y para qué?**
* Se utilizaron modelos generativos para la refactorización de scripts en Python, optimización de algoritmos de grafos y asistencia en la redacción de documentación legal y técnica del repositorio.

**2. ¿Qué sesgos potenciales podría tener el sistema que se construye?**
* El algoritmo de enrutamiento podría sufrir un sesgo de priorización vehicular, tendiendo a dirigir volúmenes masivos de tráfico hacia barrios residenciales o zonas de menores ingresos con el fin de descongestionar avenidas principales, afectando negativamente la calidad de vida de esos residentes.

**3. ¿Qué medidas se tomaron para mitigar esos sesgos?**
* Se implementaron penalizaciones de peso en los nodos del grafo correspondientes a zonas escolares, hospitales y vías residenciales de un solo carril, asegurando que el enrutamiento priorice vías arteriales diseñadas para alto flujo de la ciudad.

**4. ¿Qué principios del ACM Code of Ethics o IEEE Code of Ethics se aplicaron?**
* Se aplicó el Principio 1.1 del ACM Code of Ethics ("Contribuir a la sociedad y al bienestar humano, reconociendo que todas las personas son partes interesadas en la informática"). Se prioriza el bienestar ambiental (reducción de CO2) y la seguridad comunitaria sobre la simple velocidad matemática.

**5. ¿Qué dilemas éticos enfrentó el equipo durante el desarrollo y cómo los resolvió?**
* El principal dilema fue decidir entre ofrecer la ruta más rápida (que incentiva al usuario a usar la app de inmediato) frente a la ruta más ecológica (que podría ser ligeramente más lenta). Se resolvió ofreciendo ambas opciones de forma transparente, pero marcando visualmente y preseleccionando siempre la "Ruta Verde" como la opción por defecto.
