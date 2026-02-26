# Diseño estratégico del nuevo programa académico 2025–2026 en ingeniería de software con agentes autónomos

## Contexto global y transformación del trabajo de desarrollo

Entre 2024 y 2026, el desarrollo de software asistido por IA dejó de ser “autocomplete con esteroides” y se movió hacia **plataformas agentic**: sistemas donde uno o varios agentes pueden **planear, ejecutar y verificar** tareas complejas usando herramientas reales (editor, terminal, navegador, CI). Un ejemplo claro es **Google Antigravity**, que formaliza un enfoque *agent-first* con dos superficies: una vista tipo IDE para trabajo síncrono y una superficie “manager” para **orquestar múltiples agentes de forma asíncrona**. citeturn5view2turn6view0

Este cambio está respaldado por investigación y benchmarks que ya no evalúan “una función en un archivo”, sino **resolución de issues reales en repos**. *SWE-bench* (ICLR 2024) define el problema de resolver issues a partir de repos y descripciones; y *SWE-agent* (NeurIPS 2024) muestra que el diseño de interfaces “agent-computer” impacta performance en tareas reales de ingeniería. citeturn3search20turn3search21turn3search8  
Además, trabajos como **AutoCodeRover** (ISSTA 2024 / arXiv 2024) investigan enfoques autónomos de “program improvement” (bugs + features) combinando LLMs con búsqueda/diagnóstico, apuntando explícitamente al mantenimiento/evolución de software. citeturn3search2turn3search10turn3search6

En el ecosistema industrial, el patrón se repite: **GitHub Copilot en VS Code** ya describe capacidades **multi‑agent** y ejecución en paralelo, y **GitLab** está empujando su **Duo Agent Platform** para automatización con contexto DevSecOps. citeturn2search23turn2search1turn2search16turn2search10

El resultado práctico: el rol del desarrollador se desplaza de *“escribir cada línea”* hacia *“diseñar el trabajo, supervisarlo y validar calidad”*. Esto no es filosofía: organizaciones grandes reportan explícitamente que el cuello de botella no era teclear más rápido, sino navegar contexto, documentación, pruebas, releases y toil. Por ejemplo, **AWS** describe que, en la industria, los devs pueden pasar **solo 1–2 horas diarias escribiendo código** y el resto en tareas necesarias alrededor del ciclo de vida. citeturn12search0turn12search5  
En paralelo, **Atlassian** reporta en su State of DevEx 2025 la paradoja: la IA ahorra tiempo, pero la productividad total se sigue “fugando” por fricción organizacional (información, coordinación, dirección). citeturn11search0turn11search2turn11search8

Lo que sí se está volviendo obsoleto (o, con cariño, “comoditizado”) no es saber programar, sino depender de:
- **boilerplate manual** como ventaja competitiva,
- “memorizar” APIs sin habilidad de integrar contexto rápido,
- prácticas de QA que no escalan (sin automatización ni CI),
- y, sobre todo, trabajar sin mecanismos de verificación y gobernanza para output generado por agentes. citeturn10search0turn10search2turn5view2

El riesgo de no actualizar la formación es doble: quedarse atrás en productividad y, peor, **romper cosas más rápido**. Antigravity, por ejemplo, expone explícitamente políticas de ejecución en terminal y revisión (request review vs auto‑execute), y advierte sobre **prompt injection** vía navegación web, sugiriendo allowlists. citeturn6view0turn7search1  
Y sí: ya hubo incidentes públicos donde herramientas agentic ejecutaron acciones destructivas por mala interpretación (la versión moderna del “rm -rf”, pero con sonrisa). citeturn0news45turn0news49

image_group{"layout":"carousel","aspect_ratio":"16:9","query":["Google Antigravity agent manager screenshot","Scrum framework diagram events artifacts roles"],"num_per_query":1}

## Alineación con estándares y marcos formales

