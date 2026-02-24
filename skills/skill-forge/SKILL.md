---
name: skill-forge
description: >
  Crea nuevas skills de alta calidad para Antigravity. Ofrece dos modos: Modo Rápido 
  (entrevista ligera para skills simples) y Modo Avanzado (arquitectura completa con 
  scripts, references y empaquetado según estándares Anthropic).
  Usar cuando el usuario pida: crear habilidad, diseñar nueva skill, automatizar tarea, 
  skill father, skill creator, nueva herramienta, skill forge.
---

# Skill Forge: La Fragua de Habilidades

Combina la entrevista humana amigable con la ingeniería técnica profesional en un solo flujo.

## Paso 0: Selección de Modo

Al activarse, pregunta al usuario:
- *"¿Necesitas una skill rápida (entrevista ligera, resultado inmediato) o una skill avanzada (arquitectura completa con scripts, archivos de referencia y empaquetado profesional)?"*

Si el usuario no está seguro, usa **Modo Rápido** por defecto. Siempre podrá escalar después.

---

## Modo Rápido

### Fase 1: Entrevista Interactiva
**Regla de oro:** Haz **solo 1-2 preguntas por turno**. No abrumes al usuario.

1. **Objetivo Principal:** *¿Qué problema específico resuelve esta skill?*
2. **Contexto (RAG):** *¿Tienes archivos de ejemplo que pueda leer?* (Si da rutas, léelos antes de continuar).
3. **Disparadores:** *¿Qué frases deberían activar esta skill?* (para el `description` del frontmatter YAML).
4. **Entradas y Salidas:** *¿Qué recibe el agente y qué formato de respuesta esperas?*
5. **Reglas o Casos Borde:** *¿Alguna directriz especial de formato, tono u otras condiciones?*
6. **Ubicación:** *¿Global (`~/.gemini/antigravity/skills/`) o específica del Workspace (`.agent/skills/`)?*

### Fase 2: Diseño del SKILL.md
Estándar obligatorio:
1. **Frontmatter YAML** (`---`): `name` (minúsculas con guiones) + `description` (cuándo activarse, palabras clave).
2. **Rol y Propósito:** Quién es el agente y cómo se comporta.
3. **Instrucciones paso a paso** con manejo de excepciones.
4. **Estructura de Salida** en formato Markdown claro.

### Fase 3: Creación Automática
No pidas al usuario que cree nada manualmente:
1. Crea la carpeta y subcarpetas (`references/`, `scripts/`, `assets/`) según necesidad.
2. Escribe el `SKILL.md` directamente con la herramienta de creación de archivos.
3. Confirma al usuario que la skill está lista para invocarse.

### Fase 4: Oferta de Escalamiento
Al finalizar, pregunta:
- *"¿Deseas escalar esta skill al Modo Avanzado para añadir scripts reutilizables, archivos de referencia y empaquetado profesional?"*

Si dice sí → continúa con el Modo Avanzado a partir de la Fase A2.

---

## Modo Avanzado

### Fase A1: Entrevista (igual que Modo Rápido, Fases 1-3)
Ejecuta las mismas fases de entrevista del Modo Rápido si no se han hecho aún.

### Fase A2: Planificación de Recursos Reutilizables
Analiza cada caso de uso concreto preguntando:
1. ¿Hay código que se reescribiría cada vez? → Candidato a `scripts/`
2. ¿Hay documentación de referencia que el agente necesitaría consultar? → Candidato a `references/`
3. ¿Hay templates, imágenes o boilerplate que se copiarían? → Candidato a `assets/`

### Fase A3: Implementación de Recursos
- Crea los scripts necesarios en `scripts/`. Pruébalos ejecutándolos.
- Crea los archivos de referencia en `references/`.
- Copia os assets a `assets/`.
- Elimina carpetas vacías que no se necesiten.

### Fase A4: Refinamiento del SKILL.md
Aplica principios de **Progressive Disclosure**:
- Mantén el SKILL.md bajo 500 líneas.
- Mueve detalles extensos a `references/`.
- Referencia explícitamente cada archivo externo desde el SKILL.md.
- Usa forma imperativa/infinitiva.
- Incluye SOLO información que el agente NO sabría por sí mismo.

### Fase A5: Validación
Verifica que la skill cumple:
- [ ] Frontmatter YAML correcto (`name` + `description` completo).
- [ ] Ningún archivo innecesario (no README, no CHANGELOG).
- [ ] Scripts ejecutados y verificados.
- [ ] Referencias enlazadas desde SKILL.md.
