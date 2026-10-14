# Arquitectura de AutoCheck

Documentación viva de arquitectura: decisiones (ADR) y diagramas como código (PlantUML).

## Trazabilidad: necesidad → decisión → diseño

| Necesidad | Decisión (ADR) | Estado | Diagramas |
|---|---|---|---|
| Organizar módulos y responsabilidades | [ADR-0001: Patrón arquitectónico](adr/0001-patron-arquitectonico.md) | Aceptado | [C4 de contexto](diagrams/c4-contexto.puml), [Secuencia](diagrams/secuencia-proceso-clave.puml) |
| Almacenar usuarios, vehículos y evaluaciones | [ADR-0002: Sistema de persistencia](adr/0002-sistema-de-persistencia.md) | Propuesto | [C4 de contexto](diagrams/c4-contexto.puml), [Secuencia](diagrams/secuencia-proceso-clave.puml) |
| Proteger cuentas, datos y fotografías | [ADR-0003: Estrategia de seguridad](adr/0003-estrategia-seguridad.md) | Propuesto | [Secuencia](diagrams/secuencia-proceso-clave.puml) |

## Cómo mantenerla
- Un cambio de arquitectura implica un nuevo ADR o actualizar el existente.
- Los diagramas se editan en los `.puml` y se versionan con Git.