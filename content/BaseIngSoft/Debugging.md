---
title: "Debugging"
type: "practice"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Programming Languages]]"
related:
  - "[[Testing]]"
  - "[[Observability]]"
tags:
  - software-engineering
  - calidad
---

# Debugging

## ¿Qué es?
Debugging (depuración) es el proceso de encontrar y corregir la causa de un fallo en el software. Cuando algo no funciona como debería, depurar es investigar *por qué* ocurre y arreglarlo.

**Definición técnica:** la depuración es la actividad sistemática de localizar, analizar y corregir defectos (bugs) en un programa, formulando y verificando hipótesis sobre la causa raíz del comportamiento incorrecto.

---

## ¿Por qué existe?
El software siempre tiene errores. Saber que algo falla (lo detecta el [[Testing]]) no basta: hay que descubrir la causa exacta. El debugging existe como disciplina para pasar del síntoma a la causa raíz de forma eficiente.

---

## ¿Qué problema resuelve?
- Localizar la causa real de un fallo, no solo el síntoma.
- Reducir el tiempo entre "algo falla" y "está corregido".
- Evitar arreglos superficiales que no atacan el problema de fondo.

---

## ¿Cómo funciona?
Es un método científico aplicado al código:
1. **Reproducir** el fallo de forma fiable.
2. **Observar** el comportamiento (logs, breakpoints, inspección de variables).
3. **Formular una hipótesis** sobre la causa.
4. **Probarla** aislando variables.
5. **Corregir** y verificar que el fallo desaparece sin introducir otros.

Herramientas típicas: depuradores con breakpoints, logs y trazas de [[Observability]].

---

## Ejemplo sencillo
Es como diagnosticar por qué un coche no arranca. No cambias todas las piezas al azar: revisas batería, gasolina, motor de arranque, uno por uno, hasta encontrar la causa. Cambiar cosas sin diagnóstico es caro e ineficaz.

---

## Conceptos relacionados
- [[Testing]] — detecta *que* hay un fallo; el debugging encuentra *por qué*.
- [[Observability]] — logs, métricas y trazas son insumos clave para depurar.
- [[Programming Languages]] — los depuradores dependen del lenguaje y su entorno.

---

## Antes de estudiar esto
- [[Programming Languages]]
- [[Testing]]

---

## Después de estudiar esto
- [[Observability]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre el síntoma de un bug y su causa raíz?
2. ¿Por qué es importante reproducir un fallo antes de arreglarlo?
3. ¿Cómo se relaciona el debugging con la observabilidad?
4. ¿Por qué cambiar código "a ver si se arregla" es una mala estrategia?

---

## Errores comunes
- Arreglar el síntoma sin entender la causa raíz.
- Hacer varios cambios a la vez y no saber cuál solucionó el problema.
- No poder reproducir el fallo y aun así intentar corregirlo.

---

## Resumen
- Depurar es encontrar y corregir la causa de un fallo.
- Es un proceso sistemático de hipótesis y verificación.
- Complementa al testing: uno detecta, el otro diagnostica.
- Se apoya en logs, breakpoints y observabilidad.
- Atacar la causa raíz evita arreglos superficiales.

---

## Fuentes
- Mozilla — *MDN Web Docs: Debugging JavaScript*: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_went_wrong
- Microsoft — *Learn: Debugging*: https://learn.microsoft.com/en-us/visualstudio/debugger/what-is-debugging
