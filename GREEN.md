# Documentación de Sostenibilidad (GREEN)

## Criterios para Diseño de software con eficiencia energética
| No | OPORTUNIDAD IDENTIFICADA | IMPACTO ESPERADO |
|---|---|---|
| 1 | Almacenar en caché espacial (Redis) las rutas más consultadas. | Reduce consultas a la BD y procesamiento de CPU en un 35%. |
| 2 | Implementar "sondeo dinámico" para reducir la frecuencia de pings de GPS. | Ahorra batería del usuario y disminuye el uso de red. |
| 3 | Uso de procesamiento asíncrono (asyncio en Python) para I/O. | Maximiza la eficiencia del servidor, permitiendo más concurrencia sin escalar hardware. |

## Obsolescencia del Hardware
El diseño de EcoRutas prioriza el procesamiento en la nube y presenta una interfaz de usuario cliente sumamente ligera. Esto significa que el software no requiere hardware de última generación para funcionar de manera fluida. Cualquier dispositivo móvil fabricado en los últimos 7 años capaz de correr un navegador web estándar es compatible con nuestra plataforma. Como desarrolladores, tenemos la responsabilidad directa frente a los residuos electrónicos (e-waste). Evitamos deliberadamente inflar la aplicación con animaciones pesadas, procesos en segundo plano innecesarios o exigencias excesivas de memoria RAM. Al hacer que nuestro software sea compatible con equipos más antiguos, extendemos la vida útil tecnológica de los dispositivos de los usuarios, mitigando la cultura del desecho y promoviendo un consumo tecnológico responsable.
