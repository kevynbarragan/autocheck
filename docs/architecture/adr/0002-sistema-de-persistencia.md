# ADR-0002: Sistema de persistencia

- **Estado:** Propuesto
- **Fecha:** 2026-10-14

## Contexto
Se deben almacenar usuarios, vehículos, evaluaciones y fotografías, y consultarlos de forma relacional.

## Decisión
Se propone una base de datos relacional para datos estructurados y almacenamiento de archivos para las fotografías.

## Alternativas consideradas
- Base de datos NoSQL: flexible, pero las relaciones usuario-vehículo-evaluación son naturalmente relacionales.
- Guardar fotos dentro de la base de datos: afecta el rendimiento.

## Consecuencias
- Consultas y reportes más simples.
- Requiere definir un esquema y migraciones.

## Diagramas relacionados
- [C4 de contexto](../diagrams/c4-contexto.puml)
- [Secuencia del proceso principal](../diagrams/secuencia-proceso-clave.puml)