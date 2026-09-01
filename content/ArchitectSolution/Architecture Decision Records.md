---
title: "Architecture Decision Records"
aliases:
  - "ADR"
type: "practice"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Software Architecture]]"
  - "[[Documentation]]"
related:
  - "[[Trade-offs]]"
  - "[[Solution Architecture]]"
tags:
  - solution-architecture
  - decisiones
---

# Architecture Decision Records

## ¿Qué es?
Un ADR (Architecture Decision Record) es un documento corto que registra una decisión importante de arquitectura: qué se decidió, por qué, qué alternativas se consideraron y qué consecuencias tiene. Es la "memoria" de por qué el sistema es como es.

**Definición técnica:** artefacto ligero de documentación que captura una decisión arquitectónica significativa junto con su contexto, las opciones evaluadas, la decisión tomada y sus consecuencias, versionado junto al código.

---

## ¿Por qué existe?
Meses después nadie recuerda por qué se eligió cierta base de datos o cierto estilo. Se repiten debates ya cerrados o se revierten decisiones sin entender sus motivos. Los ADR existen para preservar el razonamiento detrás de las decisiones.

---

## ¿Qué problema resuelve?
- Pérdida del "por qué" detrás de decisiones importantes.
- Repetir debates ya resueltos cuando entra gente nueva.
- Revertir decisiones sin conocer sus consecuencias originales.

---

## ¿Cómo funciona?
Cada ADR es un archivo corto (a menudo Markdown, junto al código) con una estructura típica: **contexto** (situación y fuerzas en juego), **decisión** (qué se eligió), **alternativas consideradas**, **consecuencias** (positivas y negativas, ver [[Trade-offs]]) y **estado** (propuesto, aceptado, obsoleto). Se escriben en el momento de decidir, no después.

---

## Ejemplo sencillo
Es como el acta de una reunión importante: no basta con recordar "decidimos algo"; queda escrito qué se decidió, quiénes participaron, qué se descartó y por qué. Cuando alguien pregunta meses después, la respuesta está documentada.

---

## Conceptos relacionados
- [[Software Architecture]] — los ADR documentan sus decisiones clave.
- [[Documentation]] — es un tipo específico de documentación (de decisiones).
- [[Trade-offs]] — cada decisión implica compromisos que el ADR hace explícitos.
- [[Solution Architecture]] — herramienta central del trabajo del arquitecto.

---

## Antes de estudiar esto
- [[Software Architecture]]
- [[Documentation]]

---

## Después de estudiar esto
- [[Trade-offs]]
- [[Solution Architecture]]

---

## Preguntas de comprobación
1. ¿Qué información captura un ADR?
2. ¿Por qué es importante registrar las alternativas descartadas?
3. ¿Por qué conviene escribir el ADR en el momento de decidir?
4. ¿Cómo ayuda a alguien que se incorpora al equipo?

---

## Errores comunes
- Documentar solo la decisión y omitir el porqué y las alternativas.
- Escribir el ADR mucho después, cuando ya se olvidó el contexto.
- Tratar los ADR como burocracia en lugar de memoria útil del equipo.

---

## Resumen
- Registran decisiones de arquitectura y su razonamiento.
- Incluyen contexto, decisión, alternativas y consecuencias.
- Preservan el "por qué" a lo largo del tiempo.
- Se escriben al decidir y se versionan con el código.
- Hacen explícitos los trade-offs.

---

## Fuentes
- Michael Nygard — *Documenting Architecture Decisions*: https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions
- AWS — *ADR process*: https://docs.aws.amazon.com/prescriptive-guidance/latest/architectural-decision-records/welcome.html
