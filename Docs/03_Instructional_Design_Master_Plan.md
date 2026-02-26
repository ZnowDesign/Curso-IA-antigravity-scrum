# 03_Instructional_Design_Master_Plan.md

# Instructional Design Master Plan
## Desarrollo de Software con IA y Agentes Autónomos bajo Scrum

---

# 1. Principios Pedagógicos Fundamentales

## 1.1 Aprendizaje Activo
El estudiante construye conocimiento ejecutando tareas reales:
- Implementación multi‑archivo supervisada
- Diseño arquitectónico con ADRs
- Configuración de pipelines CI
- Supervisión de agentes en producción simulada

**Indicador medible:** ≥ 60% del tiempo total del curso es práctico.

---

## 1.2 Práctica Deliberada
Cada habilidad crítica se practica con intención explícita:
- Redacción de prompts técnicos verificables
- Refactorización guiada
- Diseño de Definition of Done con IA

**Regla:** Ninguna competencia se evalúa sin al menos 2 iteraciones previas.

---

## 1.3 Evaluación Continua
Evaluaciones integradas por sprint:
- Micro‑evaluaciones semanales
- Revisión de PRs
- Validación automatizada en CI
- Retroalimentación estructurada con rúbrica

**Meta:** Feedback ≤ 72 horas después de entrega.

---

# 2. Estrategia Didáctica por Unidad

Modelo base por cada unidad:

1. **Explicación Conceptual (20%)**  
   Marco teórico + riesgos reales.

2. **Demostración Técnica (20%)**  
   Instructor ejecuta flujo real (ej. delegar tarea a agente).

3. **Práctica Guiada (25%)**  
   Estudiantes replican con supervisión.

4. **Práctica Autónoma (25%)**  
   Caso ligeramente distinto sin guión detallado.

5. **Retroalimentación (10%)**  
   Análisis de errores comunes + mejora incremental.

---

# 3. Modelo de Clase Estándar (90 minutos)

| Minutos | Actividad |
|----------|-----------|
| 0–10 | Contexto + objetivo medible |
| 10–25 | Marco conceptual aplicado |
| 25–40 | Demo técnica real |
| 40–65 | Práctica guiada |
| 65–80 | Práctica autónoma |
| 80–90 | Retro + preguntas estratégicas |

---

# 4. Modelo de Taller Intensivo (120 minutos)

| Minutos | Actividad |
|----------|-----------|
| 0–15 | Brief técnico + alcance |
| 15–35 | Diseño previo (plan-first obligatorio) |
| 35–75 | Implementación supervisada con agentes |
| 75–100 | Testing + refactor |
| 100–115 | Presentación técnica |
| 115–120 | Retro estructurada |

---

# 5. Diseño de Laboratorios

## 5.1 Estructura Estándar

### Objetivo
Qué competencia se entrena (ej. CT1, CI1).

### Setup
- Repositorio base
- Branch definida
- Herramientas mínimas

### Pasos
1. Redactar plan técnico
2. Diseñar prompt delegable
3. Ejecutar implementación
4. Validar con tests
5. Refactorizar

### Criterios de Aceptación
- PR limpio
- Tests pasando
- Sin código muerto
- ADR documentado si aplica

### Troubleshooting Común
- Prompt ambiguo
- Sobre-generación de código
- Tests frágiles
- Pipeline mal configurado

---

# 6. Gestión de Cohortes

## 6.1 Dinámica Scrum
Equipos de 3–5 estudiantes.
Roles rotativos cada sprint:
- AI Supervisor
- Scrum Master
- Arquitecto
- Developer

## 6.2 Reglas Anti‑Plagio
- Todo uso de IA debe declararse.
- Se evalúa supervisión, no generación automática.
- Logs de commits obligatorios.

## 6.3 Uso Responsable de IA
- No delegar decisiones críticas sin revisión.
- Validar dependencias OSS.
- No exponer secretos en prompts.

---

# 7. Guía de Prompts Didácticos

## 7.1 Estructura Recomendada

Prompt = Contexto + Tarea + Restricciones + Criterios de aceptación

### Ejemplo
"Actúa como desarrollador senior. Implementa un endpoint REST en Node.js. Restricciones: arquitectura hexagonal, tests con Jest, sin dependencias innecesarias. Debe pasar cobertura ≥ 70%."

## 7.2 Buenas Prácticas
- Siempre incluir criterios de calidad.
- Nunca pedir "haz todo" sin límites.
- Separar planificación de implementación.

---

# 8. Plan de Retroalimentación

## 8.1 Tiempos
- PR revisado ≤ 72h
- Proyecto sprint ≤ 5 días

## 8.2 Formato
- Score técnico (0–5)
- Score arquitectura (0–5)
- Score supervisión IA (0–5)
- Observaciones accionables

## 8.3 Scorecard

| Dimensión | Peso | Puntaje |
|-----------|------|--------|
| Técnica | 30% | /5 |
| Arquitectura | 25% | /5 |
| Supervisión IA | 25% | /5 |
| Scrum y liderazgo | 10% | /5 |
| Ética | 10% | /5 |

---

# 9. Templates

## 9.1 Template – Plan Técnico Pre‑Implementación

```
Objetivo:
Alcance:
Arquitectura propuesta:
Riesgos técnicos:
Criterios de aceptación:
Prompt preliminar:
```

---

## 9.2 Template – ADR

```
Título:
Contexto:
Decisión:
Alternativas evaluadas:
Riesgos:
Impacto:
```

---

## 9.3 Template – Evaluación de PR

```
Calidad código:
Tests:
Cobertura:
Supervisión IA:
Observaciones:
```

---

## 9.4 Template – Retro de Sprint

```
Qué funcionó:
Qué falló:
Errores de supervisión IA:
Acciones de mejora:
```

---

Documento preparado para implementación inmediata en modalidad marketplace y cohorte premium.