Este programa se diseña para que sea “vendible” (plataformas, empresas) sin perder rigor académico. La alineación se apoya en cuatro pilares:

Primero, **Scrum** como marco operativo del curso, usando roles, eventos, artefactos y compromisos (Product Goal, Sprint Goal, Definition of Done) como esqueleto de ejecución y evaluación. Se toma como fuente normativa la **Guía Scrum 2020**. citeturn1search8turn1search0

Segundo, el cuerpo de conocimiento de ingeniería de software: **SWEBOK v4.0** de entity["organization","IEEE Computer Society","professional society"], que actualiza y consolida áreas como requirements, design, construction, testing, maintenance, configuration management, quality y process. citeturn1search1turn1search5

Tercero, el marco curricular: **Computing Curricula 2020** (CC2020) de entity["organization","ACM","computing society"] y entity["organization","IEEE","professional association"] como guía para balancear conocimientos, habilidades y competencias, con énfasis en resultados medibles y diversidad de trayectorias. citeturn1search2turn1search30

Cuarto, el ciclo de vida formal: **ISO/IEC/IEEE 12207:2017**, que define un marco de procesos de ciclo de vida aplicable a adquisición, desarrollo, operación y mantenimiento, útil para “traducir” lo ágil a un lenguaje que entiende auditoría, sector público y enterprise. citeturn1search3turn1search35

En seguridad y gobernanza (obligatorio en agentes), el programa se apoya en:
- **NIST AI RMF 1.0** y su perfil para GenAI, para gestionar riesgos y confiabilidad. citeturn7search0turn7search2turn7search6  
- **NIST SSDF (SP 800‑218)** para prácticas de desarrollo seguro integrables a cualquier SDLC (incluido Scrum). citeturn7search3turn7search7  
- **OWASP Top 10 for LLM Applications**, donde Prompt Injection aparece como riesgo central. citeturn7search1turn7search5

## Perfil de egreso estratégico

El egresado se perfila como **AI‑Augmented Software Engineer / AI Supervisor Técnico**: alguien capaz de entregar software con agentes sin sacrificar calidad, seguridad ni trazabilidad.

**Competencias técnicas profundas (medibles)**  
El egresado puede implementar y mantener un incremento de producto en un repositorio real, asegurando que:
- el cambio pasa suites de pruebas automatizadas y controles de CI,  
- integra cambios multi‑archivo, y  
- mantiene calidad de ingeniería (legibilidad, modularidad, deuda técnica controlada). citeturn3search20turn3search2turn1search1

**Competencias arquitectónicas**  
El egresado puede diseñar arquitectura y restricciones para que el trabajo delegable a agentes sea seguro y verificable (fronteras, contratos, módulos, *guardrails*), aplicando prácticas de diseño y mantenimiento coherentes con SWEBOK. citeturn1search1turn3search10turn10search2

**Competencias de supervisión de IA**  
El egresado puede operar una plataforma agentic (p. ej., Antigravity) configurando políticas de ejecución/revisión, gestionando artefactos verificables y mitigando riesgos (allowlists, revisión humana, sandbox), reduciendo el “trust gap” en trabajo autónomo. citeturn5view2turn6view0turn7search1

**Competencias de liderazgo técnico bajo Scrum**  
El egresado puede planear y ejecutar trabajo en Sprints con un backlog diseñado para delegación a agentes, manteniendo Definition of Done y trazabilidad de valor a Product Goal. citeturn1search8turn4search10turn11search0

**Competencias éticas y regulatorias**  
El egresado puede identificar riesgos de GenAI (seguridad, privacidad, prompt injection, output inseguro) y aplicar controles y gobierno alineado a NIST/OWASP/SSDF. citeturn7search2turn7search3turn7search1

## Diseño curricular completo

**Nivel y prerrequisitos**  
Programa profesional avanzado (equivalente a diplomado/posgrado práctico). Se asume experiencia previa en: Git, pruebas unitarias básicas, HTTP/APIs, y un stack de desarrollo (web o backend). Esta decisión es intencional: si el alumno aún está peleándose con “qué es una rama”, el agente le va a ganar por KO técnico.

