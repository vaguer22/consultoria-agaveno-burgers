```
date: 2026-06-28
author: Adrian — Responsable de Roadmap
version: v1.0
status: borrador
area: roadmap
summary: Índice operativo para Roadmap; estructura, frontmatter mínimo, convenciones de nombres, flujo operativo y buenas prácticas simplificadas para planificar y rastrear iniciativas.
linked_issues: []
linked_prs: []
```

---

## Convención de nombres
**Formato recomendado**  
```
YYYY-MM-DD_tipo_area_tema_vN.md
Ejemplo: 2026-07-02_epic_cocina_mejora-flujo-v1.md

- **tipo**: `plan` / `epic` / `story` / `milestone` / `dependency`.  
- **area**: producto / operaciones / marketing / finanzas / general.  
- **vN**: versión incremental.
```
---


## Frontmatter (mínimo)
Todos los .md en Roadmap/ deben incluir frontmatter YAML.

```
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: proposed / in-progress / blocked / done
area: producto / operaciones / marketing / finanzas / general
document_id: RD-YYYYMMDD-01
summary: Breve descripción del plan o iniciativa
owner: Nombre — Rol
target_date: YYYY-MM-DD   # opcional para hitos
linked_issues: []
linked_prs: []
```

Campos recomendados: priority (alta/med/baixa), metrics, dependencies.
