
# 02_LAB_GUIDE_Unidad_1.md

# Laboratorio Formal – Unidad 1  
## AI-Augmented Engineering: Supervisión Estratégica de Agentes

---

# 1. Objetivo del Laboratorio

Aplicar el modelo **AI-Augmented Engineering** mediante delegación controlada a un agente IA, validando el resultado con métricas técnicas objetivas.

Este laboratorio evalúa la capacidad de:

- Diseñar antes de delegar.
- Redactar prompts estructurados.
- Validar con pruebas automatizadas.
- Supervisar calidad técnica.
- Iterar estratégicamente.

---

# 2. Contexto Profesional

Escenario:

Una startup necesita implementar validación robusta de usuarios para su API REST.

El equipo decide utilizar un agente IA para acelerar la implementación.

Tu rol no es generar código manualmente.  
Tu rol es **supervisar al agente** y garantizar calidad profesional.

---

# 3. Historia Scrum Asociada

**Historia:**  
Como sistema, necesito validar usuarios para garantizar seguridad en el registro.

**Criterios de aceptación:**

- Email válido.
- Password mínimo 8 caracteres.
- Password con número y símbolo.
- Respuesta HTTP adecuada en caso de error.
- Tests automatizados incluidos.

---

# 4. Definition of Ready

Antes de delegar:

- [ ] Historia clara.
- [ ] Criterios de aceptación definidos.
- [ ] Edge cases identificados.
- [ ] Restricciones técnicas establecidas.
- [ ] Métrica de coverage definida (≥ 70%).

---

# 5. Setup Técnico

1. Clonar repositorio template.
2. Instalar dependencias:

```
npm install
```

3. Ejecutar pruebas base:

```
npm run test:cov
```

4. Confirmar entorno funcional.

---

# 6. Paso 1 – Diseño Técnico

Antes de escribir cualquier prompt:

Documentar:

- Qué hace la función.
- Qué inputs recibe.
- Qué outputs retorna.
- Qué errores debe manejar.
- Qué casos límite existen.

Crear archivo:

```
docs/design-notes.md
```

---

# 7. Paso 2 – Redacción del Prompt Profesional

Debe incluir:

- Contexto técnico.
- Tarea delimitada.
- Restricciones explícitas.
- Criterios de aceptación verificables.

Ejemplo base:

“Implementa una función validateUser(email, password) en Node.js.
Debe incluir validación estricta.
Debe generar tests con Jest.
Cobertura mínima 70%.
Sin librerías externas.”

Guardar el prompt en:

```
docs/prompt-used.md
```

---

# 8. Paso 3 – Generación y Supervisión

Después de generar código:

Validar:

- ¿Cumple criterios?
- ¿Está modularizado?
- ¿Está documentado?
- ¿Tests cubren casos críticos?

Si no cumple → iterar prompt.

Registrar iteraciones.

---

# 9. Paso 4 – Validación Técnica

Ejecutar:

```
npm run test:cov
```

Verificar:

- Coverage ≥ 70%
- Sin errores de lint
- CI verde

Si falla → corregir.

---

# 10. Entregables Obligatorios

Subir repositorio que incluya:

- Código funcional.
- Tests automatizados.
- Coverage report.
- Prompt documentado.
- Documento de diseño.
- Evidencia CI.
- README actualizado.

---

# 11. Métricas de Evaluación

| Criterio | Requisito |
|-----------|-----------|
| Coverage | ≥ 70% |
| CI | Verde |
| Prompt | Estructurado |
| Código | Modular |
| Documentación | Clara |

---

# 12. Errores Comunes

- Delegar sin diseñar.
- Prompt ambiguo.
- Aceptar código sin pruebas.
- Ignorar métricas.
- No iterar cuando falla.

---

# 13. Reflexión Técnica

Responder:

1. ¿Qué error cometió el agente inicialmente?
2. ¿Qué mejoraste en tu segundo prompt?
3. ¿Qué aprendiste sobre supervisión?

Máximo 400 palabras.

---

# 14. Criterio de Aprobación

Para aprobar:

- Nivel mínimo 3 en rúbrica.
- Coverage ≥ 70%.
- CI verde.
- Prompt documentado.
- Evidencia de supervisión real.

---

Laboratorio obligatorio para validación de competencia profesional.
