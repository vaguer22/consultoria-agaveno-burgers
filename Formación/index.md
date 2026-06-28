```markdown
date: 2026-06-28
author: Adrian — Responsable de Training
version: v1.2
status: borrador
area: training
summary: Índice operativo para Training; estructura por módulos, frontmatter obligatorio, plantillas, flujo operativo y buenas prácticas simplificadas para crear y mantener materiales de capacitación reproducibles.
linked_issues: []
linked_prs: []
```
---

# Training

## Propósito
Proveer un repositorio organizado y reproducible para **manuales**, **guías rápidas** y **plantillas** de capacitación. Facilitar que cualquier instructor o supervisor encuentre, use y actualice materiales con trazabilidad y control de versiones.

---

## Estructura recomendada (subcarpetas)
- **`manuales/`** — Cursos o módulos completos: objetivos, contenidos, actividades, evaluaciones y recursos.  
- **`quick-guides/`** — Guías cortas y visuales para tareas críticas en piso (paso a paso).  
- **`templates/`** — Plantillas reutilizables: checklists, rúbricas, plan de sesión, evaluaciones.  
- **`assets/`** — Imágenes, videos y archivos multimedia asociados.  
- **`changelog.md`** — Registro de cambios en materiales de capacitación.

---

## Convención de nombres
**Formato recomendado**  
```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-07-10_manual_cocina_armado-hamburguesa_v1.md
Ejemplo: 2026-07-10_quickguide_servicio_apertura-turno_v1.pdf
Ejemplo: 2026-07-10_template_checklist_entrega_v1.md
```
- **tipo**: `manual` / `quickguide` / `template`.  
- **area**: cocina / barra / servicio / delivery / admin.  
- **tema**: nombre corto de la tarea o módulo.  
- **vN**: versión incremental.

---

## Frontmatter obligatorio (mínimo)
Todos los `.md` deben incluir frontmatter YAML antes de editar.

```yaml
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: borrador / aprobado / final
area: cocina / barra / servicio / delivery / admin
duration: 1h / 2h / 1 día   # opcional para manuales
audience: personal nuevo / supervisores / todos
summary: Breve descripción del material
linked_issues: []
linked_prs: []
```

---

**Consejo:** para manuales largos añade `learning_objectives`, `prerequisites` y `assessment_method`.

---

## Plantillas mínimas (qué debe contener cada tipo)
### Manual (estructura mínima)
- **Portada**: título, versión, autor, duración.  
- **Objetivos de aprendizaje**: 3–5 objetivos claros.  
- **Contenido**: secciones con pasos y ejemplos.  
- **Actividades prácticas**: ejercicios o simulaciones.  
- **Evaluación**: criterios y rúbrica.  
- **Recursos**: enlaces, archivos y assets.  
- **Registro de cambios**: breve historial al final.

### Quick-guide (estructura mínima)
- **Título y propósito** (1 línea).  
- **Pasos numerados** (máx. 8 pasos).  
- **Checklist rápido** (sí/no).  
- **Tiempo estimado**.  
- **Contacto** (quién preguntar si hay dudas).

### Template (ejemplos)
- **Checklist de apertura**: pasos, responsable, firma.  
- **Rúbrica de evaluación**: criterios y puntajes.  
- **Plan de sesión**: tiempo, actividades, recursos.

---

## Flujo operativo recomendado (resumido)
1. **Crear**: duplicar la plantilla desde `templates/` y completar frontmatter.  
2. **Revisar**: enviar PR o compartir borrador con un instructor y un supervisor.  
3. **Probar**: aplicar el material en una sesión piloto (si aplica) y recoger feedback.  
4. **Aprobar**: marcar `status: aprobado` y actualizar `changelog.md`.  
5. **Publicar**: mover versión final a `manuales/` o `quick-guides/` y subir assets.  
6. **Revisar periódicamente**: programar revisión según `next_review` o cada 6–12 meses.

---

## Buenas prácticas operativas (fáciles de entender)
1. **Frontmatter primero**: siempre añade el frontmatter mínimo antes de escribir.  
2. **Usa plantillas**: evita formatos libres; parte de `templates/`.  
3. **Hazlo práctico**: prioriza pasos claros, ejemplos y checklists.  
4. **Versiona**: no sobrescribas; crea `vN+1` y anota el motivo en `changelog.md`.  
5. **Prueba en campo**: valida guías con al menos una sesión real antes de publicar.  
6. **Adjunta assets**: fotos o videos cortos en `assets/` y referencia en el documento.  
7. **Lenguaje simple**: oraciones cortas, verbos en imperativo y listas numeradas.  
8. **Accesibilidad**: usa títulos claros, texto legible y alternativas para multimedia.

---

## Evaluación y medición del impacto
- **Indicadores simples**: tasa de aprobación en evaluación, tiempo promedio de ejecución, número de incidencias tras capacitación.  
- **Registro**: guardar resultados de evaluaciones en `manuales/` o en `templates/assessment-results/` con `kpi_id` si aplica.  
- **Mejora continua**: actualizar materiales según feedback y resultados medibles.

---

## Ejemplos de nombres de archivo
- `manuales/2026-07-10_manual_cocina_armado-hamburguesa_v1.md`  
- `quick-guides/2026-07-10_quickguide_servicio_apertura-turno_v1.pdf`  
- `templates/2026-07-10_template_checklist_entrega_v1.md`  
- `assets/2026-07-10_img_armado-hamburguesa_v1.jpg`

---

## Roles y contacto
- **Coordinador de Training** — mantiene la carpeta y valida materiales.  
- **Instructores** — crean y prueban manuales y guías.  
- **Supervisores** — aplican y validan en campo.  
- **Soporte técnico** — gestiona assets multimedia y publicación.

**Cómo solicitar un cambio:** abrir un *issue* con etiqueta `training`, adjuntar la propuesta y referenciar el archivo afectado.
