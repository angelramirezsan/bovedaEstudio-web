---
title: "Embeddings"
type: "concept"
area: "AI / Next Generation"
level: 6
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Machine Learning]]"
related:
  - "[[Vector Databases]]"
  - "[[RAG]]"
  - "[[Large Language Models]]"
tags:
  - ai
---

# Embeddings

## ¿Qué es?
Un embedding es una forma de representar un dato (una palabra, una frase, una imagen) como una lista de números que captura su *significado*. Datos con significado parecido tienen números parecidos, así la computadora puede medir "qué tan similares son".

**Definición técnica:** representación vectorial densa de un objeto en un espacio multidimensional, aprendida por un modelo, en la que la proximidad geométrica entre vectores refleja similitud semántica.

---

## ¿Por qué existe?
Las computadoras no entienden texto ni imágenes directamente; necesitan números. Y no cualquier número: uno que capture el significado, para poder comparar por sentido y no solo por coincidencia exacta de palabras. Los embeddings existen para eso.

---

## ¿Qué problema resuelve?
- Comparar cosas por significado, no por coincidencia literal de texto.
- Buscar contenido "parecido" aunque use palabras distintas (búsqueda semántica).
- Alimentar tareas de IA que requieren representar el significado.

---

## ¿Cómo funciona?
Un modelo convierte cada dato en un **vector** (lista de números). "Perro" y "cachorro" quedan cerca; "perro" y "avión", lejos. La cercanía se mide con distancias (ej. similitud del coseno). Estos vectores se guardan y consultan en una [[Vector Databases]], y son la base técnica de la búsqueda semántica que usa [[RAG]].

---

## Ejemplo sencillo
Imagina un mapa donde cada palabra es un punto. Palabras relacionadas ("médico", "hospital", "enfermera") están en el mismo barrio; palabras sin relación, en ciudades distintas. Buscar por significado es mirar qué hay cerca en ese mapa, aunque no compartan letras.

---

## Conceptos relacionados
- [[Machine Learning]] — los embeddings son representaciones aprendidas por modelos.
- [[Vector Databases]] — almacenan y buscan embeddings eficientemente.
- [[RAG]] — usa embeddings para encontrar información relevante.
- [[Large Language Models]] — internamente representan el texto con embeddings.

---

## Antes de estudiar esto
- [[Machine Learning]]

---

## Después de estudiar esto
- [[Vector Databases]]
- [[RAG]]

---

## Preguntas de comprobación
1. ¿Qué captura un embedding además de los datos en sí?
2. ¿Por qué se dice que permiten "búsqueda semántica"?
3. ¿Cómo se mide la similitud entre dos embeddings?
4. ¿Qué relación tienen con las bases de datos vectoriales?

---

## Errores comunes
- Pensar que un embedding es solo "codificar texto" (captura significado, no forma).
- Comparar embeddings de modelos distintos como si fueran compatibles.
- Ignorar que la calidad del embedding depende del modelo que lo genera.

---

## Resumen
- Representan datos como vectores que capturan significado.
- Datos similares quedan cerca en el espacio vectorial.
- Habilitan la búsqueda semántica (por sentido, no por palabra exacta).
- Se almacenan y consultan en bases de datos vectoriales.
- Son la base técnica de RAG y de los LLM.

---

## Fuentes
- Google — *Machine Learning: Embeddings*: https://developers.google.com/machine-learning/crash-course/embeddings
- Microsoft — *Learn: Understand embeddings*: https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/understand-embeddings
