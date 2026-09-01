---
title: "Documentation"
type: "practice"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Programming Languages]]"
related:
  - "[[Clean Code]]"
  - "[[API]]"
  - "[[Architecture Decision Records]]"
tags:
  - software-engineering
  - comunicacion
---

# Documentation

## ¿Qué es?
La documentación es la información escrita que explica cómo funciona un sistema, cómo usarlo y por qué se tomaron ciertas decisiones. Ayuda a que otras personas (y tú en el futuro) entiendan el software sin tener que leer todo el código.

**Definición técnica:** conjunto de artefactos escritos que describen un sistema desde distintas perspectivas: de usuario, de API, de arquitectura y de decisiones, con el objetivo de transferir conocimiento y reducir la dependencia del conocimiento tácito.

---

## ¿Por qué existe?
El conocimiento que vive solo en la cabeza de las personas se pierde cuando cambian de equipo o de empresa. La documentación existe para preservar y compartir ese conocimiento de forma duradera.

---

## ¿Qué problema resuelve?
- Dependencia de "la única persona que sabe cómo funciona".
- Tiempo perdido reconstruyendo decisiones ya tomadas.
- Dificultad para incorporar nuevas personas al equipo.

---

## ¿Cómo funciona?
Existen tipos según su propósito:
- **De usuario**: cómo usar el producto.
- **De API** ([[API]]): qué endpoints existen y cómo llamarlos.
- **De arquitectura**: cómo está estructurado el sistema.
- **De decisiones** ([[Architecture Decision Records]]): por qué se eligió una opción.

La mejor documentación es la mínima suficiente y que se mantiene actualizada; la desactualizada engaña más que ayuda.

---

## Ejemplo sencillo
Es como el manual de un electrodoméstico: no necesitas entender su ingeniería interna, solo saber cómo usarlo y qué hacer si algo falla. Sin manual, cada persona reinventa el uso por prueba y error.

---

## Conceptos relacionados
- [[Clean Code]] — el código claro reduce la documentación necesaria, pero no la reemplaza del todo.
- [[API]] — su documentación es clave para que otros la consuman.
- [[Architecture Decision Records]] — documentan el porqué de las decisiones.

---

## Antes de estudiar esto
- [[Programming Languages]]

---

## Después de estudiar esto
- [[Architecture Decision Records]]
- [[API]]

---

## Preguntas de comprobación
1. ¿Por qué el conocimiento tácito es un riesgo para un equipo?
2. ¿Qué tipos de documentación existen y para quién es cada uno?
3. ¿Por qué la documentación desactualizada puede ser peor que no tenerla?
4. ¿Cómo se relaciona el código limpio con la documentación?

---

## Errores comunes
- Documentar en exceso lo obvio y no lo importante.
- Dejar que la documentación se desactualice y engañe.
- Confiar solo en el conocimiento tácito de las personas.

---

## Resumen
- La documentación transfiere y preserva conocimiento.
- Reduce la dependencia del conocimiento tácito.
- Hay tipos según propósito: usuario, API, arquitectura, decisiones.
- Debe ser mínima suficiente y estar actualizada.
- El código limpio la complementa, no la sustituye.

---

## Fuentes
- Divio — *The documentation system*: https://documentation.divio.com/
- Write the Docs — *Documentation Guide*: https://www.writethedocs.org/guide/
