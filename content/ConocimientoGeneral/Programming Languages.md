---
title: "Programming Languages"
type: "concept"
area: "Software Engineering"
level: 1
status: "not-started"
difficulty: "basic"
prerequisites: []
related:
  - "[[Data Structures and Algorithms]]"
  - "[[Software Design]]"
  - "[[Debugging]]"
tags:
  - fundamentos
---

# Programming Languages

## ¿Qué es?
Un lenguaje de programación es la forma en que le damos instrucciones a una computadora usando reglas y palabras que ella puede entender. Es el "idioma" con el que escribes lo que quieres que el sistema haga.

**Definición técnica:** un lenguaje de programación es un sistema formal de notación, con una sintaxis y una semántica definidas, que permite expresar algoritmos y estructuras de datos que luego son traducidos (compilados o interpretados) a instrucciones ejecutables por una máquina.

---

## ¿Por qué existe?
Las computadoras solo entienden código máquina (unos y ceros). Escribir directamente en ese nivel es lento, propenso a errores e imposible de mantener. Los lenguajes de programación existen para que las personas puedan expresar ideas complejas de forma legible y que una herramienta las traduzca a algo que la máquina ejecuta.

---

## ¿Qué problema resuelve?
- Traducir intención humana en instrucciones ejecutables.
- Permitir abstracción: pensar en "clientes" y "pedidos" en lugar de registros de memoria.
- Facilitar mantenimiento, colaboración y reutilización de código.

---

## ¿Cómo funciona?
El código fuente se transforma en instrucciones ejecutables por dos vías principales:
- **Compilación**: se traduce todo el programa antes de ejecutarlo (ej. C, Go, Rust).
- **Interpretación / JIT**: se traduce y ejecuta sobre la marcha (ej. Python, JavaScript).

Los lenguajes se agrupan por **paradigmas**: imperativo, orientado a objetos, funcional, declarativo. Un mismo problema puede resolverse con distintos paradigmas.

---

## Ejemplo sencillo
Piensa en una receta de cocina. La receta (código fuente) está escrita en un idioma que entiendes; tú (el intérprete) la ejecutas paso a paso. Si estuviera escrita en símbolos químicos exactos (código máquina) sería precisa pero inutilizable para una persona.

---

## Conceptos relacionados
- [[Data Structures and Algorithms]] — el lenguaje es el medio; las estructuras y algoritmos son *qué* expresas con él.
- [[Software Design]] — un buen diseño trasciende el lenguaje concreto.
- [[Debugging]] — los errores se encuentran y corrigen en el código escrito en el lenguaje.

---

## Antes de estudiar esto
- (Ninguno — es un punto de entrada del grafo.)

---

## Después de estudiar esto
- [[Data Structures and Algorithms]]
- [[Version Control]]

---

## Preguntas de comprobación
1. ¿Por qué no programamos directamente en código máquina?
2. ¿Qué diferencia hay entre compilar e interpretar?
3. ¿Qué significa que un lenguaje siga un "paradigma"?
4. ¿Por qué el diseño de software no depende de un lenguaje concreto?

---

## Errores comunes
- Creer que "saber un lenguaje" equivale a "saber programar"; lo transferible son los conceptos, no la sintaxis.
- Confundir el lenguaje (herramienta) con el paradigma (forma de pensar).
- Pensar que un lenguaje es siempre mejor que otro; depende del problema y el contexto.

---

## Resumen
- Un lenguaje de programación traduce intención humana en instrucciones ejecutables.
- Existe para abstraer y hacer mantenible lo que sería imposible en código máquina.
- Se ejecuta vía compilación o interpretación.
- Los paradigmas describen formas de pensar los problemas.
- Los conceptos son transferibles entre lenguajes; la sintaxis no.

---

## Fuentes
- Python Software Foundation — *Python Documentation*: https://docs.python.org/3/
- Mozilla — *MDN Web Docs: JavaScript*: https://developer.mozilla.org/en-US/docs/Web/JavaScript
- Microsoft — *.NET Documentation*: https://learn.microsoft.com/en-us/dotnet/
