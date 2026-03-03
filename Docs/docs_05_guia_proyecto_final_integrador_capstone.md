# 05_Guia_Proyecto_Final_Integrador_Capstone.md

# Guía del Proyecto Final Integrador (Capstone)
## Desarrollo de Software con IA y Agentes Autónomos bajo Scrum

---

# 1. Objetivo del Capstone

El Proyecto Final Integrador tiene como finalidad demostrar dominio profesional en:

- Ingeniería de software moderna con IA
- Supervisión estratégica de agentes autónomos (Antigravity)
- Implementación bajo Scrum
- Arquitectura validada con evidencia técnica
- Gobernanza y calidad industrial

## Criterios de Éxito

El proyecto se considera exitoso si:

- Cumple todos los Quality Gates definidos.
- Evidencia uso real y documentado de agentes en múltiples fases.
- Presenta arquitectura coherente con decisiones justificadas (ADRs).
- Supera evaluación mínima Nivel 3 en todas las dimensiones.

---

# 2. Alcance Mínimo Requerido

## 2.1 Arquitectura
- Modelo C4 (Contexto + Contenedores mínimo).
- ≥3 ADR documentados.
- Identificación de riesgos técnicos.

## 2.2 Funcionalidades
- Mínimo 3 features completas end‑to‑end.
- Persistencia real de datos.
- Manejo de errores estructurado.

## 2.3 Pruebas
- Coverage ≥ 80%.
- Pruebas unitarias obligatorias.
- Al menos 1 prueba de integración.

## 2.4 CI/CD
- Pipeline automatizado (build + test + lint).
- Quality gates activos.

## 2.5 Documentación
- README profesional.
- Documentación API (OpenAPI/Swagger o equivalente).
- Política de uso responsable de IA.

## 2.6 Demo
- Video 8–12 minutos.
- Presentación técnica estructurada.

---

# 3. Uso Obligatorio de Agentes (Antigravity)

El proyecto debe integrar agentes en las siguientes fases:

| Fase | Evidencia Obligatoria |
|------|----------------------|
| Planificación | Generación de historias de usuario + backlog refinado por agente |
| Implementación | Código generado bajo prompt estructurado y supervisado |
| Pruebas | Generación inicial de tests por agente + validación humana |
| Documentación | README o API docs asistidas por IA |
| Pipeline | Configuración inicial generada por agente y revisada |

Debe incluir registro de prompts utilizados y justificación técnica.

---

# 4. Entregables Obligatorios

1. Repositorio Git público o privado compartido.
2. README completo.
3. Carpeta /docs con ADRs.
4. Documentación API.
5. Reporte de cobertura.
6. Evidencia de pipeline exitoso.
7. Video demo.
8. Pitch técnico (PDF).

---

# 5. Cronograma por Modalidad

## Intensiva (8–10 semanas)
- Sprint 1: Diseño + Backlog
- Sprint 2: Feature 1 + tests
- Sprint 3: Feature 2 + CI
- Sprint 4: Feature 3 + hardening
- Sprint 5: Demo + ajustes finales

## Semestral (16 semanas)
- Sprint 1–2: Diseño arquitectónico
- Sprint 3–6: Desarrollo incremental
- Sprint 7: Optimización + cobertura
- Sprint 8: Demo técnica

## Ejecutiva (12 semanas)
- Sprint 1–2: Diseño estratégico
- Sprint 3–5: Desarrollo core
- Sprint 6: Gobernanza + presentación

---

# 6. Rúbrica Resumida del Capstone

| Dimensión | Nivel 1 | Nivel 2 | Nivel 3 | Nivel 4 |
|------------|----------|----------|----------|----------|
| Arquitectura | Inconsistente | Funcional | Justificada con ADR | Validada por métricas |
| Calidad Técnica | Inestable | Estable | Robusta + CI | Industrial |
| Supervisión IA | Uso superficial | Corrección básica | Documentada | Estratégica y reusable |
| Gobernanza | Ausente | Parcial | Política básica | Formal y completa |
| Defensa Técnica | Superficial | Clara | Argumentada | Profunda y estratégica |

---

# 7. Checklist de Preparación para Presentación Final

## Técnica
- [ ] Todos los tests pasan
- [ ] Coverage ≥ 80%
- [ ] Pipeline verde
- [ ] ADRs actualizados

## Documentación
- [ ] README claro y ejecutable
- [ ] API documentada
- [ ] Política IA incluida

## Demo
- [ ] Flujo funcional sin errores
- [ ] Explicación arquitectura en <3 minutos
- [ ] Justificación decisiones técnicas

## Defensa
- [ ] Argumentos de trade‑offs
- [ ] Riesgos identificados
- [ ] Métricas presentadas

---

# Anexos

## Template – Estructura de README

```
# Proyecto
Descripción

## Arquitectura
Resumen + enlace ADR

## Instalación
Pasos reproducibles

## Testing
Comando cobertura

## Uso de IA
Prompts principales + supervisión
```

---

## Template – Registro de Prompts

```
Fecha:
Fase:
Prompt utilizado:
Resultado generado:
Correcciones realizadas:
Lección aprendida:
```

---

Documento listo para implementación en modalidad académica y empresarial.

