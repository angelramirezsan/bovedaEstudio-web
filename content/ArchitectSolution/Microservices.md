---
title: "Microservices"
type: "architecture"
area: "Solution Architecture"
level: 3
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[API]]"
  - "[[Software Architecture]]"
related:
  - "[[System Integration]]"
  - "[[Distributed Systems]]"
  - "[[Containers]]"
  - "[[Event-Driven Architecture]]"
  - "[[AI Agents]]"
tags:
  - solution-architecture
---

# Microservices

## ¿Qué es?
Microservicios es un estilo de arquitectura en el que una aplicación se construye como un conjunto de servicios pequeños e independientes, cada uno con una responsabilidad concreta, que se comunican entre sí mediante [[API]]. Es lo opuesto a tener todo en un solo bloque (monolito).

**Definición técnica:** patrón arquitectónico en el que un sistema se descompone en servicios desplegables de forma independiente, con límites definidos por capacidades de negocio, que se comunican por protocolos ligeros (habitualmente APIs sobre HTTP o mensajería).

---

## ¿Por qué existe?
En sistemas grandes, un monolito único se vuelve difícil de entender, desplegar y escalar: un cambio pequeño obliga a redesplegar todo. Los microservicios existen para permitir que distintos equipos desarrollen, desplieguen y escalen partes de forma independiente.

---

## ¿Qué problema resuelve?
- Escalar solo la parte que lo necesita, no todo el sistema.
- Permitir que equipos trabajen y desplieguen de forma autónoma.
- Aislar fallos para que un problema no tumbe todo el sistema.

---

## ¿Cómo funciona?
Cada servicio tiene su propia responsabilidad y a menudo su propia base de datos. Se comunican vía [[API]] o [[Messaging]]. Suelen empaquetarse en [[Containers]] y desplegarse de forma independiente. Como introducen las complejidades de los [[Distributed Systems]] (red, latencia, fallos parciales), no siempre son la mejor opción: un monolito bien diseñado suele ser mejor punto de partida.

---

## Ejemplo sencillo
Es como una empresa organizada en departamentos especializados (ventas, logística, soporte) en lugar de una sola persona haciéndolo todo. Cada departamento opera de forma autónoma y se coordina con los demás mediante mensajes claros.

---

## Conceptos relacionados
- [[API]] — el mecanismo por el que se comunican.
- [[Distributed Systems]] — los microservicios son un caso concreto de sistema distribuido.
- [[Containers]] — la forma habitual de empaquetarlos y desplegarlos.
- [[Event-Driven Architecture]] — un estilo común para comunicarlos de forma desacoplada.
- [[AI Agents]] — evolucionan la idea de servicios autónomos hacia componentes con IA.

---

## Antes de estudiar esto
- [[API]]
- [[Software Architecture]]

---

## Después de estudiar esto
- [[System Integration]]
- [[Distributed Systems]]

---

## Preguntas de comprobación
1. ¿Qué diferencia a un microservicio de un monolito?
2. ¿Qué ventajas de escalado e independencia ofrecen?
3. ¿Qué complejidades nuevas introducen respecto a un monolito?
4. ¿Por qué no siempre conviene empezar con microservicios?

---

## Errores comunes
- Adoptarlos por moda sin necesitar su escala ni su independencia.
- Crear microservicios tan acoplados que en la práctica son un monolito distribuido.
- Subestimar la complejidad operativa (red, observabilidad, despliegue).

---

## Resumen
- Descomponen la aplicación en servicios pequeños e independientes.
- Se comunican por APIs o mensajería.
- Permiten escalar y desplegar partes de forma autónoma.
- Introducen la complejidad de los sistemas distribuidos.
- No siempre son la mejor opción de partida.

---

## Fuentes
- Martin Fowler — *Microservices*: https://martinfowler.com/articles/microservices.html
- Microsoft — *Azure Architecture Center: Microservices*: https://learn.microsoft.com/en-us/azure/architecture/guide/architecture-styles/microservices
- AWS — *What are Microservices?*: https://aws.amazon.com/microservices/
