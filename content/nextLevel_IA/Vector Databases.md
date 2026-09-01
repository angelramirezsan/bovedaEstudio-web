---
title: "Vector Databases"
type: "technology"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Embeddings]]"
  - "[[Databases]]"
related:
  - "[[RAG]]"
  - "[[Large Language Models]]"
tags:
  - ai
  - datos
---

# Vector Databases

## ¿Qué es?
Una base de datos vectorial es una base de datos especializada en guardar y buscar [[Embeddings]] (los vectores que representan significado). Su superpoder es encontrar rápidamente los elementos "más parecidos" a uno dado.

**Definición técnica:** sistema de almacenamiento optimizado para vectores de alta dimensión que implementa búsqueda por similitud (habitualmente ANN, *approximate nearest neighbor*) para recuperar los elementos semánticamente más cercanos a una consulta.

---

## ¿Por qué existe?
Las bases de datos tradicionales ([[Relational Databases]]) buscan por coincidencia exacta o por rangos, no por *similitud de significado*. Con la IA surgió la necesidad de buscar "lo más parecido" entre millones de vectores de forma eficiente. Las bases vectoriales existen para eso.

---

## ¿Qué problema resuelve?
- Buscar por significado (semántica) y no por coincidencia exacta.
- Encontrar los elementos más similares entre millones de vectores rápidamente.
- Dar "memoria" y contexto recuperable a sistemas de IA como [[RAG]].

---

## ¿Cómo funciona?
Guarda embeddings junto con sus datos originales. Ante una consulta, convierte la pregunta en un embedding y busca los vectores más cercanos usando algoritmos de vecino más cercano aproximado (ANN), que sacrifican algo de exactitud por muchísima velocidad. Es una pieza clave del patrón [[RAG]] y complementa (no sustituye) a las bases de datos tradicionales.

---

## Ejemplo sencillo
Es como un bibliotecario que, en vez de buscar por título exacto, entiende de qué trata tu pregunta y te trae los libros más relacionados por tema, aunque no compartan ni una palabra en el título. Busca por sentido, no por coincidencia literal.

---

## Conceptos relacionados
- [[Embeddings]] — lo que estas bases almacenan y comparan.
- [[Databases]] — son una familia especializada de bases de datos.
- [[RAG]] — las usa para recuperar contexto relevante.
- [[Large Language Models]] — se apoyan en ellas para acceder a conocimiento externo.

---

## Antes de estudiar esto
- [[Embeddings]]
- [[Databases]]

---

## Después de estudiar esto
- [[RAG]]

---

## Preguntas de comprobación
1. ¿En qué se diferencia buscar en una base vectorial frente a una relacional?
2. ¿Qué significa búsqueda por "vecino más cercano aproximado" (ANN)?
3. ¿Por qué son clave para RAG?
4. ¿Sustituyen a las bases de datos tradicionales? ¿Por qué?

---

## Errores comunes
- Creer que reemplazan a las bases relacionales (las complementan).
- Ignorar que la búsqueda ANN es aproximada, no exacta.
- Mezclar embeddings de modelos distintos, que no son comparables.

---

## Resumen
- Almacenan y buscan embeddings por similitud de significado.
- Usan búsqueda por vecino más cercano aproximado (ANN).
- Habilitan la búsqueda semántica a gran escala.
- Son una pieza central del patrón RAG.
- Complementan, no sustituyen, a las bases tradicionales.

---

## Fuentes
- Microsoft — *Learn: Vector databases*: https://learn.microsoft.com/en-us/azure/cosmos-db/vector-database
- PostgreSQL — *pgvector extension*: https://github.com/pgvector/pgvector
- AWS — *What is a vector database?*: https://aws.amazon.com/what-is/vector-databases/
