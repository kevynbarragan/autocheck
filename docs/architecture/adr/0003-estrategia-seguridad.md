# ADR-0003: Estrategia de seguridad

- **Estado:** Propuesto
- **Fecha:** 2026-10-14

## Contexto
El sistema maneja cuentas de usuario, datos de vehículos y fotografías que deben protegerse.

## Decisión
Se propone autenticación con tokens, validación de datos y permisos en el backend, contraseñas con hash y comunicación por HTTPS.

## Alternativas consideradas
- Sesiones en servidor: válidas, pero menos adecuadas si el frontend y el backend se separan.
- Validar solo en el frontend: insuficiente.

## Consecuencias
- Mayor protección de datos y fotografías.
- Se debe gestionar la expiración y renovación de tokens.

## Diagramas relacionados
- [Secuencia del proceso principal](../diagrams/secuencia-proceso-clave.puml)