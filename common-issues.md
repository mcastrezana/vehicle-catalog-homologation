# Problemas Comunes en la Homologación de Catálogos Vehiculares

## 📌 Objetivo del documento
Este documento describe **incidencias comunes detectadas en la operación**
relacionadas con la homologación de catálogos vehiculares en entornos
multiaseguradora.

Los ejemplos presentados se basan en **casos reales de operación**, explicados
de forma genérica y con fines demostrativos para portafolio profesional.

---

## 🚗 1. “El vehículo sí existe, pero no cotiza”
### Descripción
Uno de los reclamos más frecuentes es que un vehículo:
- Aparece en el catálogo
- Está correctamente definido
- Pero no genera cotización

### Causa raíz
En muchos casos:
- El catálogo está correcto
- La versión está homologada
- **No existe tarifa disponible o está fuera de reglas de negocio**

### Aprendizaje clave
> La falta de cotización **no siempre es un problema de catálogo**.

Separar catálogo y tarifa permite diagnósticos más rápidos y evita reprocesos.

---

## 🔑 2. Versión sin Clave Interna
### Descripción
Versiones enviadas por la aseguradora que:
- Existen en su catálogo
- Tienen descripción completa
- Pero **no cuentan con Clave Aon**

### Impacto
- No pueden homologarse
- No pueden validarse correctamente
- Bloquean el flujo de cotización

### Resolución
- Asignación de Clave Aon
- Validación de estructura
- Homologación posterior

> Sin clave interna no es posible mantener control ni trazabilidad del catálogo.

---

## 🔁 3. AMIS duplicadas por aseguradora
### Descripción
Algunas aseguradoras cuentan con **más de una clave AMIS para el mismo vehículo**
y modelo (año).

### Regla operativa aplicada
> **Solo se puede homologar una AMIS por cada combinación de:**
> - Clave Aon  
> - Modelo (año / año‑modelo)  
> - Aseguradora  

### Ejemplo conceptual
Una aseguradora puede enviar dos AMIS distintas para un mismo vehículo en el
modelo 2021, mientras que para otros años solo existe una AMIS válida.

En este caso:
- La duplicidad se evalúa únicamente para el modelo 2021
- Se homologa una sola AMIS
- Las AMIS adicionales se excluyen para evitar ambigüedad

### Impacto si no se controla
- Cotizaciones inconsistentes
- Errores en emisión
- Confusión en procesos posteriores

---

## ⏳ 4. Vehículos aún no homologados con una o más aseguradoras
### Descripción
Existen casos en los que un vehículo:
- Ya se encuentra definido en el catálogo interno
- Cuenta con información completa
- **Pero aún no ha sido homologado con todas las aseguradoras**

### Causa raíz
- El proceso de homologación es **100 % manual**
- La carga y validación se realiza por aseguradora
- La homologación se completa de forma progresiva

### Impacto operativo
- El vehículo es visible en el catálogo
- Puede estar homologado con otras aseguradoras
- **Pero no genera cotización con una aseguradora específica**

### Aprendizaje clave
> La ausencia de cotización en estos casos **no representa un error de catálogo**,
> sino un proceso de homologación pendiente.

---

## 🏢 5. Vehículo existente, pero sin cotización por homologación o tarifa
### Descripción
Una situación frecuente ocurre cuando:
- El vehículo existe en el catálogo
- Puede estar homologado con una o más aseguradoras
- **Pero no genera cotización para el negocio específico que se intenta cotizar**

Esto sucede porque **no todos los negocios cotizan con todas las aseguradoras**
disponibles en la plataforma.

---

### Escenarios posibles
Un vehículo puede no cotizar debido a alguno de los siguientes escenarios:

1. ✅ Existe homologación con otras aseguradoras  
   ❌ No existe homologación con la aseguradora activa del negocio

2. ✅ Existe homologación con la aseguradora del negocio  
   ❌ No existe tarifa disponible para esa versión

3. ✅ Existe homologación  
   ❌ La tarifa existe, pero está fuera de reglas de negocio

---

### Contexto operativo
- La plataforma puede contar con múltiples aseguradoras
- Cada negocio trabaja solo con un subconjunto de ellas
- Un mismo vehículo puede:
  - Cotizar con ciertas aseguradoras
  - No cotizar con otras por falta de homologación o tarifa

Es común que los usuarios localicen el vehículo en el catálogo,
pero no obtengan cotización debido a estas condiciones.

---

### Resolución operativa
Para resolver este tipo de casos es necesario identificar la causa real:

- **Si no existe homologación** con la aseguradora del negocio:
  - Confirmar qué aseguradora participa en el negocio
  - Solicitar la clave correspondiente a la aseguradora
  - Completar el proceso de homologación manual

- **Si existe homologación pero no tarifa**:
  - Validar disponibilidad de tarifa
  - Escalar con el área correspondiente
  - Confirmar si la versión está fuera de reglas de negocio

---

### Aprendizaje clave
> La existencia del vehículo en el catálogo **no garantiza cotización**.

La cotización depende de dos factores independientes:
- Homologación con la aseguradora correcta
- Disponibilidad de tarifa válida para el negocio

Separar estos conceptos permite:
- Diagnósticos más claros
- Menos retrabajo operativo
- Comunicación más efectiva con áreas internas y clientes

---

## 📄 6. Duplicados por diferencias mínimas de texto
### Descripción
Versiones que representan el mismo vehículo, pero con:
- Diferencias mínimas en la descripción
- Abreviaturas distintas
- Orden diferente de características

### Riesgo
- Falsa percepción de versiones distintas
- Incremento innecesario del catálogo
- Dificultad en mantenimiento y control

### Buen control
- Análisis por estructura, no solo por texto
- Consolidación lógica de versiones equivalentes

---

## 📅 7. Inconsistencias en modelo (año)
### Descripción
Versiones donde:
- El grupo modelo es correcto
- La versión es válida
- Pero el **año no corresponde**

### Impacto
- Homologaciones incorrectas
- Cotizaciones erróneas
- Problemas en emisión o conciliación

### Prevención
- Validación explícita del modelo (año)
- Revisión de rangos de vigencia
- Controles previos a la homologación

---

## ✅ Conclusión
La mayoría de las incidencias relacionadas con cotización y emisión **no se originan
en el catálogo**, sino en:
- Tarifas
- Reglas de negocio
- Procesos de homologación por aseguradora

Un proceso sólido de homologación permite:
- Diagnósticos más rápidos
- Menos reprocesos
- Mayor estabilidad operativa
- Mejor entendimiento entre áreas técnicas, operativas y de negocio

---

## 📎 Alcance
Los casos descritos representan situaciones comunes en entornos multiaseguradora,
presentadas de forma genérica y con fines demostrativos para portafolio profesional.
