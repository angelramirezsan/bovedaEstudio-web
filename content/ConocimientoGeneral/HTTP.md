---
title: "HTTP"
type: "standard"
area: "Software Engineering"
level: 1
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Programming Languages]]"
related:
  - "[[API]]"
  - "[[System Integration]]"
  - "[[Security Fundamentals]]"
tags:
  - fundamentos
  - estandar
---

# HTTP

## ¿Qué es?
HTTP es el conjunto de reglas que usan los navegadores, aplicaciones y servidores para pedirse información entre sí a través de internet. Cuando abres una página web o una app consulta datos, casi siempre hay HTTP de por medio.

**Definición técnica:** HTTP (HyperText Transfer Protocol) es un protocolo de capa de aplicación, sin estado, basado en el modelo petición-respuesta, estandarizado por la IETF, que define cómo un cliente solicita recursos a un servidor y cómo este responde.

---

## ¿Por qué existe?
Para que sistemas distintos (hechos por distintas personas, en distintos lenguajes) puedan comunicarse necesitaban un lenguaje común y acordado. HTTP surge como ese estándar universal para transferir recursos en la web.

---

## ¿Qué problema resuelve?
- Estandariza la comunicación cliente-servidor sin importar la tecnología de cada lado.
- Define verbos claros (GET, POST, PUT, DELETE) y códigos de estado (200, 404, 500).
- Permite que la web y las [[API]] modernas funcionen de forma interoperable.

---

## ¿Cómo funciona?
El cliente envía una **petición** con un método (GET, POST...), una URL, cabeceras y opcionalmente un cuerpo. El servidor devuelve una **respuesta** con un código de estado, cabeceras y un cuerpo. Es **sin estado**: cada petición es independiente, lo que obliga a mecanismos como tokens o cookies para mantener sesión. Su versión segura, **HTTPS**, añade cifrado mediante TLS.

---

## Ejemplo sencillo
Es como pedir en un restaurante: haces una petición ("una GET del menú, por favor"), el mesero (servidor) responde con el plato (recurso) o con un mensaje ("404: ese plato no existe"). Cada pedido es independiente: el mesero no recuerda lo que pediste ayer a menos que le des tu nombre (token/cookie).

---

## Conceptos relacionados
- [[API]] — la mayoría de las APIs web se exponen sobre HTTP.
- [[System Integration]] — HTTP es uno de los canales más comunes para integrar sistemas.
- [[Security Fundamentals]] — HTTPS/TLS protege la comunicación HTTP.

---

## Antes de estudiar esto
- [[Programming Languages]]

---

## Después de estudiar esto
- [[API]]
- [[Security Fundamentals]]

---

## Preguntas de comprobación
1. ¿Qué significa que HTTP sea "sin estado" y qué implicaciones tiene?
2. ¿Qué diferencia hay entre GET y POST a nivel conceptual?
3. ¿Qué información aporta un código de estado como 404 o 500?
4. ¿Qué añade HTTPS respecto a HTTP?

---

## Errores comunes
- Usar GET para operaciones que modifican datos (deberían usar POST/PUT/DELETE).
- Creer que HTTPS "asegura" la aplicación entera; solo cifra el transporte.
- Ignorar el significado de los códigos de estado y devolver siempre 200.

---

## Resumen
- HTTP es el protocolo estándar de comunicación cliente-servidor en la web.
- Funciona por petición-respuesta y es sin estado.
- Define métodos y códigos de estado interoperables.
- HTTPS añade cifrado sobre HTTP.
- Es la base sobre la que se construyen las APIs web.

---

## Fuentes
- Mozilla — *MDN Web Docs: HTTP*: https://developer.mozilla.org/en-US/docs/Web/HTTP
- IETF — *RFC 9110: HTTP Semantics*: https://www.rfc-editor.org/rfc/rfc9110
