# Reglas de Homologación de Catálogos Vehiculares

## 📌 Objetivo del documento
Este documento describe las **reglas conceptuales y operativas de homologación**
entre un catálogo vehicular interno y los catálogos proporcionados por las aseguradoras.

El proceso de homologación tiene como objetivo garantizar **control, trazabilidad
y consistencia del catálogo**, asegurando que cada versión vehicular esté correctamente
identificada mediante una clave interna única.

Las reglas aquí descritas están basadas en **experiencia operativa real** y se presentan
de forma generalizada para fines de portafolio profesional.

---

## 🧩 ¿Qué es la homologación?
La homologación es el proceso mediante el cual una **versión vehicular proveniente
del catálogo de una aseguradora** se asocia a una **clave interna (Clave Aon)** utilizada
por la plataforma o área operativa.

Este proceso permite:
- Mantener un catálogo interno completo y controlado
- Unificar criterios entre múltiples aseguradoras
- Evitar ambigüedad en la identificación de vehículos
- Facilitar validaciones operativas posteriores
- Separar claramente catálogo, reglas de negocio y tarifa

---

## ✅ Alcance real de la Homologación
En la operación real, el criterio general es:

> **Todas las versiones vehiculares proporcionadas por la aseguradora deben ser homologadas**,  
> aun cuando no todas sean cotizables.

La homologación **no filtra versiones por criterios comerciales**.
La exclusión de cotización depende de:
- Disponibilidad de tarifa
- Reglas de negocio
- Restricciones técnicas o comerciales

Este enfoque garantiza que el catálogo interno:
- Esté completo
- Sea trazable
- Permita un diagnóstico claro ante incidencias

---

## 🔑 Condiciones para homologar una versión
Una versión vehicular puede ser homologada cuando:

- Existe correspondencia clara entre:
  - Marca
  - Grupo modelo (familia comercial)
  - Modelo (año / año‑modelo)
  - Versión
- Cuenta con una **Clave Interna (Clave Aon)** válida
- No genera ambigüedad dentro del catálogo interno
- Cumple con los criterios mínimos de calidad del dato

> La existencia de la Clave Aon es indispensable para el control del catálogo,
> independientemente de que la versión cotice o no.

---

## 🚫 Manejo de AMIS duplicadas por aseguradora
En algunos casos, las aseguradoras pueden contar con **más de una clave AMIS**
para el mismo vehículo.

Para evitar duplicidad y ambigüedad operativa, se aplica la siguiente regla:

> **Solo se puede homologar una AMIS por cada combinación de:**
> - Clave Aon  
> - Modelo (año / año‑modelo)  
> - Aseguradora  

---

## 🔍 Aplicación de la regla de AMIS duplicadas
Cuando una aseguradora envía más de una AMIS para el mismo vehículo:

- Se identifica el conjunto de AMIS duplicadas
- Se valida que correspondan a la misma:
  - Marca
  - Grupo modelo
  - Modelo (año)
- **Se selecciona únicamente una AMIS para homologar**
- Las AMIS adicionales se excluyen para evitar duplicidad

Esta validación se realiza **por modelo (año)**, no de forma global para todo el vehículo.

---

## 🧠 Ejemplo conceptual
Una aseguradora puede contar con dos AMIS distintas para un mismo vehículo en el
modelo 2021, mientras que para otros años solo existe una AMIS válida.

En este escenario:
- La duplicidad **solo aplica al modelo 2021**
- Se homologa una sola AMIS para ese año
- Los demás modelos se procesan de forma independiente

Esto permite mantener consistencia, control y claridad en el catálogo.

---

## ⚠️ Homologación vs Cotización
Un principio fundamental es que:

> **Homologar una versión no implica que esa versión deba cotizar**

Una versión homologada puede no cotizar cuando:
- No existe tarifa asociada
- Se encuentra fuera de reglas de negocio
- Tiene restricciones comerciales o técnicas

La homologación asegura:
- Control del catálogo
- Identificación única
- Trazabilidad

Mientras que la cotización depende de capas posteriores al catálogo.

Separar estos conceptos evita:
- Confusión en el análisis de incidencias
- Retrabajo operativo
- Diagnósticos incorrectos de “faltantes de catálogo”

---

## 🔄 Mantenimiento de la Homologación
La homologación es un proceso dinámico que debe contemplar:

- Altas de nuevas versiones
- Cambios en versiones existentes
- Revisión de AMIS duplicadas
- Depuración de versiones obsoletas
- Validación periódica de consistencia

Un mantenimiento continuo reduce errores recurrentes en los procesos de cotización y emisión.

---

## ✅ Buenas Prácticas
- Homologar el catálogo completo por aseguradora
- Aplicar reglas de duplicidad por modelo (año)
- Mantener una relación clara uno a uno entre versión y Clave Aon
- Documentar criterios de selección de AMIS
- Distinguir claramente catálogo, reglas de negocio y tarifa
- Priorizar consistencia y control sobre filtrado de versiones

---

## 📎 Alcance del Documento
Este documento describe **reglas conceptuales y operativas** aplicables a entornos
multiaseguradora.

No representa la implementación de ningún sistema productivo específico.
Todos los ejemplos se presentan con fines demostrativos y de portafolio profesional.
