---
title: "Databases"
type: "concept"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Data Structures and Algorithms]]"
related:
  - "[[Relational Databases]]"
  - "[[SQL]]"
  - "[[Vector Databases]]"
tags:
  - software-engineering
  - datos
---

# Databases

## ¿Qué es?
Una base de datos es un sistema para almacenar información de forma organizada y poder recuperarla de manera confiable y eficiente. Es donde vive el dato persistente de una aplicación (usuarios, pedidos, mensajes).

**Definición técnica:** una base de datos es una colección organizada de datos gestionada por un sistema gestor (DBMS) que garantiza almacenamiento, consulta, actualización, integridad y control de acceso concurrente.

---

## ¿Por qué existe?
Guardar datos en archivos sueltos no escala: es difícil buscar, evitar duplicados, mantener consistencia y controlar accesos simultáneos. Las bases de datos existen para gestionar datos de forma fiable a gran escala y con muchos usuarios a la vez.

---

## ¿Qué problema resuelve?
- Persistir datos más allá del tiempo de vida de un programa.
- Consultar y filtrar grandes volúmenes de forma eficiente.
- Mantener integridad y consistencia con accesos concurrentes.

---

## ¿Cómo funciona?
Existen varias familias según cómo modelan los datos:
- **Relacionales** ([[Relational Databases]]): datos en tablas con relaciones, consultadas con [[SQL]].
- **NoSQL**: documentos, clave-valor, grafos o columnas, para casos donde la flexibilidad o la escala importan más que el modelo tabular.
- **Vectoriales** ([[Vector Databases]]): almacenan representaciones numéricas para búsqueda por similitud, clave en IA.

El DBMS gestiona índices para buscar rápido, transacciones para garantizar consistencia y control de concurrencia.

---

## Ejemplo sencillo
Es como una biblioteca bien organizada: los libros (datos) están catalogados e indexados, puedes encontrar uno en segundos, hay reglas de préstamo (integridad) y varias personas pueden consultar el catálogo a la vez sin caos.

---

## Conceptos relacionados
- [[Relational Databases]] — la familia más común, base del modelo tabular.
- [[SQL]] — el lenguaje estándar para consultar bases relacionales.
- [[Vector Databases]] — variante especializada para IA y búsqueda semántica.

---

## Antes de estudiar esto
- [[Data Structures and Algorithms]]

---

## Después de estudiar esto
- [[Relational Databases]]
- [[SQL]]

---

## Preguntas de comprobación
1. ¿Por qué no basta con guardar datos en archivos de texto?
2. ¿Qué diferencia hay entre una base relacional y una NoSQL a nivel conceptual?
3. ¿Qué papel juega un índice en el rendimiento de una consulta?
4. ¿En qué caso usarías una base de datos vectorial?

---

## Errores comunes
- Elegir NoSQL "porque es moderno" sin que el problema lo justifique.
- Ignorar los índices y luego culpar a la base de datos por la lentitud.
- Confundir la base de datos (el sistema) con el modelo de datos (cómo se organiza).

---

## Resumen
- Una base de datos almacena y recupera información de forma fiable y eficiente.
- Existen familias: relacionales, NoSQL y vectoriales, entre otras.
- El DBMS gestiona índices, transacciones y concurrencia.
- La elección depende del patrón de acceso y del problema.
- Es el hogar del dato persistente de casi todo sistema.

---

## Fuentes
- PostgreSQL Global Development Group — *PostgreSQL Documentation*: https://www.postgresql.org/docs/
- Microsoft — *Learn: Databases*: https://learn.microsoft.com/en-us/training/paths/azure-fundamentals-describe-azure-database-services/
- MongoDB — *What Is a Database?*: https://www.mongodb.com/resources/basics/databases