**Estructura por unidades**  
Se proponen 10 unidades en secuencia pedagógica de: fundamentos → operación de agentes → ingeniería de calidad → DevSecOps/CI/CD → gobernanza → capstone. La selección y orden se justifican por el salto industry‑grade hacia flujos agentic descritos en plataformas como Antigravity (planificar‑ejecutar‑verificar con herramientas) y por la evidencia de investigación en agentes para SE (resolución de issues reales). citeturn5view2turn6view0turn3search21turn10search2

A continuación, cada unidad incluye objetivo, resultados medibles (con verbo observable) y el nivel cognitivo máximo esperado (orientado por taxonomías de aprendizaje, con énfasis en aplicación/creación):

| Unidad | Enfoque | Objetivo específico | Resultados de aprendizaje medibles (máximo nivel) | Evidencia práctica obligatoria |
|---|---|---|---|---|
| Fundamentos de AI‑Augmented Engineering | Paradigma agentic, límites, evaluación | Entender qué tareas son delegables y cómo se verifican | Delimita tareas delegables; compara asistencia vs autonomía; explica trade‑offs de evaluación tipo issue‑resolution (Analizar/Evaluar) citeturn3search20turn7search4turn7search8 | Mini‑lab: resolver issue simple en repo con verificación por tests, documentando supuestos |
| Scrum aplicado a trabajo con agentes | Scrum operativo para equipos aumentados | Ejecutar Scrum “de verdad” con trabajo delegado a agentes | Construye backlog con Definition of Done y compromisos; ejecuta eventos Scrum y evidencia incrementos (Aplicar/Crear) citeturn1search8turn4search10 | Simulación Sprint 0: backlog + DoD + entorno de repo |
| Antigravity como plataforma agent‑first | Orquestación multi‑agente, políticas, artefactos | Configurar y operar Antigravity con seguridad básica | Configura políticas de ejecución/revisión; usa modos de planeación vs ejecución rápida; gestiona artefactos verificables (Aplicar) citeturn6view0turn5view2 | Lab: instalación + configuración + primer agente con “request review” |
| Diseño de especificaciones delegables | Spec‑driven + criterios de aceptación | Escribir specs que un agente pueda ejecutar sin ambigüedad | Redacta historias con AC; define invariantes; traduce specs en tareas atómicas para agentes (Crear) citeturn6view1turn6view0 | Taller: transformar requerimientos difusos en spec ejecutable + checklist |
| Implementación multi‑archivo supervisada | Cambios end‑to‑end con verificación | Ejecutar desarrollo por agente con revisión profesional | Realiza PR con cambios multi‑módulo; ejecuta revisión técnica; corrige errores del agente (Evaluar/Crear) citeturn5view2turn2search23turn3search2 | Lab: feature completa (UI/API) con revisión y aprobación humana |
| Testing impulsado por modelos | Unit/integration/e2e con generación asistida | Elevar cobertura y confiabilidad con criterios | Genera y mejora pruebas; mide cobertura útil; detecta pruebas frágiles; integra testing a CI (Evaluar) citeturn3search20turn7search4 | Lab: suite de pruebas + “test gap report” |
| AI‑assisted CI/CD y DevSecOps | CI/CD gobernado, automatización segura | Operar pipelines con guardrails y feedback loop | Integra CI (build/test/lint); define gates; automatiza checks; gestiona fallas y rollback (Aplicar/Crear) citeturn2search16turn12search12turn7search3 | Pipeline mínimo viable + policy de merge + evidencias |
| Gobernanza y seguridad de agentes | Prompt injection, permisos, supply chain | Reducir superficie de ataque y daño operativo | Implementa allowlists; limita permisos; aplica SSDF; gestiona riesgos OWASP LLM (Evaluar) citeturn6view0turn7search1turn10news45 | Laboratorio: hardening del entorno y checklist de seguridad |
| Observabilidad, métricas y DevEx con IA | Métricas útiles, no teatro | Medir efectividad real (calidad/flujo) | Define métricas alineadas a valor; analiza fricción; propone mejoras de proceso y tooling (Analizar/Evaluar) citeturn11search0turn12search3 | Reporte DevEx: “dónde se va el tiempo” + plan de mejora |
| Capstone profesional | Producto completo en Sprints | Integrar todo en un proyecto realista | Entrega incrementos por Sprint; justifica decisiones; evidencia gobierno de agentes; cumple DoD (Crear/Evaluar) citeturn1search8turn6view0turn7search2 | Proyecto final + defensa técnica |

