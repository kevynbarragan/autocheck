# ADR-0001: Patrón arquitectónico

- **Estado:** Aceptado
- **Fecha:** 2026-10-14

## Contexto
AutoCheck necesita separar la interfaz web, la lógica de negocio y el análisis con IA para que el equipo pueda trabajar en paralelo y mantener el sistema.

## Decisión
Se adopta una arquitectura cliente-servidor en capas: interfaz web, backend/API y servicio de evaluación con IA.

## Alternativas consideradas
- Monolito sin separación de capas: más rápido al inicio, pero difícil de mantener.
- Microservicios: demasiada complejidad para el alcance del proyecto.

## Consecuencias
- Responsabilidades claras por capa.
- Mayor esfuerzo inicial de organización.

## Diagramas relacionados
- [C4 de contexto](../diagrams/c4-contexto.puml)
- [Secuencia del proceso principal](../diagrams/secuencia-proceso-clave.puml)