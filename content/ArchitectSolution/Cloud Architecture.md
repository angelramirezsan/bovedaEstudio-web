---
title: "Cloud Architecture"
type: "architecture"
area: "Solution Architecture"
level: 5
status: "not-started"
difficulty: "advanced"
prerequisites:
  - "[[Distributed Systems]]"
  - "[[Containers]]"
related:
  - "[[Scalability]]"
  - "[[Deployment]]"
  - "[[Solution Architecture]]"
  - "[[AI Architecture]]"
tags:
  - solution-architecture
  - cloud
---

# Cloud Architecture

## ¿Qué es?
La arquitectura en la nube es el diseño de sistemas que se apoyan en servicios de proveedores de nube (como AWS, Azure o Google Cloud) en lugar de servidores propios. Aprovecha recursos que se pagan por uso y se escalan bajo demanda.

**Definición técnica:** disciplina de diseño de soluciones sobre infraestructura y servicios gestionados de proveedores cloud, aplicando modelos de servicio (IaaS, PaaS, SaaS) y principios de elasticidad, pago por uso y responsabilidad compartida.

---

## ¿Por qué existe?
Comprar y mantener servidores propios es caro, lento de escalar y difícil de dimensionar ante demanda variable. La nube existe para ofrecer infraestructura elástica y servicios gestionados que se consumen como un servicio, reduciendo el peso operativo.

---

## ¿Qué problema resuelve?
- Inversión inicial alta y capacidad fija en servidores propios.
- Lentitud para escalar ante picos de demanda.
- Carga operativa de mantener infraestructura de bajo nivel.

---

## ¿Cómo funciona?
Ofrece servicios en distintos niveles de abstracción:
- **IaaS**: infraestructura básica (máquinas, red, almacenamiento).
- **PaaS**: plataformas gestionadas (bases de datos, colas) sin administrar servidores.
- **SaaS**: software listo para usar.

Aplica **elasticidad** (escalar arriba/abajo automáticamente), **pago por uso** y un **modelo de responsabilidad compartida** (el proveedor asegura la infraestructura; tú, tus datos y configuración). Es el entorno natural de los [[Distributed Systems]] y los [[Containers]].

---

## Ejemplo sencillo
Es como usar electricidad de la red en lugar de tener tu propio generador. No compras ni mantienes la central: pagas por lo que consumes y puedes usar más o menos según lo necesites. La nube es "computación como servicio público".

---

## Conceptos relacionados
- [[Distributed Systems]] — la nube es donde se construyen y operan naturalmente.
- [[Scalability]] — la elasticidad de la nube facilita escalar horizontalmente.
- [[Deployment]] — se despliega sobre servicios cloud.
- [[Solution Architecture]] — la nube es hoy un componente central de casi toda solución.
- [[AI Architecture]] — los servicios de IA suelen consumirse desde la nube.

---

## Antes de estudiar esto
- [[Distributed Systems]]
- [[Containers]]

---

## Después de estudiar esto
- [[Solution Architecture]]
- [[AI Architecture]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre IaaS, PaaS y SaaS?
2. ¿Qué significa "elasticidad" en la nube?
3. ¿Qué implica el modelo de responsabilidad compartida?
4. ¿Por qué el pago por uso cambia la forma de dimensionar sistemas?

---

## Errores comunes
- Asumir que "la nube es responsable de todo", incluida tu configuración y tus datos.
- "Levantar y mover" (lift-and-shift) sin rediseñar y no aprovechar la elasticidad.
- Ignorar costos: la facilidad para crear recursos puede disparar el gasto.

---

## Resumen
- Diseña soluciones sobre servicios gestionados de proveedores cloud.
- Modelos de servicio: IaaS, PaaS, SaaS.
- Principios: elasticidad, pago por uso, responsabilidad compartida.
- Es el entorno natural de sistemas distribuidos y contenedores.
- Componente central de la arquitectura de soluciones moderna.

---

## Fuentes
- AWS — *AWS Well-Architected Framework*: https://aws.amazon.com/architecture/well-architected/
- Microsoft — *Azure Architecture Center*: https://learn.microsoft.com/en-us/azure/architecture/
- Google Cloud — *Cloud Architecture Center*: https://cloud.google.com/architecture
