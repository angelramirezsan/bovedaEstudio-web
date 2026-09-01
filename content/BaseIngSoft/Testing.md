---
title: "Testing"
type: "practice"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Programming Languages]]"
related:
  - "[[Debugging]]"
  - "[[CI-CD]]"
  - "[[Clean Code]]"
tags:
  - software-engineering
  - calidad
---

# Testing

## ¿Qué es?
Testing (pruebas) es verificar que el software hace lo que debe hacer, idealmente de forma automática. En lugar de comprobar todo a mano cada vez, escribes pruebas que se ejecutan solas y avisan si algo se rompió.

**Definición técnica:** el testing de software es el proceso de evaluar un sistema para detectar diferencias entre el comportamiento esperado y el real. Incluye niveles como pruebas unitarias, de integración y de extremo a extremo (end-to-end).

---

## ¿Por qué existe?
Todo cambio en el código puede romper algo que antes funcionaba. Comprobarlo manualmente no escala. El testing existe para dar confianza de que el sistema sigue funcionando tras cada cambio.

---

## ¿Qué problema resuelve?
- Detectar errores temprano, cuando son baratos de corregir.
- Permitir cambiar el código sin miedo a romper lo existente (regresiones).
- Documentar el comportamiento esperado del sistema.

---

## ¿Cómo funciona?
Se organiza por niveles, a menudo representados como una **pirámide de pruebas**:
- **Unitarias**: prueban una pieza pequeña y aislada (una función).
- **De integración**: prueban que varias piezas funcionan juntas.
- **End-to-end**: prueban el flujo completo como lo haría un usuario.

Una práctica común es **TDD (Test-Driven Development)**: escribir la prueba antes que el código. Las pruebas suelen ejecutarse automáticamente en cada cambio mediante [[CI-CD]].

---

## Ejemplo sencillo
Es como los controles de calidad en una fábrica: antes de que un producto salga, pasa por comprobaciones automáticas. Si una pieza falla, se detecta ahí y no en manos del cliente.

---

## Conceptos relacionados
- [[Debugging]] — testing detecta *que* hay un fallo; debugging encuentra *por qué*.
- [[CI-CD]] — las pruebas se ejecutan automáticamente en el pipeline.
- [[Clean Code]] — el código bien diseñado es más fácil de probar.

---

## Antes de estudiar esto
- [[Programming Languages]]
- [[Version Control]]

---

## Después de estudiar esto
- [[Debugging]]
- [[CI-CD]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre una prueba unitaria y una de integración?
2. ¿Por qué las pruebas dan confianza para refactorizar?
3. ¿Qué es una regresión y cómo ayudan las pruebas a evitarla?
4. ¿Qué propone TDD y qué ventaja tiene?

---

## Errores comunes
- Confundir "el código compila" con "el código funciona".
- Escribir solo pruebas end-to-end (lentas y frágiles) y descuidar las unitarias.
- Pruebas que dependen unas de otras o del orden de ejecución.

---

## Resumen
- El testing verifica que el software se comporte como se espera.
- Se organiza en niveles: unitario, integración, end-to-end.
- Da confianza para cambiar código sin romper lo existente.
- TDD escribe la prueba antes que el código.
- Se automatiza dentro de CI/CD.

---

## Fuentes
- Martin Fowler — *TestPyramid*: https://martinfowler.com/bliki/TestPyramid.html
- Python Software Foundation — *unittest*: https://docs.python.org/3/library/unittest.html
- Microsoft — *Learn: Testing fundamentals*: https://learn.microsoft.com/en-us/dotnet/core/testing/
