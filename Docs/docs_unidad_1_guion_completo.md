# Unidad 1 – AI-Augmented Engineering: Fundamentos y Cambio de Paradigma
## Desarrollo de Software con IA y Agentes Autónomos bajo Scrum

---

# 1. Ficha Técnica

Duración total sugerida: 3–4 horas

- Teoría: 60 min
- Demo técnica: 45 min
- Práctica guiada: 60 min
- Práctica autónoma: 45 min
- Retroalimentación: 30 min

Competencias asociadas:
- CT1 (Implementación supervisada)
- CI1 (Diseño de prompts técnicos)
- CI2 (Detección de errores IA)
- CL1 (Visión estratégica)

Nivel Bloom esperado: Analizar / Evaluar

---

# 2. Objetivos Medibles

Al finalizar la unidad, el estudiante será capaz de:

1. Explicar técnicamente la diferencia entre uso básico de IA y supervisión estratégica.
2. Diseñar un prompt estructurado con restricciones y criterios de aceptación.
3. Detectar errores estructurales en código generado por IA.
4. Aplicar un proceso plan-first antes de delegar implementación.

---

# 3. Marco Conceptual

## 3.1 Cambio de Paradigma

Antes:
Developer escribe código línea por línea.

Ahora:
Developer supervisa generación automatizada.

Nuevo rol: AI-Augmented Engineer.

---

## 3.2 Productividad Real vs Falsa Productividad

Falsa productividad:
- Código rápido
- Sin tests
- Sin arquitectura
- Sin CI

Productividad real:
- Código validado
- Coverage mínimo
- ADR documentado
- Pipeline exitoso

---

## 3.3 Riesgos Técnicos del Uso No Supervisado

- Código duplicado
- Violación de principios SOLID
- Vulnerabilidades
- Dependencias innecesarias
- Deuda técnica acelerada

---

## 3.4 Introducción a Antigravity

Concepto central:
No delegar implementación sin plan.

Flujo Antigravity básico:
1. Definir alcance.
2. Diseñar plan técnico.
3. Redactar prompt con restricciones.
4. Generar.
5. Validar.
6. Corregir.

---

# 4. Demo Técnica Obligatoria

## Escenario

Implementar función en Node.js que calcule total de orden con validaciones.

## Paso 1 – Plan Técnico

- Inputs esperados
- Validaciones necesarias
- Estructura modular

## Paso 2 – Prompt Estructurado

"Actúa como desarrollador senior. Implementa función calculateOrderTotal. Restricciones: validar tipos, sin dependencias externas, incluir tests con Jest, coverage mínimo 70%."

## Paso 3 – Generación

Revisión inmediata:
- ¿Cumple restricciones?
- ¿Incluye tests?
- ¿Respeta modularidad?

## Paso 4 – Validación

Ejecutar tests.
Revisar lint.

---

# 5. Laboratorio Guiado

## Objetivo

Aplicar proceso plan-first y delegación controlada.

## Setup

- Repo base proporcionado.
- Node.js 18+.
- Jest configurado.

## Actividad

Implementar módulo "userValidation" con:
- Validación email
- Validación password
- Tests unitarios

## Criterios de Aceptación

- Coverage ≥70%.
- Sin errores lint.
- Prompt documentado.

---

# 6. Práctica Autónoma

Escenario distinto:

Crear módulo "discountEngine" con reglas condicionales.

Debe incluir:
- Plan previo documentado.
- Prompt estructurado.
- Validación automatizada.

---

# 7. Integración con Scrum

Artefactos asociados:

Historia de usuario ejemplo:

Como usuario autenticado
Quiero calcular total correctamente
Para visualizar el monto final exacto

Definition of Done:
- Tests ≥70%
- Sin errores críticos
- Código revisado

---

# 8. Evaluación

Tipo: Formativa

Instrumento: Rúbrica laboratorio nivel 1–4

Quality Gates:
- Coverage ≥70%
- CI verde

---

# 9. Errores Comunes

| Error | Corrección |
|-------|------------|
| Prompt ambiguo | Forzar restricciones explícitas |
| Código sin tests | Exigir coverage mínimo |
| Generación masiva sin revisión | Dividir en tareas pequeñas |

---

# 10. Preguntas Detonadoras

- ¿Qué parte de esta tarea NO delegarías?
- ¿Cómo sabes que el código es seguro?
- ¿Qué validación no detecta automáticamente la IA?

---

# 11. Resultado Esperado

El estudiante entiende que la IA no reemplaza criterio técnico.
La supervisión es la competencia clave.

---

Unidad lista para producción de slides y grabación.

