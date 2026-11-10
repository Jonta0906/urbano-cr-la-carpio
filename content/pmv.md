## Evidencias documentales y planificación inicial

- Se recibieron ficha, historia EPACR-GIS-01, presentación en PDF y PPTX y backlog.
- S17 registra 17 tareas: una Completada (recopilación de cartografía), una En Progreso (normalización de proyecciones) y 15 No Iniciada. Son estados declarados.

S14 desarrolla EPACR-GIS-01/TS-101.2 (normalización de proyecciones). El backlog incluye ocho historias EPACR-GIS-01 a EPACR-GIS-08. Las fechas y firmas escritas del formulario se preservan en el anexo, sin inferir aprobación de todo el PMV.

### Tareas originales de S17

Fuente documental: archivo de planificación `S17` (ver inventario en Metodología). Cada fila conserva su código de trazabilidad original para vincular las tareas con los Issues y el tablero de seguimiento.

| Clave de importación | ID original | HU | Tarea | Prioridad | Rol | Horas estimadas | Estado declarado | Criterio original |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| S17-r13 | TS-101.1 | EPACR-GIS-01 | Recopilación de cartografía institucional para construcción de la línea base  | Should | QA Geoespacial | 8 | Completada | CRS EPSG:4326, metadato ISO 19115. |
| S17-r14 | TS-101.2 | EPACR-GIS-01 | Normalizar proyecciones de la línea base | Should | QA Geoespacial | 5 | En Progreso | CRS EPSG:4326, metadato ISO 19115. |
| S17-r15 | TS-101.3 | EPACR-GIS-01 | Crear Geodatabase para concentrar toda la información | Should | QA Geoespacial | No indicado | No Iniciada | CRS EPSG:4326, metadato ISO 19115. |
| S17-r16 | TS-101.4 | EPACR-GIS-01 | Validar topología y elaborar metadatos de todas las capas de información que deben concentrarse en la geodatabase | Should | QA Geoespacial | No indicado | No Iniciada | Geometrías validadas sin solapamientos ni duplicados topológicos. |
| S17-r17 | TS-102.1 | EPACR-GIS-02 | Consulta de mosaicos Sentinel-2 u otras colecciones disponibles libres de nubes | Should | Analista ETL SIG | No indicado | No Iniciada | Mosaico descargado, CRS EPSG:4326, metadato ISO 19115. Nubosidad inferior al 10% |
| S17-r18 | TS-103.1 | EPACR-GIS-03 | Procesar Script de cálculo de índice NDVI para detectar cambios temporales  | Should | Analista ETL SIG | No indicado | No Iniciada | Nubosidad inferior al 10% |
| S17-r19 | TS-104.1 | EPACR-GIS-04 | Clasificación supervisada para identificación de usos de suelo | Should | Analista ETL SIG | No indicado | No Iniciada | No indicado |
| S17-r20 | TS-105.1 | EPACR-GIS-05 | Construir índice multicriterio | Must | Líder Técnico SIG | No indicado | No Iniciada | Geometrías validadas sin solapamientos ni duplicados topológicos. |
| S17-r21 | TS-105.2 | EPACR-GIS-05 | Generar pendientes e integrar la hidrografía  | Must | Líder Técnico SIG | No indicado | No Iniciada | Geometrías validadas sin solapamientos ni duplicados topológicos. |
| S17-r22 | TS-105.3 | EPACR-GIS-05 | Calcular indice de densificación | Must | Líder Técnico SIG | No indicado | No Iniciada | Geometrías validadas sin solapamientos ni duplicados topológicos. |
| S17-r23 | TS-105.4 | EPACR-GIS-05 | Generar mapa de vulnerabilidad. | Must | Líder Técnico SIG | No indicado | No Iniciada | No indicado |
| S17-r24 | TS-106.1 | EPACR-GIS-06 | Construir modelos de crecimiento urbano para evaluar escenarios: tendencial,de intervención y  sostenible. | Could | Líder Técnico SIG | No indicado | No Iniciada | Algoritmo comparado contra línea base testigo; margen error <5%. |
| S17-r25 | TS-107.1 | EPACR-GIS-07 | Publicar servicios OGC | Must | Dev Frontend GIS | No indicado | No Iniciada | Topología limpia comprobada sin huecos; capa publicada en staging. |
| S17-r26 | TS-107.2 | EPACR-GIS-07 | Configurar el sistema de publicación Web y desarrollar visor | Must | Dev Frontend GIS | No indicado | No Iniciada | Topología limpia comprobada sin huecos; capa publicada en staging. |
| S17-r27 | TS-107.3 | EPACR-GIS-07 | Implementar filtros, widgets e  integrar el dashboard. | Must | Dev Frontend GIS | No indicado | No Iniciada | Topología limpia comprobada sin huecos; capa publicada en staging. |
| S17-r28 | TS-108.1 | EPACR-GIS-08 | Construcción de guía metodológica para replicación en otros asentamientos | Should | Líder Técnico SIG | No indicado | No Iniciada | Guía técnica y script de automatización en repositorio Git. |
| S17-r29 | TS-108.2 | EPACR-GIS-08 | Documentación de flujo ETL de actualización y guía de metadatos | Could | Líder Técnico SIG | No indicado | No Iniciada | Guía técnica y script de automatización en repositorio Git. |

## Especificación de módulos de aplicación

Estos componentes describen el diseño funcional previsto para el visor y el tablero de la iniciativa. Los módulos e indicadores se habilitan de forma progresiva a medida que el equipo incorpora y valida cada conjunto de datos en el repositorio.

- Ficha territorial de La Carpio con aviso de delimitación pendiente de homologar.
- Visor por capas de referencia, áreas verdes, usos del suelo y amenazas únicamente cuando existan capas revisadas.
- Filtros y widgets del tablero vinculados al mismo ámbito y fecha.
- Indicadores con fuente, definición y cobertura; no publicar automáticamente la cifra de población como dato actualizado.
- Espacio para metodología, acuerdos interinstitucionales y escenarios, cada uno con estado de desarrollo.

### Estados vacíos y navegación

Para garantizar la transparencia técnica, las capas e indicadores en preparación se identifican explícitamente como pendientes hasta contar con datos verificados, evitando sustituir mediciones faltantes con valores simulados. Todos los enlaces de colaboración de esta página conectan directamente con el repositorio oficial de la iniciativa.
