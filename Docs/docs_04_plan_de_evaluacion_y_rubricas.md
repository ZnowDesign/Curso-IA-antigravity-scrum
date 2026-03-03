# 04_Plan_de_Evaluacion_y_Rubricas.md

# Plan de Evaluación y Rúbricas
## Desarrollo de Software con IA y Agentes Autónomos bajo Scrum

---

# 1. Modelo Integral de Evaluación

El sistema de evaluación es **competencial, incremental y basado en evidencia verificable en repositorio y pipeline CI/CD**.

Se compone de tres capas:

1. **Evaluación Diagnóstica** → determina punto de partida.
2. **Evaluación Formativa** → mejora continua por sprint.
3. **Evaluación Sumativa** → certifica dominio profesional.

Todas las evaluaciones miden explícitamente:
- Calidad técnica
- Arquitectura
- Supervisión de agentes IA
- Gobernanza y ética
- Trabajo ágil bajo Scrum

---

# 2. Evaluación Diagnóstica

## Objetivo
Determinar nivel inicial en:
- Programación estructurada y modular
- Testing automatizado
- Uso práctico de herramientas IA
- Comprensión real de Scrum

## Instrumentos

| Instrumento | Duración | Evidencia Medible | Criterio de Análisis |
|-------------|----------|------------------|---------------------|
| Mini‑Proyecto Técnico | 2 h | Repo funcional + commits | Calidad estructural + pruebas |
| Cuestionario Técnico | 45 min | Resultados automatizados | ≥70% correcto = intermedio |
| Autoevaluación IA | 20 min | Declaración estructurada | Coherencia técnica |

Clasificación resultante:
- Básico
- Intermedio
- Avanzado

No impacta nota final, pero ajusta nivel de exigencia.

---

# 3. Evaluación Formativa

Aplicada por sprint.

## Componentes
- Revisión estructurada de Pull Requests
- Validación automática CI
- Checklist de supervisión IA
- Retroalimentación con scorecard

## Métricas Operativas
- Feedback ≤ 72 horas
- Mejora documentada entre sprint N y N+1
- Registro obligatorio de decisiones técnicas

---

# 4. Evaluación Sumativa

| Componente | Evidencia Principal | Validación Técnica |
|------------|--------------------|-------------------|
| Laboratorios | PR aprobado | CI verde + coverage mínimo |
| Tareas Técnicas | Documento + implementación | Revisión rúbrica |
| Participación Scrum | Sprint Report | Métricas reales |
| Proyecto Final | Sistema completo | Defensa técnica formal |

---

# 5. Rúbrica – Laboratorios Técnicos (Nivel 1–4)

| Nivel | Calidad Técnica | Coverage | Supervisión IA | Documentación |
|-------|----------------|----------|---------------|---------------|
| 1 | Código incompleto o frágil | <50% | Delegación sin restricciones | Ausente |
| 2 | Funcional parcial | 50–69% | Prompt limitado | README básico |
| 3 | Funcional robusto | ≥70% | Corrección justificada | README claro |
| 4 | Calidad industrial (modular + limpio) | ≥80% | Estrategia reusable documentada | ADR + evidencia CI |

---

# 6. Rúbrica – Tareas Técnicas

| Nivel | Planificación | Implementación | Verificación | Mejora Medible |
|-------|--------------|---------------|-------------|---------------|
| 1 | Sin plan formal | Generación directa | Sin tests | Sin mejora |
| 2 | Plan básico | Código funcional | Tests mínimos | Ajustes simples |
| 3 | Plan estructurado | Código limpio | Tests ≥70% coverage | Refactor explicado |
| 4 | Diseño estratégico con riesgos | Código optimizado | Validación automatizada | Mejora cuantificable |

---

# 7. Rúbrica – Participación Scrum

| Nivel | Artefactos | Colaboración | Liderazgo | Métricas |
|-------|-----------|--------------|-----------|----------|
| 1 | Uso mínimo | Baja participación | Pasivo | Sin datos |
| 2 | Backlog organizado | Participa | Apoya tareas | Métricas simples |
| 3 | DoD claro y usado | Activo | Facilita decisiones | Métricas reales |
| 4 | Backlog optimizado con IA | Coordina equipo | Lidera sprint | Métricas analizadas |

---

# 8. Rúbrica – Proyecto Final

| Nivel | Arquitectura | Calidad Técnica | Supervisión IA | Gobernanza | Defensa |
|-------|--------------|----------------|---------------|-----------|---------|
| 1 | Débil o incoherente | Inestable | Sin control | Sin política | Superficial |
| 2 | Funcional | Estable | Correcciones básicas | Riesgos identificados | Clara |
| 3 | ADR coherente | Robusto + CI estable | Supervisión documentada | Política básica IA | Argumentada |
| 4 | Arquitectura validada | Calidad industrial | Estrategia IA completa | Gobernanza formal | Defensa profunda |

---

# 9. Supervisión de Agentes IA – Criterios Específicos

| Criterio | Nivel 1 | Nivel 2 | Nivel 3 | Nivel 4 |
|----------|---------|---------|---------|---------|
| Calidad del Prompt | Ambiguo | Parcial | Claro + restricciones | Estratégico + reusable |
| Control de Alcance | Sin límites | Alcance parcial | Alcance definido | Control iterativo documentado |
| Verificación | Sin pruebas | Validación manual | Tests adecuados | Automatización CI |
| Corrección | No corrige | Corrección superficial | Corrección con análisis | Mejora estructural cuantificada |
| Trazabilidad | Sin registro | PR simple | PR documentado | ADR + commit vinculado |

---

# 10. Quality Gates Mínimos

## Para aprobar cualquier entrega:
- Coverage ≥ 70%
- Lint sin errores críticos
- Sin vulnerabilidades críticas conocidas
- README actualizado
- Pipeline CI exitoso

## Proyecto Final requiere:
- Coverage ≥ 80%
- ≥3 ADR documentados
- Política formal de uso IA
- Pipeline estable 3 ejecuciones consecutivas

---

# 11. Política de Entregas

## Reintentos
- 1 reintento por laboratorio.
- Proyecto final: revisión intermedia obligatoria.

## Criterios de Aprobación
- Puntaje mínimo global: Nivel 3.
- Cumplir todos los quality gates.

## Tolerancia a Fallos
- Falla CI = no aprobado.
- Uso indebido de IA (sin declaración) = revisión disciplinaria.

## Recuperación
Entrega correctiva con documento obligatorio:
"Post‑Mortem Técnico" incluyendo causa raíz y acción correctiva.

---

# 12. Ponderaciones por Modalidad

## Intensiva (8–10 semanas)

| Componente | Peso |
|------------|------|
| Laboratorios | 30% |
| Tareas | 20% |
| Participación Scrum | 10% |
| Proyecto Final | 40% |

## Semestral (16 semanas)

| Componente | Peso |
|------------|------|
| Laboratorios | 25% |
| Tareas | 20% |
| Participación Scrum | 15% |
| Proyecto Final | 40% |

## Ejecutiva (12 semanas)

| Componente | Peso |
|------------|------|
| Laboratorios | 20% |
| Casos Empresariales | 20% |
| Participación Estratégica | 10% |
| Proyecto Final Ejecutivo | 50% |

---

# 13. Escala Global de Certificación

| Puntaje Final | Certificación |
|---------------|---------------|
| Nivel 4 sostenido | Distinción Profesional |
| Nivel 3 | Aprobado Profesional |
| Nivel 2 | Aprobado Condicional |
| Nivel 1 | No Aprobado |

---

Documento listo para validación académica y empresarial.

