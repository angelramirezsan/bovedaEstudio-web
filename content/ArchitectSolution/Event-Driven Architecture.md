---
title: "Event-Driven Architecture"
type: "architecture"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "advanced"
prerequisites:
  - "[[Messaging]]"
  - "[[Microservices]]"
related:
  - "[[System Integration]]"
  - "[[Distributed Systems]]"
  - "[[Resilience]]"
tags:
  - solution-architecture
  - eventos
---

# Event-Driven Architecture

## ¿Qué es?
La arquitectura orientada a eventos (EDA) es un estilo en el que los componentes reaccionan a "eventos" (cosas que pasaron), en lugar de llamarse directamente unos a otros. Cuando algo ocurre ("pedido creado"), se publica un evento y quien esté interesado reacciona.

**Definición técnica:** estilo arquitectónico en el que la comunicación se basa en la producción, detección y consumo de eventos (hechos inmutables ocurridos en el pasado), promoviendo desacoplamiento entre productores y consumidores mediante [[Messaging]].

---

## ¿Por qué existe?
En sistemas complejos, hacer que cada componente conozca y llame a todos los demás genera un enredo frágil. EDA existe para desacoplar: el productor de un evento no necesita saber quién ni cuántos reaccionan a él.

---

## ¿Qué problema resuelve?
- Acoplamiento fuerte entre componentes que se llaman directamente.
- Dificultad para añadir nuevos comportamientos sin tocar el código existente.
- Necesidad de reaccionar a hechos en tiempo casi real.

---

## ¿Cómo funciona?
Un componente **publica** un evento cuando algo ocurre. Otros **se suscriben** y reaccionan de forma independiente. El productor no sabe quién consume: para añadir una nueva reacción, basta suscribir un nuevo consumidor sin modificar al productor. Se apoya en [[Messaging]] (pub/sub) e introduce la complejidad de los [[Distributed Systems]] (orden, duplicados, consistencia eventual).

---

## Ejemplo sencillo
Es como publicar en un tablón de anuncios: quien pone el aviso ("se vendió el producto X") no sabe quién lo leerá. El de facturación, el de inventario y el de notificaciones lo ven y cada uno actúa. Añadir un nuevo interesado no obliga a cambiar el aviso.

---

## Conceptos relacionados
- [[Messaging]] — el mecanismo técnico que la sustenta.
- [[Microservices]] — EDA es una forma habitual de comunicarlos.
- [[Distributed Systems]] — hereda sus retos de orden y consistencia.
- [[Resilience]] — el desacoplamiento aumenta la tolerancia a fallos.

---

## Antes de estudiar esto
- [[Messaging]]
- [[Microservices]]

---

## Después de estudiar esto
- [[Distributed Systems]]
- [[Solution Architecture]]

---

## Preguntas de comprobación
1. ¿Qué es un "evento" en este contexto?
2. ¿Por qué el productor no conoce a sus consumidores?
3. ¿Qué ventaja da para extender el sistema sin modificar lo existente?
4. ¿Qué complejidades hereda de los sistemas distribuidos?

---

## Errores comunes
- Usar eventos para todo, incluso donde una llamada directa sería más clara.
- Ignorar el orden y la posible duplicación de eventos.
- Confundir un "evento" (algo que pasó) con un "comando" (una orden de hacer algo).

---

## Resumen
- Los componentes reaccionan a eventos en lugar de llamarse directamente.
- Desacopla productores y consumidores.
- Facilita extender el sistema sin modificar lo existente.
- Se apoya en mensajería pub/sub.
- Hereda los retos de los sistemas distribuidos.

---

## Fuentes
- Martin Fowler — *What do you mean by "Event-Driven"?*: https://martinfowler.com/articles/201701-event-driven.html
- AWS — *Event-Driven Architecture*: https://aws.amazon.com/event-driven-architecture/
- Microsoft — *Azure Architecture Center: Event-driven architecture*: https://learn.microsoft.com/en-us/azure/architecture/guide/architecture-styles/event-driven
