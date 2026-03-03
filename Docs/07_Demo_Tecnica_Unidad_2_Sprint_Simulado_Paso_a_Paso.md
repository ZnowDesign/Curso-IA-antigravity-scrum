
# 07_Demo_Tecnica_Unidad_2_Sprint_Simulado_Paso_a_Paso.md

# Demo Técnica Completa – Unidad 2 (Lista para Grabar)
## Sprint Simulado con Scrum + IA + Agentes (Antigravity / AI-Augmented Engineering)

Duración objetivo de demo: **18–25 min (Marketplace)** / **30–40 min (Premium)**  
Formato: **Screen recording + cámara (opcional)**  
Resultado final: **Users API funcional + CI verde + coverage ≥ 70% + prompts documentados**

---

# 0) Qué vas a demostrar (en 20 segundos)

**Mensaje clave:** “La IA acelera, pero Scrum + CI gobiernan.”  
**Evidencia final en pantalla:**  
- Endpoint funcionando  
- Tests pasando  
- Coverage ≥ 70%  
- Pipeline CI verde  
- Prompts y decisiones documentadas  

---

# 1) Preparación previa (antes de grabar)

## 1.1 Requisitos técnicos
- Node.js **18+**
- Git
- Editor (VS Code recomendado)
- Cuenta GitHub (para mostrar CI)
- Proyecto template (puede ser el repo base del curso)

## 1.2 Higiene de grabación
- Desactivar notificaciones
- Terminal limpia (prompt minimal)
- Zoom activado en pantalla (ideal 110–125%)
- Fuente monoespaciada ≥ 16–18 pt
- Repo sin secretos (nada de API keys en pantalla)

## 1.3 Archivos que deben existir
- `README.md`
- `package.json`
- `src/`
- `tests/`
- `.github/workflows/ci.yml`
- `docs/SPRINT.md` (backlog)
- `docs/PROMPTS.md` (prompts usados)
- `docs/RETRO.md` (retro)

---

# 2) Guion de demo (timeline sugerido)

## 2.1 (0:00–2:30) Sprint Planning (rápido, visual)
**Objetivo:** mostrar que “primero se planea”.

### En pantalla: `docs/SPRINT.md`
Pega/explica este Sprint Backlog (corto):

```md
# Sprint 1 – Users API (AI-Supervised)

## Objetivo del Sprint
Entregar Users API mínima con calidad verificable (CI + coverage ≥70%).

## Historias
1) GET /users
   - AC: retorna arreglo JSON (mock o in-memory)
   - DoD: tests + CI verde + coverage ≥70%

2) POST /users
   - AC: crea usuario en memoria con validación
   - DoD: tests + CI verde + coverage ≥70%

3) Validación validateUser(email, password)
   - AC: email válido, password min 8, 1 número, 1 símbolo
   - DoD: tests unitarios + coverage ≥70%
```

**Punto instructor (one-liner):** “La IA entra DESPUÉS del diseño.”

---

## 2.2 (2:30–5:00) DoR / DoD (lo mínimo, pero serio)
### Definition of Ready (decirlo y señalarlo)
- Historia delimitada
- Restricciones explícitas
- Criterios verificables
- Tarea delegable definida

### Definition of Done (mostrar en README o `docs/SPRINT.md`)
- CI verde
- Coverage ≥ 70%
- Lint sin errores críticos (si aplica)
- Docs actualizadas
- Evidencia de supervisión IA (prompts + decisiones)

---

## 2.3 (5:00–7:00) Setup del proyecto (comandos)
En terminal:

```bash
npm install
npm test
```

**Si no hay proyecto base:** crea rápido (premium):
```bash
npm init -y
npm i express
npm i -D jest supertest
```

Y agrega scripts en `package.json`:

```json
"scripts": {
  "start": "node src/server.js",
  "test": "jest --runInBand",
  "test:cov": "jest --coverage --runInBand"
}
```

---

# 3) Delegación a agente – prompts listos (parte central)

> Nota: aquí puedes usar tu herramienta de agente/antigravity/codex.  
> En la grabación, **solo lee el prompt y muestra el output**, sin enseñar claves.

## 3.1 Prompt 1 – Crear la función de validación + tests
Guárdalo en `docs/PROMPTS.md` (lo lees y lo ejecutas):

```md
## Prompt 1 — validateUser + tests

Actúa como backend senior en Node.js.

Tarea:
- Implementa `validateUser(email, password)` en `src/validators/validateUser.js`.

Restricciones:
- Sin librerías externas.
- Email: regex razonable (no perfecto, pero consistente).
- Password: mínimo 8 chars, 1 número, 1 símbolo.
- Retornar `{ ok: boolean, errors: string[] }`.
- Código modular y legible.

Pruebas:
- Genera tests Jest en `tests/validateUser.test.js`.
- Cobertura mínima objetivo: 70%.
- Incluye casos: válido, email inválido, sin número, sin símbolo, corto.

No generes archivos adicionales fuera de lo pedido.
```

