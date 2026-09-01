---
title: "Messaging"
type: "pattern"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[System Integration]]"
related:
  - "[[Event-Driven Architecture]]"
  - "[[Microservices]]"
  - "[[Resilience]]"
tags:
  - solution-architecture
  - integracion
---

# Messaging

## ¿Qué es?
La mensajería es una forma de comunicar sistemas enviándose mensajes a través de un intermediario, sin que tengan que hablar directamente ni al mismo tiempo. Un sistema deja un mensaje y sigue con lo suyo; otro lo recoge cuando puede.

**Definición técnica:** estilo de comunicación asíncrona en el que los componentes intercambian mensajes a través de un *message broker* (cola o tópico), desacoplándose en el tiempo y en el espacio, con garantías de entrega configurables.

---

## ¿Por qué existe?
Las llamadas directas ([[API]] síncronas) acoplan a los sistemas: si el receptor está caído o lento, el emisor se bloquea o falla. La mensajería existe para desacoplarlos, absorber picos de carga y aumentar la resiliencia.

---

## ¿Qué problema resuelve?
- Acoplamiento temporal: el emisor no debe esperar al receptor.
- Picos de carga: los mensajes se acumulan en cola y se procesan al ritmo posible.
- Fallos del receptor: los mensajes esperan hasta que vuelva a estar disponible.

---

## ¿Cómo funciona?
Un **productor** envía mensajes a un **broker** (una cola o un tópico). Un **consumidor** los lee cuando puede. Dos modelos comunes:
- **Colas (point-to-point)**: cada mensaje lo procesa un solo consumidor.
- **Publicación/suscripción (pub/sub)**: un mensaje llega a varios interesados.

Es la base técnica de la [[Event-Driven Architecture]] y refuerza la [[Resilience]] de los [[Microservices]].

---

## Ejemplo sencillo
Es como dejar una nota en un buzón en lugar de llamar por teléfono. No necesitas que la otra persona esté disponible en ese instante: deja el mensaje y ella lo lee cuando puede. Si recibe muchas notas, las atiende una por una sin colapsar.

---

## Conceptos relacionados
- [[System Integration]] — la mensajería es un mecanismo clave de integración asíncrona.
- [[Event-Driven Architecture]] — se construye sobre mensajería.
- [[Microservices]] — la usan para comunicarse de forma desacoplada.
- [[Resilience]] — absorbe picos y tolera receptores caídos.

---

## Antes de estudiar esto
- [[System Integration]]

---

## Después de estudiar esto
- [[Event-Driven Architecture]]

---

## Preguntas de comprobación
1. ¿Qué significa que la mensajería sea "asíncrona"?
2. ¿Qué diferencia hay entre una cola y un modelo pub/sub?
3. ¿Cómo ayuda la mensajería a manejar picos de carga?
4. ¿Por qué desacopla mejor que una llamada API directa?

---

## Errores comunes
- Asumir entrega y orden garantizados sin configurarlos.
- No manejar mensajes que fallan repetidamente (necesidad de "dead letter queue").
- Usar mensajería cuando una simple llamada síncrona bastaría.

---

## Resumen
- Comunica sistemas mediante mensajes a través de un broker.
- Es asíncrona: desacopla en tiempo y espacio.
- Modelos: colas (point-to-point) y pub/sub.
- Absorbe picos y aumenta la resiliencia.
- Es la base de la arquitectura orientada a eventos.

---

## Fuentes
- Hohpe & Woolf — *Enterprise Integration Patterns*: https://www.enterpriseintegrationpatterns.com/
- Apache — *Kafka Documentation*: https://kafka.apache.org/documentation/
- AWS — *What is Message Queuing?*: https://aws.amazon.com/message-queue/
