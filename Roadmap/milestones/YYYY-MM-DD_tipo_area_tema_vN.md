## Convención de nombres
**Formato recomendado**  
```
YYYY-MM-DD_tipo_area_tema_vN.md
Ejemplo: 2026-07-04_milestone_lanzamiento_v1.md
```

- **tipo**: `plan` / `epic` / `story` / `milestone` / `dependency`.  
- **area**: producto / operaciones / marketing / finanzas / general.  
- **vN**: versión incremental.

---

## Frontmatter obligatorio (mínimo)
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

Campos recomendados: `priority` (alta/med/baixa), `metrics`, `dependencies`.
