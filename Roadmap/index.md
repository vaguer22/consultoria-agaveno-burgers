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

# Roadmap

## Propósito
Organizar la planificación estratégica y táctica del proyecto en un solo lugar: iniciativas, hitos, dependencias y estado. Facilitar priorización, seguimiento y comunicación entre equipos.

---

## Estructura recomendada
- **plans/** — Planes de alto nivel por trimestre o ciclo (objetivos, iniciativas clave, métricas).  
- **epics/** — Epics o iniciativas grandes con descripción, alcance y criterios de éxito.  
- **stories/** — Historias o tareas vinculadas a epics (entregables, responsables, estimación).  
- **milestones/** — Hitos con fecha objetivo y criterios de aceptación.  
- **dependencies/** — Dependencias entre iniciativas y riesgos asociados.  
- **changelog.md** — Registro de cambios en el roadmap.  
- **assets/** — Diagramas, timelines y recursos visuales.

---

## Convención de nombres
**Formato recomendado**  
```text
YYYY-MM-DD_tipo_area_tema_vN.md
Ejemplo: 2026-07-01_plan_q3_product_v1.md
Ejemplo: 2026-07-02_epic_cocina_mejora-flujo-v1.md
Ejemplo: 2026-07-03_story_servicio_reducir-tiempo-v1.md
Ejemplo: 2026-07-04_milestone_lanzamiento_v1.md
```
- **tipo**: `plan` / `epic` / `story` / `milestone` / `dependency`.  
- **area**: producto / operaciones / marketing / finanzas / general.  
- **vN**: versión incremental.

---

## Frontmatter obligatorio (mínimo)
Todos los `.md` en `Roadmap/` deben incluir frontmatter YAML.

```yaml
---
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
---
```

Campos recomendados: `priority` (alta/med/baixa), `metrics`, `dependencies`.

---

## Flujo operativo recomendado (resumido)
1. **Proponer**: crear `plan/` o `epic/` con frontmatter y objetivos claros.  
2. **Priorizar**: asignar `priority`, owner y dependencias; discutir en la reunión de roadmap.  
3. **Desglosar**: crear `stories/` vinculadas al `epic/` con responsables y estimaciones.  
4. **Ejecutar**: mover estado a `in-progress`, actualizar `milestones/` y registrar bloqueos en `dependencies/`.  
5. **Cerrar**: marcar `status: done`, documentar resultados y lecciones en `changelog.md`.  

---

## Buenas prácticas (fáciles de seguir)
1. **Frontmatter primero**: añade metadatos antes de escribir contenido.  
2. **Manténlo corto**: objetivos y criterios de éxito claros en 3–5 líneas.  
3. **Vincula artefactos**: usa `linked_issues` y `linked_prs` para trazabilidad.  
4. **Actualiza el estado**: registra cambios de estado y fechas en cada commit.  
5. **Prioriza visible**: usa `priority` y `target_date` para tomar decisiones rápidas.  
6. **No dupliques**: referencia epics desde stories en lugar de copiar contenido.  
7. **Revisa periódicamente**: agenda revisión de roadmap cada sprint o mes.

---

## Roles y contacto
- **Owner de Roadmap** — mantiene la carpeta y coordina priorización.  
- **Product Owner / Responsable de área** — define objetivos y acepta entregables.  
- **PM / Scrum Master** — desglosa epics en stories y gestiona bloqueos.  
- **Stakeholders** — revisan prioridades y validan hitos.  
- **Soporte técnico** — ayuda con assets y publicación.

**Cómo proponer un cambio:** abrir un *issue* con etiqueta `roadmap`, crear PR con la nueva versión (`vN+1`) y asignar al Owner para revisión.

---
