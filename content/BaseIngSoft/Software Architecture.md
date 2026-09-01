---
title: "Software Architecture"
type: "concept"
area: "Software Engineering"
level: 3
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Software Design]]"
  - "[[Design Patterns]]"
related:
  - "[[API]]"
  - "[[Microservices]]"
  - "[[Solution Architecture]]"
  - "[[Non-Functional Requirements]]"
tags:
  - software-engineering
  - arquitectura
---

# Software Architecture

## ¿Qué es?
La arquitectura de software es la estructura de alto nivel de un sistema: cuáles son sus grandes partes, cómo se dividen las responsabilidades y cómo se comunican. Son las decisiones que son difíciles de cambiar después.

**Definición técnica:** la arquitectura de software es el conjunto de estructuras del sistema, sus elementos, propiedades visibles y relaciones, junto con las decisiones fundamentales que guían su evolución y satisfacen requisitos funcionales y no funcionales.

---

## ¿Por qué existe?
A medida que un sistema crece, las decisiones de estructura tienen consecuencias enormes y costosas de revertir (cómo se dividen los servicios, cómo fluyen los datos). La arquitectura existe para tomar esas decisiones de forma consciente y alineada con los objetivos del negocio.

---

## ¿Qué problema resuelve?
- Sistemas que no soportan crecimiento porque su estructura no lo permite.
- Decisiones importantes tomadas por accidente en lugar de deliberadamente.
- Falta de una visión compartida entre equipos sobre cómo encaja todo.

---

## ¿Cómo funciona?
Define **estilos arquitectónicos** (monolito, capas, [[Microservices]], [[Event-Driven Architecture]]) y las decisiones clave: límites de componentes, flujo de datos, y cómo se satisfacen los [[Non-Functional Requirements]] (rendimiento, seguridad, escalabilidad). Opera a mayor escala que el [[Software Design]]: la arquitectura es la ciudad; el diseño, cada edificio.

---

## Ejemplo sencillo
Es como el plano urbanístico de una ciudad: dónde van las zonas residenciales, comerciales e industriales, cómo se conectan por avenidas. Cambiar el diseño de una casa es fácil; mover una avenida principal, no. Por eso la arquitectura se piensa con cuidado.

---

## Conceptos relacionados
- [[Software Design]] — la arquitectura opera a mayor escala que el diseño.
- [[Microservices]] — un estilo arquitectónico concreto.
- [[Solution Architecture]] — extiende la arquitectura de software a la solución completa (infraestructura, negocio, integración).
- [[Non-Functional Requirements]] — la arquitectura existe en gran parte para satisfacerlos.

---

## Antes de estudiar esto
- [[Software Design]]
- [[Design Patterns]]

---

## Después de estudiar esto
- [[API]]
- [[Microservices]]
- [[Solution Architecture]]

---

## Preguntas de comprobación
1. ¿Qué caracteriza a una decisión "arquitectónica" frente a una de diseño?
2. ¿Por qué las decisiones arquitectónicas son costosas de revertir?
3. ¿Qué relación hay entre arquitectura y requisitos no funcionales?
4. ¿En qué se diferencia un monolito de una arquitectura de microservicios?

---

## Errores comunes
- Elegir microservicios por moda sin necesitar su complejidad.
- Confundir arquitectura (estructura y decisiones) con diagramas bonitos.
- Ignorar los requisitos no funcionales hasta que el sistema falla en producción.

---

## Resumen
- Define la estructura de alto nivel y las decisiones difíciles de revertir.
- Divide responsabilidades y define cómo se comunican las partes.
- Existe para satisfacer requisitos funcionales y no funcionales.
- Opera a mayor escala que el diseño de software.
- Es el puente hacia la arquitectura de soluciones.

---

## Fuentes
- Bass, Clements, Kazman — *Software Architecture in Practice* (Addison-Wesley), ISBN 978-0136886099.
- Microsoft — *Azure Architecture Center*: https://learn.microsoft.com/en-us/azure/architecture/
- ISO/IEC/IEEE — *42010: Architecture description*: https://www.iso.org/standard/74393.html
