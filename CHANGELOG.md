# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-07-21
### Added
- Lanzamiento inicial de la API RESTful de enrutamiento EcoRutas (`v1`).
- Endpoint `/routes/calculate` para cálculo de rutas óptimas (Eco-Routing) minimizando el consumo de combustible.
- Endpoint `/tracking/sync` para sincronización de telemetría mediante *ping batching*.
- Implementación de algoritmos de optimización de rutas penalizando zonas escolares y residenciales de un solo carril.
- Documentación legal y ética estructurada (`LICENSE` MIT, `PRIVACY_POLICY.md`, `TERMS.md`, `CODE_OF_CONDUCT.md`).
- Archivos de transparencia y sostenibilidad técnica (`GREEN.md`, `ETHICS.md`, `AI_USAGE.md`).
- Implementación de seguridad con cifrado TLS 1.3 y hashing Argon2 en cumplimiento con la LOPDP.
- Especificación de la API en formato OpenAPI (`Api.yaml`).

### Changed
- Refactorización del algoritmo de búsqueda de grafos vehiculares utilizando procesamiento asíncrono (`asyncio`) y estructuras eficientes (`heapq`).
- Ajuste del esquema de sincronización GPS del lado del cliente, pasando de reportes de 1 segundo a un modelo de sondeo dinámico (10-15 segundos) para ahorrar batería y ancho de banda.

### Fixed
- Prevención de desbordamientos de memoria al procesar respuestas masivas de geolocalización.
- Corrección de sesgos algorítmicos que derivaban tráfico pesado por vías no arteriales.

## [0.5.0] - 2026-06-15
### Added
- Estructura base del repositorio de software y definición de la arquitectura de sistema.
- Configuración de entornos virtuales en Python y definición de dependencias (`requirements.txt`).
- Esquema de base de datos relacional para el registro anónimo de emisiones de CO2 y métricas de trayectos.

### Security
- Reglas de exclusión en `.gitignore` para evitar la filtración accidental de claves de API y archivos locales `.env`.