## Cargas horarias y modalidades profesionales

Se propone una **carga total de 120 horas de trabajo del estudiante**, con predominio práctico, porque el núcleo del programa es operar ingeniería con agentes (no “leer sobre” agentes). Esta orientación está alineada con tendencias reportadas: la ganancia de IA se pierde si el equipo no mejora flujo, calidad y coordinación (DevEx + procesos). citeturn11search0turn12search0

**Distribución base (120 h)**  
- Teoría guiada (sincrónica): **24 h**  
- Taller práctico guiado (sincrónica): **24 h**  
- Laboratorio autónomo (asincrónico): **48 h**  
- Proyecto integrador (asincrónico + checkpoints): **24 h**

**Relación práctica vs teoría**: ~80% práctica (taller+lab+proyecto) / 20% teoría.

**Asignación por unidad (horas totales por unidad)**  
- Unidades 1–2: 18 h  
- Unidades 3–4: 26 h  
- Unidades 5–7: 36 h  
- Unidad 8: 10 h  
- Unidad 9: 10 h  
- Unidad 10 (Capstone): 20 h  
(La suma mantiene 120 h; la mayor carga está en implementación/QA/CI y capstone, donde se materializa el aprendizaje).

**Tres modalidades de calendario (misma carga, distinto ritmo)**

| Modalidad | Duración | Ritmo semanal sugerido | Sprints académicos | Justificación |
|---|---|---|---|---|
| Intensiva | 10 semanas | 4.8 h sincrónicas + 7.2 h asincrónicas (≈12 h/sem) | 5 Sprints de 2 semanas | Maximiza inmersión; ideal para bootcamp profesional sin perder gobernanza |
| Ejecutiva | 12 semanas | 4 h sincrónicas + 6 h asincrónicas (≈10 h/sem) | 4 Sprints de 3 semanas | Mejor para profesionales; más tiempo para hardening y calidad incremental |
| Semestral | 16 semanas | 3 h sincrónicas + 4.5 h asincrónicas (≈7.5 h/sem) | 4 Sprints de 4 semanas | Favorece profundidad, retroalimentación y madurez de prácticas de ingeniería |

La estructura por Sprints se fundamenta en la Guía Scrum (inspección y adaptación) y en la evidencia de que la productividad real depende del sistema de trabajo, no solo del editor con IA. citeturn1search8turn11search0

## Proyecto final integrador y modelo de evaluación por rúbrica

**Objetivo del capstone**  
Construir, probar y desplegar (en entorno controlado) un producto o feature de nivel profesional usando **Scrum** y una plataforma agentic (Antigravity), asegurando **trazabilidad, seguridad, CI/CD y calidad**.

**Alcance mínimo**  
- Un servicio (API) + un consumidor (UI o cliente) o un componente equivalente de arquitectura.  
- Al menos 2 flujos end‑to‑end.  
- Pruebas automatizadas (unit + integración o e2e según stack) integradas en CI.  
- Políticas de gobernanza de agentes: permisos, revisión y mitigación de prompt injection (allowlist o equivalente). citeturn6view0turn7search1turn7search3

