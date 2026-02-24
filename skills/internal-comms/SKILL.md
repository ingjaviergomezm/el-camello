---
name: internal-comms
description: A set of resources to help me write all kinds of internal communications, using the formats that my company likes to use. Claude should use this skill whenever asked to write some sort of internal communications (status reports, leadership updates, 3P updates, company newsletters, FAQs, incident reports, project updates, etc.).
license: Complete terms in LICENSE.txt
---

## When to use this skill
To write internal communications, use this skill for:
- 3P updates (Progress, Plans, Problems)
- Company newsletters
- FAQ responses
- Status reports
- Leadership updates
- Project updates
- Incident reports

## How to use this skill

To write any internal communication:

1. **Identify the communication type** from the request
2. **Load the appropriate guideline file** from the `examples/` directory:
    - `examples/3p-updates.md` - For Progress/Plans/Problems team updates
    - `examples/company-newsletter.md` - For company-wide newsletters
    - `examples/faq-answers.md` - For answering frequently asked questions
    - `examples/general-comms.md` - For anything else that doesn't explicitly match one of the above
3. **Follow the specific instructions** in that file for formatting, tone, and content gathering

If the guideline file doesn't exist or the type doesn't match, use these **inline fallbacks**:

### Fallback: 3P Update
```
## Progress (Lo que se logró)
- [Logro 1]
## Plans (Lo que viene)
- [Plan 1]
## Problems (Bloqueos)
- [Problema 1] → Acción propuesta: [Solución]
```

### Fallback: Status Report
```
## Estado General: 🟢 En camino / 🟡 En riesgo / 🔴 Bloqueado
## Hitos Completados: [Lista]
## Próximos Hitos: [Lista con fechas]
## Riesgos y Mitigaciones: [Lista]
```

## Keywords
3P updates, company newsletter, company comms, weekly update, faqs, common questions, updates, internal comms
