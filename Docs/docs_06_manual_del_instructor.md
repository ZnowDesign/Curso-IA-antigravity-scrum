# 06_Manual_del_Instructor.md

# Manual del Instructor
## Desarrollo de Software con IA y Agentes Autónomos bajo Scrum

---

# 1. Propósito del Manual

Este documento garantiza consistencia académica, calidad técnica y estandarización en la impartición del curso, independientemente del instructor o modalidad.

El enfoque es:
- Profesional avanzado
- Orientado a mercado real
- Basado en evidencia técnica verificable
- Centrado en supervisión de agentes IA

---

# 2. Guía de Facilitación por Unidad

## Unidad 1 – Fundamentos de AI‑Augmented Engineering

### Objetivos
- Comprender el cambio de paradigma Developer → AI Supervisor.
- Identificar riesgos y límites reales de agentes.

### Agenda Sugerida (90 min)
- 20 min: Marco conceptual
- 20 min: Demo supervisión real de agente
- 30 min: Práctica guiada de prompt estructurado
- 20 min: Retroalimentación

### Puntos Críticos
- Evitar visión “IA hace todo”.
- Insistir en validación humana.

### Demo Sugerido
- Generación de módulo simple + corrección estructural.

---

## Unidad 2 – Scrum + Agentes

### Objetivos
- Integrar eventos Scrum con delegación controlada.

### Demo
- Generación de backlog usando agente + refinamiento manual.

### Punto Crítico
- Diferenciar automatización de liderazgo.

---

## Unidad 3 – Arquitectura con IA

### Objetivos
- Aplicar ADRs antes de delegar implementación.

### Demo
- Creación de ADR y evaluación de trade‑offs.

### Error Común
- Delegar arquitectura sin análisis previo.

---

## Unidad 4 – Implementación Supervisada

### Objetivos
- Generar código multi‑archivo con control de alcance.

### Demo
- Prompt estructurado + revisión PR.

### Error Común
- Prompt ambiguo sin criterios de aceptación.

---

## Unidad 5 – Testing y CI/CD con IA

### Objetivos
- Validar código generado mediante tests y pipeline.

### Demo
- Generación de tests + ejecución CI.

### Error Común
- Confiar en tests generados sin revisión.

---

## Unidad 6 – Gobernanza y Seguridad

### Objetivos
- Aplicar políticas de uso responsable.

### Demo
- Checklist de riesgos IA.

---

## Unidad 7 – Liderazgo Técnico AI‑Augmented

### Objetivos
- Medir productividad real vs ilusión de productividad.

### Actividad
- Análisis métricas sprint.

---

## Unidad 8 – Gestión de Proyecto con IA

### Objetivos
- Integrar agentes en planificación sin perder control humano.

---

## Unidad 9 – Capstone

### Objetivos
- Integrar arquitectura, implementación y supervisión.

---

# 3. Preguntas Detonadoras

- ¿Qué parte de esta tarea NO debería delegarse a un agente?
- ¿Cómo validas que el código generado es seguro?
- ¿Qué riesgos arquitectónicos no detecta la IA?
- ¿Qué métrica demuestra mejora real?

---

# 4. Errores Comunes del Alumno y Corrección

| Error | Causa | Estrategia de Corrección |
|-------|-------|-------------------------|
| Prompt genérico | Falta de restricciones | Forzar plantilla estructurada |
| Confianza ciega en IA | Falta de testing | Exigir cobertura mínima |
| Arquitectura improvisada | No usar ADR | Evaluación obligatoria de diseño |
| Uso excesivo de copy‑paste | Falta de comprensión | Defensa técnica oral |

---

# 5. Evaluación de Prompts sin Sesgo

## Criterios Objetivos
- Claridad de contexto
- Restricciones técnicas explícitas
- Criterios de aceptación definidos
- Reproducibilidad del resultado

No se evalúa creatividad literaria; se evalúa precisión técnica.

---

# 6. Guía de Evaluación Rápida (Checkpoints por Sesión)

| Checkpoint | Evidencia |
|------------|----------|
| Plan previo a delegar | Documento breve |
| Prompt estructurado | Texto versionado |
| Tests ejecutados | Pipeline verde |
| Corrección documentada | PR comentado |

---

# 7. Modalidad Online – Recomendaciones

## Gestión de Tiempo
- Bloques de 20 min máximo por explicación.
- Alternar teoría y ejecución.

## Breakout Rooms
- Equipos Scrum fijos.
- Roles rotativos.

## Herramientas
- Repositorio compartido
- CI visible en tiempo real
- Pizarra digital para ADRs

---

# 8. Librería de Ejemplos

## 8.1 Prompt Técnico Base

"Actúa como desarrollador senior. Implementa endpoint REST en Node.js. Restricciones: arquitectura hexagonal, tests Jest ≥70% coverage, sin dependencias innecesarias. Entrega código modular."

---

## 8.2 Historia Scrum

Como usuario autenticado
Quiero crear una orden
Para registrar una compra correctamente

Criterios de aceptación:
- Persistencia correcta
- Validación de datos
- Test unitario incluido

---

## 8.3 Definition of Ready

- Historia clara
- Criterios de aceptación definidos
- Dependencias identificadas

---

## 8.4 Definition of Done

- Tests ≥70%
- Pipeline exitoso
- Código revisado
- Documentación actualizada

---

Manual listo para implementación consistente en modalidad presencial, online y corporativa.

