---
title: "SQL"
type: "standard"
area: "Software Engineering"
level: 2
status: "not-started"
difficulty: "basic"
prerequisites:
  - "[[Relational Databases]]"
related:
  - "[[Databases]]"
  - "[[Testing]]"
tags:
  - software-engineering
  - datos
---

# SQL

## ¿Qué es?
SQL es el lenguaje con el que le pides información a una base de datos relacional o le indicas que guarde, cambie o borre datos. Es como hacer preguntas y dar órdenes a la base de datos.

**Definición técnica:** SQL (Structured Query Language) es un lenguaje declarativo estandarizado (ISO/IEC 9075) para definir, consultar y manipular datos en sistemas relacionales. Declaras *qué* quieres, no *cómo* obtenerlo; el motor decide el plan de ejecución.

---

## ¿Por qué existe?
Cada base de datos podría tener su propia forma de consultar, lo que sería un caos. SQL existe como lenguaje común y estandarizado para trabajar con datos relacionales, portable entre distintos motores.

---

## ¿Qué problema resuelve?
- Consultar y filtrar datos sin escribir código de bajo nivel.
- Combinar información de varias tablas (JOIN).
- Insertar, actualizar y eliminar datos de forma consistente.

---

## ¿Cómo funciona?
Escribes sentencias declarativas: `SELECT` para consultar, `INSERT`/`UPDATE`/`DELETE` para modificar, `CREATE`/`ALTER` para definir estructura. El motor traduce tu consulta en un **plan de ejecución** optimizado usando índices. Un `JOIN` combina filas de tablas relacionadas.

```sql
SELECT c.nombre, COUNT(p.id) AS total_pedidos
FROM clientes c
JOIN pedidos p ON p.cliente_id = c.id
GROUP BY c.nombre;
```

---

## Ejemplo sencillo
Es como pedir en una biblioteca: "dame todos los libros de ciencia ficción publicados después de 2010, ordenados por autor". No explicas cómo buscarlos; describes el resultado que quieres y el sistema se encarga.

---

## Conceptos relacionados
- [[Relational Databases]] — SQL es su lenguaje natural de consulta.
- [[Databases]] — SQL es el estándar dominante para el modelo relacional.
- [[Testing]] — las consultas también deben probarse y validarse.

---

## Antes de estudiar esto
- [[Relational Databases]]

---

## Después de estudiar esto
- [[API]]
- [[Testing]]

---

## Preguntas de comprobación
1. ¿Qué significa que SQL sea "declarativo"?
2. ¿Para qué sirve un JOIN?
3. ¿Por qué un índice puede acelerar un SELECT?
4. ¿Qué riesgo tiene construir consultas concatenando texto del usuario? (pista: inyección SQL)

---

## Errores comunes
- Construir consultas concatenando entrada del usuario (riesgo de inyección SQL); usar consultas parametrizadas.
- Traer todas las columnas (`SELECT *`) cuando solo se necesitan algunas.
- Olvidar que el orden de resultados no está garantizado sin `ORDER BY`.

---

## Resumen
- SQL es el lenguaje declarativo estándar para bases relacionales.
- Consulta, modifica y define datos de forma portable.
- Los JOIN combinan tablas relacionadas.
- El motor optimiza el plan de ejecución usando índices.
- Las consultas parametrizadas previenen la inyección SQL.

---

## Fuentes
- ISO/IEC — *ISO/IEC 9075 (SQL Standard)*: https://www.iso.org/standard/76583.html
- PostgreSQL Global Development Group — *SQL Language*: https://www.postgresql.org/docs/current/sql.html
- OWASP — *SQL Injection*: https://owasp.org/www-community/attacks/SQL_Injection