### Checkpoint rápido
En terminal:
```bash
npm run test:cov
```
En pantalla: muestra el porcentaje de coverage.

---

## 3.2 Prompt 2 – Generar server Express + endpoints GET/POST
```md
## Prompt 2 — Express API mínima

Actúa como backend senior.

Crea una API Express mínima en `src/server.js` con:

- GET /users -> retorna lista in-memory (array)
- POST /users -> recibe {email, password}
  - usar validateUser(email, password)
  - si ok: agrega al array y retorna 201
  - si no ok: retorna 400 con {errors}

Restricciones:
- Sin BD (solo memoria).
- Manejo de errores básico.
- Código claro.
- Exporta `app` para pruebas con supertest.

Genera tests en `tests/users.api.test.js`:
- GET devuelve 200 y array
- POST válido devuelve 201
- POST inválido devuelve 400 y errors

No uses librerías adicionales fuera de express/jest/supertest.
```

### Checkpoint
```bash
npm run test:cov
```

---

## 3.3 Prompt 3 – Corrección por fallos (si algo falla en demo)
Si el coverage queda < 70% o hay edge cases:

```md
## Prompt 3 — completar coverage

La suite actual no llega a coverage ≥70% o falta cubrir casos.

Sin cambiar la lógica funcional, agrega tests faltantes para:
- password con espacio
- email con caracteres inválidos
- payload incompleto en POST (sin email o password)

Mantén claridad en nombres de tests.
```

---

# 4) CI/CD: pipeline mínimo “enterprise” (sin humo)

## 4.1 Archivo `.github/workflows/ci.yml`
Pega esto en pantalla y comitea:

```yml
name: CI

on:
  pull_request:
  push:
    branches: [ main ]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: '18'
      - run: npm ci
      - run: npm run test:cov
```

> Premium: agrega lint + audit ligero (si tienes ESLint), pero no lo forces si aún no está en el repo.

## 4.2 Commit y push
```bash
git add .
git commit -m "Sprint: users api + tests + ci"
git push
```

**En pantalla:** abre GitHub → Actions → pipeline verde.

---

# 5) Sprint Review (2–3 minutos, demo de evidencia)

## 5.1 Ejecutar app
```bash
npm start
```

## 5.2 Probar endpoints
En otra terminal:

```bash
curl -s http://localhost:3000/users | jq
```

POST válido (ejemplo):
```bash
curl -s -X POST http://localhost:3000/users   -H "Content-Type: application/json"   -d '{"email":"dev@empresa.com","password":"Passw0rd!"}' | jq
```

POST inválido:
```bash
curl -s -X POST http://localhost:3000/users   -H "Content-Type: application/json"   -d '{"email":"mal","password":"123"}' | jq
```

**Evidencia:** coverage + CI verde + endpoints.

---

# 6) Retrospective (1–2 min, cerrar profesional)

En `docs/RETRO.md` (muestra y lee 3 bullets):

```md
# Retro Sprint 1

## Qué funcionó
- Prompts con restricciones redujeron iteraciones.
- CI forzó DoD real.

## Qué falló / riesgos
- Primera versión no cubrió payload incompleto.
- Necesitamos estandarizar DoR para historias delegables.

## Acciones para el siguiente sprint
- Plantilla fija de historia + criterios + restricciones.
- Añadir lint y security scan ligero.
```

---

# 7) Checklist de finalización (para grabación)

✅ Sprint Backlog visible (docs/SPRINT.md)  
✅ Prompts registrados (docs/PROMPTS.md)  
✅ Tests passing + coverage ≥ 70%  
✅ CI verde en GitHub Actions  
✅ Demo endpoints funcionando  
✅ Retro documentada  

---

# 8) Versión Marketplace vs Premium (qué recortar)

## Marketplace (18–25 min)
- Planning rápido (1 min)
- DoR/DoD en 30 seg
- Prompt 1 + Prompt 2
- Mostrar coverage
- Mostrar CI verde
- Cierre

## Premium (30–40 min)
- Explicar criterios y por qué
- Mostrar 1 fallo real y cómo se corrige
- Añadir Prompt 3
- Retro con métricas y acciones

---

# 9) Recursos para el equipo de edición

- Insertar lower-third: “Unidad 2 – Scrum + IA + Agentes”
- Zoom en:
  - `docs/SPRINT.md`
  - `docs/PROMPTS.md`
  - output de `npm run test:cov`
  - pantalla de GitHub Actions “green”
- Subtítulos en palabras clave:
  - DoR, DoD, Coverage, CI, Supervisión, Delegación

---

Documento listo para grabación: operativo, repetible y verificable.
