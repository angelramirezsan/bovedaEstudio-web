---
title: "Design Patterns"
type: "pattern"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Software Design]]"
related:
  - "[[Clean Code]]"
  - "[[Software Architecture]]"
tags:
  - software-engineering
  - diseno
---

# Design Patterns

## ¿Qué es?
Los patrones de diseño son soluciones ya conocidas y probadas para problemas que aparecen una y otra vez al programar. En lugar de reinventar la rueda, aplicas una solución que la comunidad ya validó.

**Definición técnica:** un patrón de diseño es una solución general y reutilizable a un problema recurrente dentro de un contexto de diseño. Los patrones clásicos (creacionales, estructurales y de comportamiento) fueron catalogados por el "Gang of Four".

---

## ¿Por qué existe?
Muchos problemas de diseño se repiten entre proyectos (crear objetos, comunicar componentes, extender comportamiento). Los patrones existen para dar un vocabulario común y soluciones probadas, evitando errores ya conocidos.

---

## ¿Qué problema resuelve?
- Resolver problemas de diseño recurrentes sin improvisar.
- Comunicar ideas de diseño con un vocabulario compartido ("usemos un Observer aquí").
- Evitar trampas ya identificadas por la industria.

---

## ¿Cómo funciona?
Se agrupan en familias:
- **Creacionales** (cómo crear objetos): Factory, Singleton, Builder.
- **Estructurales** (cómo componer objetos): Adapter, Decorator, Facade.
- **De comportamiento** (cómo interactúan): Observer, Strategy, Command.

Un patrón no es código para copiar, sino una plantilla que adaptas a tu caso.

---

## Ejemplo sencillo
Son como recetas de cocina reconocidas: "sofrito", "salsa madre". No te dicen exactamente qué plato hacer, pero te dan una técnica probada que aplicas a tus ingredientes. Nombrar la técnica ("hagamos un roux") comunica mucho en pocas palabras.

---

## Conceptos relacionados
- [[Software Design]] — los patrones son herramientas del diseño.
- [[Clean Code]] — bien aplicados mejoran la claridad; mal aplicados la empeoran.
- [[Software Architecture]] — existen también patrones a nivel arquitectónico.

---

## Antes de estudiar esto
- [[Software Design]]

---

## Después de estudiar esto
- [[Software Architecture]]

---

## Preguntas de comprobación
1. ¿Por qué un patrón es una plantilla y no código para copiar?
2. ¿Qué diferencia hay entre patrones creacionales, estructurales y de comportamiento?
3. ¿Qué ventaja da tener un "vocabulario común" de patrones en un equipo?
4. ¿Por qué aplicar patrones sin necesidad puede empeorar el diseño?

---

## Errores comunes
- Forzar patrones donde no hacen falta (sobre-ingeniería).
- Memorizar patrones sin entender el problema que resuelven.
- Confundir un patrón de diseño con una librería o framework.

---

## Resumen
- Son soluciones probadas a problemas de diseño recurrentes.
- Se agrupan en creacionales, estructurales y de comportamiento.
- Dan un vocabulario común al equipo.
- Son plantillas que se adaptan, no código a copiar.
- Usados sin criterio, añaden complejidad innecesaria.

---

## Fuentes
- Gamma, Helm, Johnson, Vlissides — *Design Patterns* (Addison-Wesley, 1994), ISBN 978-0201633610.
- Refactoring.Guru — *Design Patterns*: https://refactoring.guru/design-patterns
