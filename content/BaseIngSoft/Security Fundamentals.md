---
title: "Security Fundamentals"
type: "concept"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "intermediate"
prerequisites:
  - "[[HTTP]]"
  - "[[Programming Languages]]"
related:
  - "[[Security Architecture]]"
  - "[[API]]"
  - "[[AI Security]]"
tags:
  - software-engineering
  - seguridad
---

# Security Fundamentals

## ¿Qué es?
Los fundamentos de seguridad son los principios básicos para proteger un sistema y sus datos de accesos, usos o daños no autorizados. Es pensar, desde el inicio, en cómo evitar que alguien haga algo que no debería.

**Definición técnica:** conjunto de principios y prácticas para preservar la **confidencialidad, integridad y disponibilidad** (tríada CIA) de la información, mediante autenticación, autorización, cifrado, validación de entradas y gestión de vulnerabilidades.

---

## ¿Por qué existe?
El software maneja datos valiosos y está expuesto a actores maliciosos. Los fallos de seguridad tienen consecuencias graves (fuga de datos, fraude, daño reputacional). Estos fundamentos existen para reducir el riesgo desde el diseño, no como parche final.

---

## ¿Qué problema resuelve?
- Accesos no autorizados a datos o funciones.
- Manipulación o robo de información sensible.
- Vulnerabilidades explotables como inyección o exposición de secretos.

---

## ¿Cómo funciona?
Se apoya en conceptos clave:
- **Autenticación**: verificar quién eres.
- **Autorización**: verificar qué puedes hacer.
- **Cifrado**: proteger datos en tránsito (HTTPS/TLS) y en reposo.
- **Validación de entradas**: no confiar en datos externos (evita inyección, ver [[SQL]]).
- **Principio de mínimo privilegio**: dar solo los permisos necesarios.

Organizaciones como OWASP catalogan los riesgos más frecuentes.

---

## Ejemplo sencillo
Es como la seguridad de un edificio: la entrada con credencial (autenticación), qué pisos puedes visitar (autorización), documentos en caja fuerte (cifrado) y no dejar entrar paquetes sin revisar (validación de entradas).

---

## Conceptos relacionados
- [[HTTP]] — HTTPS/TLS protege la comunicación.
- [[Security Architecture]] — lleva estos fundamentos al nivel de sistema completo.
- [[API]] — las APIs deben autenticar y autorizar cada petición.
- [[AI Security]] — extiende estos principios a los riesgos propios de la IA.

---

## Antes de estudiar esto
- [[HTTP]]
- [[Programming Languages]]

---

## Después de estudiar esto
- [[Security Architecture]]
- [[API]]

---

## Preguntas de comprobación
1. ¿Qué diferencia hay entre autenticación y autorización?
2. ¿Qué protege la tríada CIA (confidencialidad, integridad, disponibilidad)?
3. ¿Por qué nunca se debe confiar en la entrada del usuario?
4. ¿Qué significa el principio de mínimo privilegio?

---

## Errores comunes
- Confundir autenticación con autorización.
- Tratar la seguridad como un paso final en lugar de un requisito de diseño.
- Guardar secretos (contraseñas, tokens) en el código o el repositorio.

---

## Resumen
- La seguridad protege confidencialidad, integridad y disponibilidad.
- Se basa en autenticación, autorización, cifrado y validación.
- Debe pensarse desde el diseño, no como parche.
- El mínimo privilegio reduce la superficie de ataque.
- OWASP documenta los riesgos más comunes.

---

## Fuentes
- OWASP — *OWASP Top Ten*: https://owasp.org/www-project-top-ten/
- NIST — *Cybersecurity Framework*: https://www.nist.gov/cyberframework
- Mozilla — *MDN Web Docs: Web security*: https://developer.mozilla.org/en-US/docs/Web/Security
