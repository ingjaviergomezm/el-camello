# Registro de Capacidades: Antigravity HQ

Referencia rápida para el orquestador. Consultar antes de seleccionar el escuadrón.

## Fábrica Meta (Creación de Skills)

| Skill | Output | Interactiva | Dependencias |
|-------|--------|:-----------:|-------------|
| `skill-forge` | SKILL.md + carpetas | Sí (entrevista) | Ninguna |

## Suite Ejecutiva y Comunicaciones

| Skill | Output | Interactiva | Dependencias |
|-------|--------|:-----------:|-------------|
| `reuniones-summary` | Markdown | No | Ninguna |
| `doc-coauthoring` | .md / .docx | Sí (3 fases) | Ninguna |
| `internal-comms` | Markdown | No | `examples/` |

## Suite Ofimática y Analítica

| Skill | Output | Interactiva | Dependencias |
|-------|--------|:-----------:|-------------|
| `xlsx` | .xlsx / .csv | No | Ninguna |
| `docx` | .docx | No | `brand-*` (si existe) |
| `pptx` | .pptx | No (QA sí) | `brand-*` o `theme-factory` |
| `pdf` | .pdf | No | Ninguna |

## Arte y Diseño

| Skill | Output | Interactiva | Dependencias |
|-------|--------|:-----------:|-------------|
| `brand-father` | SKILL.md (`brand-*`) | Sí (entrevista) | Ninguna |
| `theme-factory` | Estilos aplicados | Sí (selección) | NO usar si existe `brand-*` |
| `canvas-design` | .pdf / .png + .md | No | `brand-*` (si existe) |

## Escuadrón de Ingeniería

| Skill | Output | Interactiva | Dependencias |
|-------|--------|:-----------:|-------------|
| `mcp-builder` | Servidor MCP | Sí (fases) | Ninguna |
| `web-artifacts-builder` | .html (bundle) | No | Ninguna |
| `webapp-testing` | Informe QA | No | Servidor corriendo |
| `algorithmic-art` | .html + .md | No | Ninguna |

## Reglas de Precedencia
1. **`brand-*`** siempre tiene prioridad sobre `theme-factory`.
2. Skills interactivas **no pueden ejecutarse en paralelo**; requieren turnos del usuario.
3. Para entregables visuales (docx, pptx, pdf, canvas-design), verificar si existe un `brand-*` ANTES de generar.
