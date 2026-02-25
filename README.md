# 🐪 El Camello

### The Office, pero colombiano. Y con IA.

> 16 empleados de IA. 5 pisos. 0 vacaciones. Un PM adicto al tinto.  
> Un CEO (tú) que aprueba todo con el dedo índice.

🔗 **[Ver la Demo en Vivo →](https://ingjaviergomezm.github.io/el-camello/)**

---

## 🤔 ¿Qué es esto?

Bueno, si llegaste hasta aquí, es porque ya manejas la IAG, tienes una cuenta de Gemini Pro, tienes instalado **Antigravity** y quieres potenciar tu productividad **x10**.

*El Camello* es un sistema de **16 agentes de IA especializados** (llamados *Skills*) organizados como una oficina corporativa colombiana de 5 pisos. Cada "empleado" tiene un rol específico, una personalidad definida (y algo de humor negro), y la capacidad de ejecutar tareas profesionales complejas — desde crear un pitch deck para inversionistas hasta construir una webapp completa en React.

**¿Y por qué "El Camello"?** Porque en Colombia, *"el camello"* es *el trabajo*. Y aquí, la IA trabaja mientras el humano vibea. ☕

---

## 🧩 Espera... ¿Qué es Antigravity?

**Antigravity** es una extensión de VS Code creada por Google DeepMind que te da acceso a un agente de IA avanzado (basado en Gemini) directamente en tu editor de código. Piensa en él como un compañero de trabajo que:

- Lee tu código y tus archivos
- Ejecuta comandos en tu terminal
- Navega la web por ti
- Crea, edita y organiza documentos
- Y lo más importante: **puede usar Skills** (módulos especializados) para tareas específicas

Es como tener un dev senior disponible 24/7, pero que además sabe hacer presentaciones, escribir documentos y diseñar interfaces. Sin preguntas pasivo-agresivas.

---

## 🔌 ¿Y qué es un MCP?

**MCP** (Model Context Protocol) es un estándar que le permite a la IA conectarse con herramientas y servicios externos. Imagina que la IA es un celular — el MCP son las apps que le instalas para que tenga superpoderes.

Por ejemplo:
- Un MCP de GitHub le permite crear repos y hacer commits
- Un MCP de Stitch le permite diseñar interfaces
- Un MCP custom que tú construyas le permite hablar con TU base de datos

**El Camello usa Skills** (no MCPs directamente), pero el agente `mcp-builder` del Piso 5 puede **construir MCPs nuevos** si los necesitas. Sí, tus empleados pueden contratar herramientas.

---

## 🏢 ¿Qué son las Skills?

Una **Skill** es un archivo Markdown (`SKILL.md`) que le dice a Antigravity **cómo hacer algo específico**. Es como darle un manual de procedimientos a un empleado nuevo.

Cada Skill contiene:
- **Nombre y descripción** (para que Antigravity la encuentre automáticamente)
- **Instrucciones paso a paso** (qué hacer, en qué orden)
- **Referencias opcionales** (archivos adicionales, templates, ejemplos)

Cuando le pides algo a Antigravity y coincide con una Skill instalada, él la lee y la sigue al pie de la letra. Es como si le hubieras entrenado un especialista nuevo en 0.5 segundos.

---

## 🏗️ El Organigrama — Quién es quién en El Camello

```
                        🏢 EL CEO (Tú)
                     Aprueba todo con el dedo índice
                              │
                        ☕ MASTER-ORCHESTRATOR
                     El PM que agenda reuniones sobre reuniones
                              │
          ┌───────────┬───────┴───────┬───────────┬──────────┐
          │           │               │           │          │
     🧠 PISO 5   🎨 PISO 4      🤓 PISO 3   👔 PISO 2  🏗️ PISO 1
    Ingeniería    Diseño        Documentos   Ejecutiva    RRHH
```

### Piso 5 — Los Cerebritos de Ingeniería 🧠
| Empleado | Qué hace | Ejemplo rápido |
|----------|----------|----------------|
| `mcp-builder` | Construye puentes entre la IA y APIs/DBs | *"Conecta mi app a mi base de datos de PostgreSQL"* |
| `web-artifacts-builder` | Crea webapps completas en un solo archivo | *"Haz un dashboard"* |
| `webapp-testing` | QA automatizado con Playwright | *"Revisa que todos los botones funcionen"* |
| `algorithmic-art` | Arte generativo con p5.js | *"Haz un flow field interactivo"* |

### Piso 4 — Los Diseñadores Hipsters 🎨
| Empleado | Qué hace | Ejemplo rápido |
|----------|----------|----------------|
| `brand-father` | Define tu identidad visual (Brand Book) | *"Crea un Brand Book para mi startup"* |
| `theme-factory` | 10 temas pre-diseñados profesionales | *"Aplícale un tema bonito a esta presentación"* |
| `canvas-design` | Arte visual calidad museo | *"Diseña un póster premium para mi evento"* |

### Piso 3 — Los Geeks y Contadores 🤓
| Empleado | Qué hace | Ejemplo rápido |
|----------|----------|----------------|
| `xlsx` | Excel avanzado: fórmulas, gráficos, limpieza | *"Limpia este CSV de 50,000 registros"* |
| `docx` | Word profesional con estilos reales | *"Genera un contrato con tabla de contenido"* |
| `pptx` | Presentaciones nivel McKinsey | *"Arma un pitch deck de 15 slides"* |
| `pdf` | Merge, split, OCR, watermarks | *"Combina estos 10 PDFs y ponles watermark"* |

### Piso 2 — Suite Ejecutiva 👔
| Empleado | Qué hace | Ejemplo rápido |
|----------|----------|----------------|
| `reuniones-summary` | Transforma transcripciones en minutas | *"Resume esta reunión de 1 hora"* |
| `doc-coauthoring` | Co-creación iterativa de documentos | *"Ayúdame a escribir un RFC técnico"* |
| `internal-comms` | Comunicaciones corporativas | *"Redacta un 3P Update para el equipo"* |

### Piso 1 — Recursos Humanos 🏗️
| Empleado | Qué hace | Ejemplo rápido |
|----------|----------|----------------|
| `skill-forge` | Crea Skills nuevas desde cero | *"Necesito un empleado que haga X"* |

---

## ⚡ ¿Cómo potencia tu productividad?

Sin El Camello:
```
Tú: Necesito un reporte en Word, una presentación, y subirlo a la web.
[3 horas después, 47 pestañas abiertas, 2 cafés derramados]
```

Con El Camello:
```
Tú: "Necesito un reporte en Word, una presentación, y subirlo a la web."
PM: Detectado proyecto complejo. Equipo: docx + pptx + web-artifacts-builder.
PM: Plan de 3 fases. ¿Apruebas, CEO?
Tú: Dale.
[15 minutos después, todo entregado con QA incluido]
```

El orquestador **detecta la complejidad**, **selecciona las Skills necesarias**, y **ejecuta las fases** pidiéndote aprobación en cada checkpoint. Tú solo apruebas o iteras.

---

## 🚀 Instalación — ¡Al grano!

### Prerrequisitos
- ✅ [VS Code](https://code.visualstudio.com/) instalado
- ✅ [Antigravity](https://marketplace.visualstudio.com/items?itemName=Google.antigravity) instalado y configurado
- ✅ Cuenta de Gemini Pro activa
- ✅ Ganas de ser productivo (esto es lo más difícil)

### Paso 1: Habilitar acceso a archivos

Abre Antigravity y ve a **Settings** (la tuerca ⚙️):

```
Agent Non-Workspace File Access → ✅ HABILITADO
```

> ⚠️ **Sin esto, Antigravity no puede leer las Skills.** Es como contratar empleados y no dejarlos entrar a la oficina.

### Paso 2: Configurar la estructura

Las Skills van en esta ruta específica. **Esto es sagrado, no lo toques:**

```
~/.gemini/antigravity/
├── skills/                          ← Aquí van todos los empleados
│   ├── algorithmic-art/
│   │   └── SKILL.md
│   ├── brand-father/
│   │   └── SKILL.md
│   ├── canvas-design/
│   │   └── SKILL.md
│   ├── doc-coauthoring/
│   │   ├── SKILL.md
│   │   └── references/
│   │       └── reader-testing.md
│   ├── docx/
│   │   └── SKILL.md
│   ├── internal-comms/
│   │   └── SKILL.md
│   ├── master-orchestrator/         ← El PM cafeinómano
│   │   ├── SKILL.md
│   │   └── references/
│   │       └── capabilities-registry.md
│   ├── mcp-builder/
│   │   └── SKILL.md
│   ├── pdf/
│   │   └── SKILL.md
│   ├── pptx/
│   │   └── SKILL.md
│   ├── reuniones-summary/
│   │   └── SKILL.md
│   ├── skill-forge/
│   │   └── SKILL.md
│   ├── theme-factory/
│   │   └── SKILL.md
│   ├── web-artifacts-builder/
│   │   └── SKILL.md
│   ├── webapp-testing/
│   │   └── SKILL.md
│   └── xlsx/
│       └── SKILL.md
└── workflows/                       ← Opcional, para automatizaciones
```

### Paso 3: Copiar y pegar — ¡Voilá!

Abre Antigravity (Ctrl+Shift+P → "Antigravity: Open") y pega este prompt:

```
Necesito que instales el sistema de Skills "El Camello" en mi entorno.

1. Clona o descarga las Skills desde: https://github.com/ingjaviergomezm/el-camello
2. Copia la carpeta `skills/` completa a la ruta `~/.gemini/antigravity/skills/`
3. Verifica que cada skill tenga su `SKILL.md` válido
4. El orquestador principal es `master-orchestrator/SKILL.md`
5. Habilita "Agent Non-Workspace File Access" si no está habilitado

Una vez instalado, pregúntame qué proyecto quiero hacer.
Tú eres el PM. Yo soy el CEO. Nadie se mueve sin mi aprobación. ☕
```

**Eso es todo.** Antigravity leerá las Skills automáticamente y las usará cuando detecte que las necesita. Es plug & play.

---

## 🎮 Primeras pruebas — Ponlo a trabajar

Una vez instalado, prueba estos comandos para ver a los empleados en acción:

### Test rápido (1 skill)
```
"Crea un archivo Excel con los meses del año, un presupuesto de ejemplo
y un gráfico de barras. Ponlo bonito."
```
→ El `xlsx` del Piso 3 se activa. Si tienes un Brand Book, lo respeta.

### Test complejo (multi-skill)
```
"Necesito un reporte en Word sobre el estado del proyecto X,
una presentación de 10 slides con los highlights,
y una landing page simple para compartirlo con el equipo."
```
→ El PM se activa, detecta complejidad ALTA, arma un equipo de 3 Skills, y te va pidiendo aprobación en cada entrega.

### Test de diseño
```
"Crea un Brand Book para mi empresa 'TechVerde'.
Colores: verdes y grises. Tipografía moderna."
```
→ El `brand-father` del Piso 4 te entrevista, crea el Brand Book, y de ahí en adelante TODOS los documentos respetan tu marca.

---

## 🧠 Tips del CEO veterano

1. **"El PM es tu aliado, no tu enemigo."** Si te pide aprobación, es porque quiere que el resultado sea bueno. Aprueba rápido o itera con feedback concreto.

2. **"Las Skills se descubren solas."** No necesitas invocarlas manualmente. Solo pide lo que necesitas y Antigravity encuentra la Skill correcta.

3. **"Brand First."** Si creas un Brand Book primero, TODOS los documentos posteriores respetarán tu identidad visual automáticamente. Es como vestir la oficina con tu logo.

4. **"Si no existe el empleado, créalo."** El `skill-forge` del Piso 1 puede fabricar Skills nuevas en minutos. ¿Necesitas un agente que genere facturas? Pídeselo.

5. **"Revisa el organigrama."** Si no sabes qué agente hace qué, abre la [demo interactiva](https://ingjaviergomezm.github.io/el-camello/) y haz click en el tab "Organigrama".

---

## 📁 Estructura del repo

```
el-camello/
├── index.html          ← Dashboard interactivo (GitHub Pages demo)
├── README.md           ← Este archivo
├── skills/             ← Las 16 Skills + el orquestador
│   ├── master-orchestrator/
│   │   ├── SKILL.md
│   │   └── references/
│   ├── skill-forge/
│   │   └── SKILL.md
│   ├── ... (14 más)
│   └── xlsx/
│       └── SKILL.md
└── LICENSE
```

---

## 🤝 Créditos

**Vibecodeado con amor, tinto colombiano y una cantidad cuestionable de `npm install`.**

| Rol | Quién |
|-----|-------|
| 🏢 CEO & Arquitecto | [Javier Gómez](https://github.com/ingjaviergomezm) · [LinkedIn](https://www.linkedin.com/in/jogomezm/) |
| ☕ PM Cafeinómano | `master-orchestrator` (el agente que agenda reuniones sobre reuniones) |
| ⚛️ Frontend | `web-artifacts-builder` (el que npm instala hasta el agua) |
| 🔍 QA | `webapp-testing` (el que te encuentra bugs el viernes a las 5pm) |

> *"Ninguna IA fue maltratada durante la producción de este proyecto. Bueno, quizás un poco."*  
> — El PM, tomando su tinto #47 del día ☕

---

## 📄 Licencia

MIT — Úsalo, modifícalo, revéndelo, regálalo. Solo no digas que lo hiciste solo. 😉
