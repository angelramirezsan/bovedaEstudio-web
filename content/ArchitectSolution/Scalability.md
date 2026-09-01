---
title: "Scalability"
type: "concept"
area: "Solution Architecture"
level: 4
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[Non-Functional Requirements]]"
  - "[[Distributed Systems]]"
related:
  - "[[Availability]]"
  - "[[Cloud Architecture]]"
  - "[[Data Structures and Algorithms]]"
tags:
  - solution-architecture
  - atributo-calidad
---

# Scalability

## ¿Qué es?
La escalabilidad es la capacidad de un sistema para manejar más trabajo (más usuarios, más datos, más peticiones) sin degradarse, agregando recursos. Un sistema escalable crece con la demanda.

**Definición técnica:** atributo de calidad que mide la capacidad de un sistema de mantener o mejorar su rendimiento al aumentar la carga, mediante escalado vertical (más recursos por nodo) u horizontal (más nodos).

---

## ¿Por qué existe?
La demanda no es constante: una app puede pasar de cientos a millones de usuarios. Si el sistema no escala, colapsa justo cuando más se usa. La escalabilidad existe para que el crecimiento sea una oportunidad y no una crisis.

---

## ¿Qué problema resuelve?
- Caídas o lentitud cuando aumenta la demanda.
- Costos ineficientes por sobredimensionar "por si acaso".
- Incapacidad de aprovechar picos de tráfico (ofertas, virales).

---

## ¿Cómo funciona?
Hay dos formas principales:
- **Vertical (scale up)**: hacer más potente una máquina. Simple, pero con techo.
- **Horizontal (scale out)**: añadir más máquinas y repartir la carga (load balancing). Es la base de los [[Distributed Systems]] y la [[Cloud Architecture]].

El escalado horizontal requiere que el sistema sea "stateless" o gestione el estado con cuidado. La eficiencia algorítmica ([[Data Structures and Algorithms]]) también afecta cuánto necesitas escalar.

---

## Ejemplo sencillo
Un restaurante puede atender más clientes de dos formas: contratar un cocinero más rápido y una cocina más grande (vertical), o abrir más sucursales con su propia cocina (horizontal). La segunda escala casi sin límite, pero exige coordinación.

---

## Conceptos relacionados
- [[Non-Functional Requirements]] — la escalabilidad es uno de ellos.
- [[Availability]] — escalar bien contribuye a mantener el servicio disponible.
- [[Cloud Architecture]] — facilita escalar horizontalmente bajo demanda.
- [[Data Structures and Algorithms]] — código eficiente reduce la necesidad de escalar.

---

## Antes de estudiar esto
- [[Non-Functional Requirements]]
- [[Distributed Systems]]

---

## Después de estudiar esto
- [[Availability]]
- [[Cloud Architecture]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre escalado vertical y horizontal?
2. ¿Por qué el escalado horizontal suele requerir servicios "stateless"?
3. ¿Cómo se relaciona la eficiencia algorítmica con la necesidad de escalar?
4. ¿Por qué sobredimensionar "por si acaso" puede ser un problema?

---

## Errores comunes
- Confundir escalabilidad con rendimiento; un sistema rápido puede no escalar.
- Asumir que añadir máquinas siempre mejora (a veces el cuello de botella es la base de datos).
- Diseñar con estado en memoria que impide escalar horizontalmente.

---

## Resumen
- Es la capacidad de manejar más carga agregando recursos.
- Puede ser vertical (más potente) u horizontal (más nodos).
- El escalado horizontal es la base de los sistemas distribuidos y la nube.
- Requiere diseñar pensando en el estado.
- Es un requisito no funcional clave.

---

## Fuentes
- AWS — *Well-Architected Framework: Performance Efficiency*: https://docs.aws.amazon.com/wellarchitected/latest/performance-efficiency-pillar/welcome.html
- Microsoft — *Azure Architecture Center: Scalability*: https://learn.microsoft.com/en-us/azure/architecture/framework/scalability/
