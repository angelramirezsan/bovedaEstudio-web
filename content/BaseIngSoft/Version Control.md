---
title: "Version Control"
type: "practice"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Programming Languages]]"
related:
  - "[[CI-CD]]"
  - "[[Documentation]]"
  - "[[Testing]]"
tags:
  - software-engineering
---

# Version Control

## ¿Qué es?
El control de versiones es un sistema que guarda el historial de cambios de tu código, para que puedas ver qué cambió, quién lo cambió y volver atrás si algo se rompe. Además permite que varias personas trabajen sobre el mismo proyecto sin pisarse.

**Definición técnica:** un sistema de control de versiones (VCS) registra los cambios en un conjunto de archivos a lo largo del tiempo, permitiendo recuperar versiones específicas, ramificar líneas de trabajo (branching) y fusionarlas (merging). Git es el sistema distribuido más extendido.

---

## ¿Por qué existe?
Antes se copiaban carpetas con nombres como `proyecto_final_v2_definitivo`. Eso no escala, pierde historial y hace imposible colaborar. El control de versiones existe para dar trazabilidad, colaboración segura y capacidad de deshacer.

---

## ¿Qué problema resuelve?
- Perder trabajo o no poder volver a un estado anterior.
- Conflictos al trabajar varias personas sobre el mismo archivo.
- Falta de trazabilidad sobre por qué y cuándo cambió algo.

---

## ¿Cómo funciona?
Cada cambio confirmado (**commit**) queda registrado con autor, fecha y mensaje. Las **ramas (branches)** permiten trabajar en paralelo sin afectar la línea principal; luego se integran mediante **merge**. En sistemas distribuidos como Git, cada persona tiene una copia completa del historial, y se sincroniza con un repositorio remoto (ej. en plataformas como GitHub o GitLab).

---

## Ejemplo sencillo
Es como los puntos de guardado de un videojuego: si tomas una mala decisión, recargas desde un punto anterior. Y si varios amigos juegan la misma partida en sus propias copias, luego juntan sus avances.

---

## Conceptos relacionados
- [[CI-CD]] — los pipelines se disparan a partir de cambios en el control de versiones.
- [[Documentation]] — los mensajes de commit y los cambios documentan la evolución.
- [[Testing]] — las pruebas suelen ejecutarse automáticamente sobre cada cambio.

---

## Antes de estudiar esto
- [[Programming Languages]]

---

## Después de estudiar esto
- [[CI-CD]]
- [[Testing]]

---

## Preguntas de comprobación
1. ¿Qué problema resuelve el control de versiones frente a copiar carpetas?
2. ¿Para qué sirve una rama (branch)?
3. ¿Qué significa que Git sea "distribuido"?
4. ¿Por qué un buen mensaje de commit es valioso a largo plazo?

---

## Errores comunes
- Hacer commits enormes que mezclan muchos cambios sin relación.
- Escribir mensajes de commit vacíos o poco descriptivos.
- Trabajar siempre en la rama principal sin aislar el trabajo en curso.

---

## Resumen
- El control de versiones guarda el historial de cambios del código.
- Permite volver atrás, colaborar y auditar la evolución.
- Git es el estándar distribuido actual.
- Las ramas aíslan el trabajo; el merge lo integra.
- Es la base de la colaboración y de la automatización moderna.

---

## Fuentes
- Software Freedom Conservancy — *Git Documentation*: https://git-scm.com/doc
- Git — *Pro Git Book*: https://git-scm.com/book/en/v2
