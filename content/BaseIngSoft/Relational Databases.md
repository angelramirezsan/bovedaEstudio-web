---
title: "Relational Databases"
type: "technology"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Databases]]"
related:
  - "[[SQL]]"
  - "[[Data Structures and Algorithms]]"
tags:
  - software-engineering
  - datos
---

# Relational Databases

## ¿Qué es?
Una base de datos relacional organiza la información en **tablas** (filas y columnas), donde las tablas se relacionan entre sí. Por ejemplo, una tabla de clientes y otra de pedidos, conectadas por el identificador del cliente.

**Definición técnica:** es un tipo de base de datos basado en el modelo relacional (Codd), donde los datos se representan como relaciones (tablas), con claves primarias y foráneas para vincularlas, y se consultan mediante [[SQL]]. Ofrece garantías transaccionales (ACID).

---

## ¿Por qué existe?
Los datos del mundo real están interconectados (un pedido pertenece a un cliente y contiene productos). El modelo relacional existe para representar esas relaciones sin duplicar información y mantener la consistencia.

---

## ¿Qué problema resuelve?
- Evitar datos duplicados e inconsistentes (normalización).
- Representar relaciones entre entidades de forma explícita.
- Garantizar transacciones fiables (ACID).

---

## ¿Cómo funciona?
Cada tabla tiene una **clave primaria** que identifica cada fila. Las **claves foráneas** apuntan a filas de otras tablas, creando relaciones. Los **índices** aceleran las búsquedas. Las **transacciones** agrupan operaciones que deben cumplirse todas o ninguna (propiedades ACID: Atomicidad, Consistencia, Aislamiento, Durabilidad).

---

## Ejemplo sencillo
Piensa en varias hojas de cálculo vinculadas: una hoja "Clientes" y otra "Pedidos". En vez de repetir el nombre del cliente en cada pedido, guardas su número de ID y las hojas se enlazan. Cambias el nombre una vez y se refleja en todo.

---

## Conceptos relacionados
- [[Databases]] — es una de las familias de bases de datos.
- [[SQL]] — el lenguaje con el que se consultan y modifican.
- [[Data Structures and Algorithms]] — los índices usan estructuras como árboles B para buscar rápido.

---

## Antes de estudiar esto
- [[Databases]]

---

## Después de estudiar esto
- [[SQL]]

---

## Preguntas de comprobación
1. ¿Qué representa una clave foránea?
2. ¿Por qué la normalización evita inconsistencias?
3. ¿Qué garantizan las propiedades ACID?
4. ¿Por qué las tablas se relacionan en lugar de duplicar datos?

---

## Errores comunes
- Duplicar datos en varias tablas en lugar de relacionarlos.
- Pensar que ACID garantiza rendimiento (garantiza consistencia).
- Crear tablas sin claves ni índices y luego sufrir consultas lentas.

---

## Resumen
- Organiza los datos en tablas relacionadas mediante claves.
- Evita duplicación y mantiene consistencia (normalización).
- Ofrece garantías transaccionales ACID.
- Se consulta con SQL.
- Es el modelo más usado en aplicaciones de negocio.

---

## Fuentes
- PostgreSQL Global Development Group — *PostgreSQL Documentation*: https://www.postgresql.org/docs/
- IBM — *What is a Relational Database?*: https://www.ibm.com/topics/relational-databases