**Entregables**  
- Repositorio con historial claro (PRs/commits), evidencias de pipeline y releases.  
- Product Backlog con historias y criterios de aceptación.  
- Evidencia de eventos Scrum: planificación, revisiones, retrospectivas (puede ser minuta corta). citeturn1search8turn4search10  
- “Dossier de supervisión de agentes”: configuración de políticas de ejecución/revisión en Antigravity, artefactos de verificación (planes, screenshots/recordings cuando aplique) y decisiones humanas de aceptación/rechazo. citeturn5view2turn6view0  
- Informe de seguridad: top riesgos OWASP LLM aplicables y mitigaciones adoptadas. citeturn7search1turn7search5

**Rúbrica sugerida (100 puntos)**  
- Valor y claridad del backlog (10): historias, AC, priorización, trazabilidad a Product Goal. citeturn1search8  
- Arquitectura y mantenibilidad (20): modularidad, decisiones justificadas, deuda técnica controlada (SWEBOK). citeturn1search1  
- Calidad e ingeniería (25): pruebas, CI/CD, Definition of Done cumplida, estabilidad del incremento. citeturn7search3turn12search12  
- Supervisión de agentes (25): políticas, revisión efectiva, evidencia de verificación (artefactos), corrección de fallas del agente. citeturn6view0turn5view2  
- Seguridad y gobernanza (15): mitigaciones OWASP/NIST, control de permisos, manejo de prompt injection. citeturn7search1turn7search2turn6view0  
- Defensa técnica (5): explicación clara de decisiones y trade‑offs.

## Benchmark internacional y posicionamiento premium

El mercado 2024–2026 ofrece piezas sueltas; el diferencial está en **integrarlas con rigor**.

**Herramientas y certificaciones orientadas a uso de copilots**  
- Recursos oficiales (p. ej., docs de VS Code para Copilot, rutas de aprendizaje de Microsoft, certificación de Copilot) entrenan uso de la herramienta, pero no necesariamente cubren gobernanza profunda ni integración curricular con estándares SE y evaluación tipo capstone. citeturn2search1turn8search2turn2search4turn8search10  
- entity["company","GitLab","devsecops platform"] ofrece learning paths y documentación de Duo/Duo Agent Platform muy valiosa para DevSecOps, pero su objetivo es adopción del ecosistema, no un programa académico integral con Scrum + SWEBOK + ISO + gobernanza agentic. citeturn2search2turn2search16turn2search10  
- entity["company","Google","tech company"] con Antigravity aporta el “poste de luz” agent‑first (artifacts, policies, multi‑agent manager), pero sus codelabs están orientados a onboarding de producto, no a formar supervisores técnicos con evaluación formal y arquitectura de aprendizaje. citeturn6view0turn5view2

**Programas de agentic AI (más cercanos a “construir agentes” que a “entregar software”)**  
- Especializaciones y cursos como los de entity["company","Coursera","online learning platform"] (p. ej., AI Agents/Agent Developer) y alianzas universitarias (p. ej., Vanderbilt) tienden a enfocarse en arquitectura de agentes y uso general, no en ingeniería del software completa con CI/CD, DoD, y gobierno de permisos sobre repos/terminal/navegación. citeturn2search12turn8search12turn8search1  
- Programas como el “Agentic AI Certificate” de entity["organization","Johns Hopkins University","research university"] muestran que el tema llegó al terreno formal; aun así, suelen centrarse en LLMs/agentes como disciplina, no en un SDLC Scrum con agentes operando en tooling real de ingeniería y evaluación por incremento. citeturn8search25

