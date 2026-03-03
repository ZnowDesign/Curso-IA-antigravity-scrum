
# 04_Prompt_Library_Curada_Unidad_1.md

# Prompt Library Curada – Unidad 1  
## AI-Augmented Engineering: Supervisión Estratégica de Agentes  
Nivel: Profesional Avanzado

---

# 1. Propósito

Esta biblioteca contiene prompts estructurados bajo estándares profesionales.

Cada prompt incluye:

- Contexto técnico claro
- Tarea delimitada
- Restricciones explícitas
- Criterios verificables
- Enfoque de supervisión

Estos prompts NO son para copiar sin pensar.  
Son modelos de referencia para delegación controlada.

---

# 2. Prompt – Generación Controlada de Función

## Objetivo:
Implementar validación robusta bajo criterios definidos.

```
Actúa como desarrollador backend senior.

Implementa una función validateUser(email, password) en Node.js.

Requisitos:
- Validar formato correcto de email.
- Password mínimo 8 caracteres.
- Al menos un número.
- Al menos un símbolo.
- No usar librerías externas.
- Código modular y legible.

Incluye:
- Tests con Jest.
- Coverage mínimo 70%.
- Manejo explícito de errores.
- Comentarios técnicos breves.

No generes código adicional innecesario.
```

---

# 3. Prompt – Generación con Restricciones de Arquitectura

```
Actúa como arquitecto de software.

Implementa la función validateUser bajo el patrón separación de responsabilidades.

Requisitos:
- Archivo independiente en carpeta validators.
- No mezclar lógica HTTP con validación.
- Incluir documentación JSDoc.
- Mantener complejidad ciclomática baja.

Incluye pruebas automatizadas.
```

---

# 4. Prompt – Generación de Tests Automáticos

```
Genera pruebas unitarias para la función validateUser.

Cobertura mínima 70%.
Incluir:
- Caso válido.
- Email inválido.
- Password sin número.
- Password sin símbolo.
- Password demasiado corto.

No modificar la función original.
```

---

# 5. Prompt – Refactorización Supervisada

```
Revisa el siguiente código y propone mejoras estructurales.

Objetivos:
- Reducir complejidad.
- Mejorar naming.
- Eliminar duplicación.
- Mantener funcionalidad intacta.

Explica cada mejora propuesta.
No reescribas completamente si no es necesario.
```

---

# 6. Prompt – Auditoría Técnica

```
Analiza este módulo como si fueras revisor técnico.

Evalúa:
- Cumplimiento de criterios.
- Riesgos de seguridad.
- Calidad estructural.
- Posible deuda técnica.

Propón mejoras concretas.
No inventes problemas inexistentes.
```

---

# 7. Prompt – Iteración Correctiva

```
La implementación actual no alcanza 70% de coverage.

Genera los tests faltantes para cumplir el estándar.

No alteres la lógica funcional.
Explica brevemente qué casos faltaban.
```

---

# 8. Prompt – Documentación Técnica

```
Genera documentación técnica en formato README para el módulo validateUser.

Debe incluir:
- Descripción.
- Requisitos.
- Cómo ejecutar pruebas.
- Métricas alcanzadas.
- Limitaciones conocidas.
```

---

# 9. Buenas Prácticas al Usar Estos Prompts

- Nunca delegar sin diseño previo.
- Siempre validar con pruebas.
- Medir coverage.
- Documentar decisiones.
- Iterar si el resultado no cumple estándares.

---

# 10. Señales de Prompt Mal Redactado

- Falta de restricciones.
- Falta de criterios medibles.
- Ambigüedad en responsabilidades.
- No exigir validación automática.

---

Documento oficial para uso profesional en Unidad 1.
