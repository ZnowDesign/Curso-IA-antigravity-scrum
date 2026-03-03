
# 06_Script_Teleprompter_Unidad_2_Extendida_Premium.md

# Unidad 2 – Versión Extendida Premium
## Scrum + IA + Agentes en Entorno Real (Deep Technical Edition)
Duración objetivo: 40–45 minutos  
Formato: Plataforma Premium / Cohorte / Corporativo

---

[HOOK ESTRATÉGICO – 0:00–1:30]

Scrum fue creado para equipos humanos.

Hoy coordinamos humanos… y agentes autónomos.

Pero integrar agentes dentro de Scrum sin rediseñar el proceso
es como poner un motor turbo en un auto sin frenos.

En esta sesión vamos a ver cómo integrar IA de manera profesional,
con métricas reales, gobierno técnico y disciplina operativa.

---

[BLOQUE 1 – REDEFINIENDO SCRUM EN 2025 – 1:30–8:00]

Scrum no cambia.
Pero su interpretación sí.

Eventos siguen siendo:
- Sprint Planning
- Daily
- Review
- Retrospective

Lo que cambia es:

1. Cómo redactamos historias.
2. Cómo estimamos.
3. Cómo medimos calidad.
4. Cómo delegamos.

Ejemplo real:

Historia tradicional:
“Como usuario quiero registrar una cuenta.”

Historia AI-Augmented:
“Como usuario quiero registrar una cuenta con validación de email RFC-compliant, password con reglas de seguridad, tests automatizados (≥70% coverage), sin librerías externas, compatible con Node 18.”

Observa la diferencia.

El segundo formato es delegable.

---

[BLOQUE 2 – DISEÑO DEL SPRINT CON DELEGACIÓN CONTROLADA – 8:00–16:00]

Supongamos un Sprint de 1 semana.

Objetivo:
Construir Users API mínima.

Sprint Backlog:

1. GET /users
2. POST /users
3. Validación robusta
4. Tests
5. Documentación Swagger

Ahora tomamos decisiones:

¿Qué delegamos?
¿Qué supervisamos?
¿Qué diseñamos manualmente?

Regla práctica:

Delegar lo repetitivo.
Supervisar lo estructural.
Diseñar lo crítico.

Ejemplo técnico:

No delegamos el modelo de dominio.
Sí delegamos funciones de validación.
No delegamos arquitectura base.
Sí delegamos generación de tests.

---

[BLOQUE 3 – PROMPTS COMO ARTEFACTOS SCRUM – 16:00–23:00]

En AI-Augmented Scrum,
el prompt es un artefacto técnico.

Debe incluir:

Contexto:
“Proyecto Node.js Express, arquitectura MVC.”

Tarea:
“Implementar controlador POST /users.”

Restricciones:
“Sin librerías externas, validación manual.”

Criterios:
“Coverage ≥ 70%, Jest obligatorio.”

Ejemplo real de prompt:

Actúa como backend senior.
Implementa POST /users bajo arquitectura MVC.
Validar email con regex RFC5322.
Password mínimo 8 caracteres, 1 número y 1 símbolo.
Incluir tests Jest.
No usar dependencias externas.
Cobertura mínima 70%.
Documentar con JSDoc.

Eso es un artefacto técnico.

---

[BLOQUE 4 – SUPERVISIÓN PROFUNDA Y REVISIÓN – 23:00–30:00]

Cuando el agente genera código:

No lo aceptamos.

Revisamos:

- Complejidad ciclomática.
- Separación de responsabilidades.
- Manejo de errores.
- Seguridad básica.

Luego ejecutamos:

npm test
npm run lint

Verificamos coverage.

Si no alcanza 70%:

Iteramos.

Si la validación está incompleta:

Refinamos prompt.

El agente no es responsable.
Nosotros lo somos.

---

[BLOQUE 5 – PIPELINE COMO GATE DE GOBERNANZA – 30:00–36:00]

El pipeline es el juez imparcial.

Build.
Test.
Lint.
Security scan.
Deploy.

Sin pipeline verde,
no hay Done.

Ejemplo de fallo común:

Coverage 52%.
Funciona.
Pero no cumple estándar.

Resultado:

Historia no se mueve a Done.

Disciplina > velocidad.

---

[BLOQUE 6 – MÉTRICAS DE MADUREZ – 36:00–41:00]

Cómo saber si el equipo madura:

1. Iteraciones promedio por historia delegada.
2. Fallos CI por sprint.
3. Tiempo de revisión humana.
4. Ratio delegación vs código manual.

Si iteramos demasiado,
el problema está en el diseño inicial.

Si el CI falla constantemente,
la gobernanza es débil.

---

[BLOQUE 7 – CASO REAL SIMULADO – 41:00–44:00]

Sprint Review:

Mostramos:
- Endpoints funcionando.
- Coverage 78%.
- CI verde.
- Documentación Swagger generada.

Explicamos:
Qué delegamos.
Qué no delegamos.
Qué iteramos.

Eso es madurez profesional.

---

[CIERRE EJECUTIVO – 44:00–45:00]

La IA no elimina Scrum.

La IA exige más disciplina Scrum.

Delegar no es automatizar sin pensar.

Es diseñar mejor.
Controlar mejor.
Validar mejor.

Eso es AI-Augmented Engineering real.

En la siguiente unidad veremos cómo escalar esta integración en equipos más grandes.

Fin de la sesión.