**Certificaciones ágiles avanzadas**  
- entity["organization","Scrum.org","scrum certification org"] (PSM II, PSD, APS‑SD) y entity["organization","Scrum Alliance","agile certification body"] (CSM) cubren Scrum y prácticas, y APS‑SD enfatiza “aprender Scrum haciendo Scrum”; sin embargo, no están diseñadas para el escenario 2025–2026 de agentes autónomos con políticas de ejecución, mitigación de prompt injection y evaluación de output generado por IA. citeturn4search0turn4search10turn4search2turn4search1  
- entity["organization","Scaled Agile","safe framework org"] (SAFe) incluye formación enterprise y hasta menciona IA como acelerador, pero el enfoque es escalado organizacional, no operación técnica agentic a nivel repo y CI/CD. citeturn4search3turn4search7

**Diferenciadores del programa propuesto (posicionamiento premium)**  
- Integra agent‑first IDE + Scrum operativo + SWEBOK + ISO 12207 + seguridad OWASP/NIST/SSDF en un solo currículo. citeturn6view0turn1search1turn1search3turn7search1turn7search3  
- Evalúa con evidencia verificable (artefactos, tests, pipelines), no con “me funcionó en mi máquina”. citeturn5view2turn3search20turn7search4  
- Forma explícitamente el rol emergente de supervisor: diseño de trabajo delegable + control de permisos + verificación. Esto responde a hallazgos de adopción industrial donde la fricción mayor ya no es escribir código, sino coordinar, encontrar información, asegurar calidad y reducir toil. citeturn11search0turn12search0

## Justificación estratégica y visión a tres a cinco años

**Por qué es necesario en 2025–2026**  
Porque la industria está estandarizando **autonomía parcial**: agentes que planean, ejecutan y verifican. Antigravity lo describe como operar a nivel tarea (no línea) y apalancar artefactos para cerrar la brecha de confianza; VS Code ya habla de multi‑agent; GitLab impulsa agentes con contexto DevSecOps. citeturn5view2turn2search23turn2search16

**Por qué es diferente a cursos tradicionales**  
Un curso tradicional enseña “usar IA para codear”. Este programa enseña **ingeniería**: cómo producir incrementos con calidad, seguridad, métricas y gobernanza, cuando parte del trabajo lo ejecuta un actor no humano con acceso a herramientas reales. Eso exige controles (políticas de terminal/revisión, allowlists, seguridad de agentes) y un proceso de verificación (pruebas + CI + artefactos). citeturn6view0turn7search1turn7search3turn5view2

**Por qué tiene potencial alto de monetización**  
Porque encaja en tres mercados simultáneos:
- B2C profesional: devs/tech leads que necesitan upskilling práctico en agentic workflows (Copilot/agent platforms) más allá de prompts. citeturn2search23turn6view0  
- B2B: empresas que quieren productividad sin aumentar riesgo (NIST/OWASP/SSDF como lenguaje común). citeturn7search2turn7search3turn11search0  
- Certificación interna / cohorte: el formato por Sprints y capstone es evaluable y auditable (lo que a empresas les gusta porque reduce “capacitaciones decorativas”). citeturn1search8turn1search3

**Visión 3–5 años (2026–2031)**  
Tres tendencias deberían guiar la evolución del programa:

1) **Benchmarks saturan rápido**. OpenAI ya advierte que SWE‑bench Verified dejó de medir frontera; el punto no es perseguir un número, sino enseñar evaluación robusta: pruebas, revisión, seguridad, monitoreo y trazabilidad. citeturn7search8turn7search4turn7search14  

2) **Seguridad será el freno o el acelerador**. La combinación de agentes + features legacy de IDEs abre vectores (prompt injection, exfiltración, RCE), y ya hay reportes de vulnerabilidades sistémicas en herramientas AI‑assisted. Este programa lo incorpora como unidad central, no como apéndice. citeturn10news45turn7search1turn6view0  

3) **La ventaja competitiva será el flujo end‑to‑end**, no “code gen”. DevEx y fricción organizacional seguirán comiéndose los beneficios si no se reestructura trabajo. Por eso Scrum + métricas + gobernanza de agentes es el combo: sin eso, la IA solo te ayuda a escribir código más rápido… para esperar más rápido en el próximo bloqueo. citeturn11search0turn12search0turn1search8