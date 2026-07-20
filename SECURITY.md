# Seguridad y Auditoría (SECURITY)

## Medidas de Protección Implementadas (Conforme a la LOPDP)
* **Cifrado en Tránsito:** Uso de TLS 1.3 para proteger las transmisiones de datos de geolocalización entre la aplicación y el servidor.
* **Cifrado en Reposo:** Las contraseñas de los usuarios se almacenan mediante el robusto algoritmo de hashing Argon2.
* **Control de Acceso:** Implementación de Autenticación de Dos Factores (2FA) para el acceso al panel de administración y métricas generales.
* **Backups Seguros:** Copias de seguridad cifradas diarias de las bases de datos transaccionales, excluyendo intencionalmente historiales temporales de ubicación precisa.

## Auditoría Ética del Repositorio
| No | Criterio | Cumple | Hallazgos y corrección |
|---|---|---|---|
| 1 | ¿Tiene archivo LICENSE declarado y justificado? | SI | Archivo MIT en raíz del proyecto. |
| 2 | ¿El .gitignore excluye archivos sensibles? | SI | Excluye `.env`, `venv/` y archivos de caché de Python. |
| 3 | ¿Hay credenciales o API keys expuestas? | NO | Revisión limpia, la configuración se maneja mediante variables de entorno local. |
| 4 | ¿Los commits son descriptivos y trazables? | SI | Estandarización de prefijos semánticos (feat, fix, docs). |
| 5 | ¿Tiene CODE_OF_CONDUCT.md? | SI | Adaptado de Contributor Covenant v2.1. |
| 6 | ¿Hay CREDITS.md o sección de atribuciones? | SI | Atribuciones correctamente integradas en el README principal. |
| 7 | ¿El README tiene sección de licencia? | SI | Badge y enlace directo a LICENSE incluidos en la cabecera. |
| 8 | ¿El código de terceros está atribuido? | SI | Comentarios explícitos en el código fuente de las librerías importadas. |
| 9 | ¿Existe AI_USAGE.md si se usó IA? | SI | Archivo redactado con registro de prompts y políticas. |
| 10 | ¿Es presentable para un reclutador? | SI | Documentación completa, ordenada y técnicamente fundamentada. |
