# 02_Mapa_Competencias_Outcomes.md

# Mapa de Competencias y Outcomes
## Desarrollo de Software con IA y Agentes Autónomos bajo Scrum

---

# 1. Marco General

Este documento define las **competencias profesionales medibles** del programa, alineadas explícitamente con:

- Scrum (roles, eventos y artefactos)
- Desarrollo supervisado con agentes (Antigravity)
- Prácticas industriales reales (CI/CD, testing, arquitectura, seguridad)
- Exigencias del mercado 2025–2026

Las competencias están organizadas en cinco categorías estratégicas:

1. Técnicas de Ingeniería de Software
2. Arquitectónicas
3. Supervisión de IA y Agentes
4. Liderazgo Técnico Ágil
5. Ética y Gobernanza

Cada competencia incluye:
- Nivel Bloom
- Criterios observables
- Evidencias concretas
- Instrumentos de evaluación

---

# 2. Competencias Técnicas

| Código | Competencia | Nivel Bloom | Criterios Observables | Evidencia (Entregable) | Instrumento de Evaluación |
|--------|------------|------------|-----------------------|------------------------|--------------------------|
| CT1 | Implementa funcionalidades multi-archivo supervisando agentes | Aplicar / Analizar | PR funcional, commits coherentes, sin código innecesario generado por IA | Repositorio + Pull Request documentado | Code Review con rúbrica técnica |
| CT2 | Diseña y ejecuta pruebas automatizadas con cobertura objetivo | Aplicar / Evaluar | Cobertura >= 70%, tests reproducibles en CI | Reporte coverage + suite tests | Validación CI + checklist técnico |
| CT3 | Configura pipeline CI con quality gates | Crear | Workflow bloquea PR con fallas de lint/test | YAML pipeline + evidencia ejecución | Auditoría pipeline |
| CT4 | Refactoriza código generado por IA aplicando principios SOLID | Analizar / Evaluar | Mejora estructural comprobable (reducción duplicación / complejidad) | Commit refactor + diff comparativo | Rúbrica técnica estructural |

---

# 3. Competencias Arquitectónicas

| Código | Competencia | Nivel Bloom | Criterios Observables | Evidencia | Instrumento |
|--------|------------|------------|-----------------------|-----------|------------|
| CA1 | Diseña arquitectura con ADRs justificadas | Analizar / Evaluar | ADR con trade-offs claros y riesgos identificados | Documento ADR (mínimo 3) | Rúbrica arquitectura |
| CA2 | Modela sistema usando C4 o equivalente | Aplicar | Diagramas coherentes con implementación real | Diagramas + enlace repo | Validación técnica |
| CA3 | Evalúa riesgos técnicos y dependencias | Evaluar | Matriz riesgos con mitigaciones accionables | Documento riesgo | Checklist revisión técnica |

---

# 4. Competencias de Supervisión de IA y Agentes

| Código | Competencia | Nivel Bloom | Criterios Observables | Evidencia | Instrumento |
|--------|------------|------------|-----------------------|-----------|------------|
| CI1 | Diseña prompts técnicos delegables y verificables | Crear | Prompt incluye alcance, restricciones, criterios de aceptación | Librería de prompts versionada | Evaluación práctica |
| CI2 | Detecta y corrige errores o alucinaciones generadas por IA | Evaluar | Corrección documentada con explicación técnica | Registro cambios + comentario PR | Rúbrica supervisión |
| CI3 | Controla alcance y versionado en trabajo con agentes | Analizar | Commit history estructurado, sin cambios fuera de scope | Repo auditado | Auditoría técnica |
| CI4 | Aplica estrategia plan-first antes de delegar implementación | Aplicar | Documento de planificación previo a ejecución | Plan técnico aprobado | Evaluación estructural |

---

# 5. Competencias de Liderazgo Técnico Ágil

| Código | Competencia | Nivel Bloom | Criterios Observables | Evidencia | Instrumento |
|--------|------------|------------|-----------------------|-----------|------------|
| CL1 | Lidera sprint AI-Augmented | Aplicar / Evaluar | Sprint report con métricas reales (lead time, defect rate) | Reporte sprint | Evaluación 360° |
| CL2 | Define Definition of Done con criterios IA | Crear | DoD documentado incluyendo quality gates | Documento Scrum | Rúbrica liderazgo |
| CL3 | Gestiona deuda técnica en entorno AI | Analizar / Evaluar | Plan reducción deuda con impacto medible | Documento técnico | Evaluación estratégica |

---

# 6. Competencias Éticas y Regulatorias

| Código | Competencia | Nivel Bloom | Criterios Observables | Evidencia | Instrumento |
|--------|------------|------------|-----------------------|-----------|------------|
| CE1 | Evalúa riesgos de privacidad en uso de IA | Evaluar | Identificación de datos sensibles y mitigación | Política AI Usage | Rúbrica ética |
| CE2 | Gestiona licencias OSS en código generado por IA | Aplicar / Evaluar | Checklist de licencias aplicado | Documento compliance | Validación checklist |
| CE3 | Diseña política interna de uso responsable de IA | Crear | Política estructurada con reglas claras | Documento formal | Evaluación documental |

---

# 7. Niveles de Dominio

| Nivel | Descriptor Medible | Evidencia Requerida |
|--------|-------------------|--------------------|
| Básico | Ejecuta tareas guiadas con supervisión mínima | Lab funcional validado |
| Intermedio | Supervisa, corrige y optimiza producción IA | PR mejorado + tests |
| Avanzado | Diseña arquitectura, políticas y liderazgo AI | Proyecto final completo |

---

# 8. Rúbrica Resumida por Nivel

| Nivel | Técnica | Arquitectura | Supervisión IA | Liderazgo | Ética |
|--------|--------|--------------|---------------|-----------|-------|
| Básico | Funciona correctamente | Diseño parcial | Uso básico agente | Participa activamente | Reconoce riesgos |
| Intermedio | Calidad estable + tests | ADR coherente | Corrige errores IA | Coordina sprint | Mitiga riesgos |
| Avanzado | Calidad industrial | Arquitectura sólida validada | Control estratégico del agente | Lidera equipo y métricas | Define políticas y gobernanza |

---

# 9. Alineación con Scrum y Desarrollo con Agentes

| Evento / Artefacto Scrum | Competencias Asociadas |
|--------------------------|------------------------|
| Product Backlog | CL2, CI1 |
| Sprint Planning | CL1, CI4 |
| Sprint Backlog | CT1, CI1 |
| Definition of Done | CT2, CI2 |
| Sprint Review | CL1 |
| Retrospective | CL3 |

---

# 10. Matriz de Empleabilidad

| Rol Profesional | Competencias Clave | Nivel Esperado |
|-----------------|-------------------|---------------|
| AI-Augmented Developer | CT1, CT2, CI1 | Intermedio |
| AI Supervisor | CI1, CI2, CA1 | Avanzado |
| Tech Lead AI | CA1, CL1, CE1 | Avanzado |
| Arquitecto AI | CA1, CA3, CE3 | Avanzado |
| Engineering Manager IA | CL1, CL3, CE1 | Avanzado |

---

