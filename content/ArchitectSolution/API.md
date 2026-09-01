---
title: "API"
type: "concept"
area: "Solution Architecture"
level: 3
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[HTTP]]"
  - "[[Software Architecture]]"
related:
  - "[[Microservices]]"
  - "[[System Integration]]"
  - "[[AI Services]]"
tags:
  - solution-architecture
  - integracion
---

# API

## ¿Qué es?
Una API es un "contrato" que permite que dos programas se comuniquen sin conocer los detalles internos del otro. Define qué puedes pedir y qué recibirás, como un menú de un restaurante: sabes qué platos puedes ordenar sin ver la cocina.

**Definición técnica:** una API (Application Programming Interface) es una interfaz que expone un conjunto de operaciones, contratos de entrada/salida y reglas, permitiendo que un sistema consuma la funcionalidad de otro ocultando su implementación interna.

---

## ¿Por qué existe?
Los sistemas necesitan usar funciones de otros sistemas sin acoplarse a su código interno. La API existe para ofrecer un punto de acceso estable: el proveedor puede cambiar su implementación mientras el contrato se mantenga.

---

## ¿Qué problema resuelve?
- Comunicar sistemas heterogéneos de forma estandarizada.
- Ocultar la complejidad interna detrás de una interfaz clara.
- Permitir reutilizar funcionalidad sin duplicarla.

---

## ¿Cómo funciona?
El consumidor envía una petición al contrato definido por la API (típicamente sobre [[HTTP]], en estilos como REST o GraphQL) y recibe una respuesta estructurada (habitualmente JSON). La API valida, procesa y responde. Un buen diseño de API es estable, versionado y bien documentado ([[Documentation]]).

---

## Ejemplo sencillo
Es como un enchufe eléctrico: no necesitas saber cómo la central genera electricidad, solo conectar tu aparato al estándar. La API es ese enchufe entre programas: un punto de conexión acordado.

---

## Conceptos relacionados
- [[HTTP]] — la mayoría de las APIs web se apoyan en él.
- [[Microservices]] — se comunican entre sí a través de APIs.
- [[System Integration]] — las APIs son el principal mecanismo de integración.
- [[AI Services]] — la IA suele consumirse como una API.

---

## Antes de estudiar esto
- [[HTTP]]
- [[Software Architecture]]

---

## Después de estudiar esto
- [[Microservices]]
- [[System Integration]]

---

## Preguntas de comprobación
1. ¿Qué problema resuelve una API?
2. ¿Qué diferencia existe entre una API y una interfaz de usuario?
3. ¿Por qué una API puede ser importante dentro de una arquitectura de microservicios?
4. ¿Por qué versionar una API es importante para sus consumidores?

---

## Errores comunes
- Confundir API (interfaz para programas) con UI (interfaz para personas).
- Exponer la estructura interna de la base de datos directamente como API.
- Romper el contrato sin versionar, rompiendo a todos los consumidores.

---

## Resumen
- Una API es un contrato que comunica programas ocultando su interior.
- Permite integrar y reutilizar funcionalidad de forma estable.
- Suele apoyarse en HTTP (REST, GraphQL).
- Es la base de microservicios e integración de sistemas.
- La IA moderna se consume mayormente vía APIs.

---

## Fuentes
- Mozilla — *MDN Web Docs: Introduction to web APIs*: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction
- OpenAPI Initiative — *OpenAPI Specification*: https://spec.openapis.org/oas/latest.html
- Microsoft — *Learn: Web API design best practices*: https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design
