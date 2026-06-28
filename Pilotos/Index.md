```
date: 2026-06-28
author: Adrian — Responsable de Pilotos
version: v1.1
status: borrador
area: pilots
summary: Índice operativo para Pilots; estructura por fases, frontmatter obligatorio, convenciones de nombres y buenas prácticas simplificadas para ejecutar pilotos reproducibles y trazables.
linked_issues: []
linked_prs: []
```

# Pilots

## Propósito
Proveer un espacio controlado para diseñar, ejecutar, analizar y decidir sobre pruebas piloto antes de su escalado. Garantizar **reproducibilidad**, **trazabilidad** y **evidencia** para la toma de decisiones.

---

## Estructura recomendada (decisión: usar subcarpetas)
- **`design/`** — Diseño del piloto: hipótesis, objetivos, criterios de éxito y plan de recolección.  
- **`execution/`** — Registros de ejecución: cronogramas, checklists, incidencias, fotos y datos crudos (`execution/data/raw/`).  
- **`analysis/`** — Datos procesados, scripts/notebooks, gráficos y conclusiones (`analysis/code/`, `analysis/exports/`).  
- **`decision/`** — Informe de recomendación: aprobado / ajustar y re-pilotar / descartado.  
- **`closure/`** — Documentación de cierre: lecciones aprendidas y transferencia a SOPs.  
- **`templates/`** — Plantillas para cada fase (usar `Estándares/templates/` como fuente única).  
- **`changelog.md`** — Registro de cambios y versiones del piloto.  
- **`assets/`** — Imágenes y multimedia optimizados relacionados al piloto.

---

## Convención de nombres
**Formato recomendado**  
```text
YYYY-MM-DD_fase_pilot_area_tema_vN.ext
Ejemplo: 2026-07-01_design_pilot_cocina_tiempo-armado_v1.md
```
**Campos clave**: fecha; fase (design/execution/analysis/decision/closure); `pilot` literal; área; tema; versión `vN`.

---

## Frontmatter obligatorio (mínimo)
Todos los `.md` en `Pilots/` y subcarpetas deben incluir frontmatter YAML.

```yaml
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: borrador / en-ejecucion / final / aprobado
area: cocina / barra / servicio / delivery / producto
pilot_id: PIL-YYYYMMDD-01
phase: design / execution / analysis / decision / closure
summary: Hipótesis y objetivo del piloto
metrics: ["KPI-YYYYMMDD-01"]
linked_issues: []
linked_prs: []
```

Campos opcionales recomendados: `sample_size`, `duration_days`, `responsible`, `source_files`.

---

## Plantillas mínimas por fase
- **Design**: `title`, `pilot_id`, `hypothesis`, `objectives`, `success_criteria`, `metrics`, `sample_size`, `duration`, `data_plan`, `risks`.  
- **Execution**: `run_id`, `date`, `checklist`, `incidents`, `data_files` (referenciados en frontmatter).  
- **Analysis**: `data_sources`, `transformations`, `kpi_results`, `visuals`, `conclusions`.  
- **Decision**: `summary_executive`, `result_vs_criteria`, `recommendation`, `next_steps`.  
- **Closure**: `lessons_learned`, `sop_changes`, `handover_items`.

---

## Flujo operativo recomendado (resumido)
1. **Diseñar** en `design/` con hipótesis, KPIs y plan de datos.  
2. **Aprobar** el diseño vía issue/PR y registrar `linked_issues`/`linked_prs`.  
3. **Ejecutar** y guardar datos crudos en `execution/data/raw/`; registrar incidencias.  
4. **Analizar** en `analysis/` con scripts reproducibles; documentar resultados.  
5. **Decidir** en `decision/` con recomendación clara.  
6. **Cerrar** en `closure/` con lecciones y actualización de SOPs si aplica.

---

## Buenas prácticas operativas (fáciles de entender)
1. **Identifica**: define claramente la hipótesis y los KPIs antes de empezar.  
2. **Registra**: guarda todos los datos crudos y fotos; no los modifiques.  
3. **Documenta**: anota cambios, incidencias y versiones en cada fase.  
4. **Reproduce**: incluye los scripts y pasos para que otro pueda repetir el análisis.  
5. **Decide con evidencia**: compara resultados contra los criterios de éxito y escribe la recomendación.  
6. **Cierra y transfiere**: si se aprueba, actualiza los SOPs; si no, documenta lecciones.

---

## Ejemplos de nombres de archivo por fase
- `design/2026-07-01_design_pilot_cocina_tiempo-armado_v1.md`  
- `execution/2026-07-05_ejecucion_pilot_cocina_tiempo-armado_run1_v1.md`  
- `analysis/2026-07-12_analisis_pilot_cocina_tiempo-armado_v1.md`  
- `decision/2026-07-15_decision_pilot_cocina_tiempo-armado_recomendacion_v1.md`  
- `closure/2026-07-20_cierre_pilot_cocina_tiempo-armado_lecciones_v1.md`

---

## Trazabilidad y control de versiones
- Usa `pilot_id` en todos los archivos relacionados.  
- Incrementa `vN` cuando cambie el diseño o la metodología.  
- Mantén `changelog.md` actualizado con motivos de cambio.

---

## Privacidad y datos
- **No subir PII** sin anonimizar.  
- Si los datos contienen información sensible, enmascara antes de commitear y documenta el método de anonimización.

---

## Roles y contacto
- **Responsable de pilotos** — coordina diseño, ejecución y cierre.  
- **Analista de datos** — procesa `execution/data/raw/` y genera `analysis/`.  
- **Panel de validación** — aprueba pilotos que impactan procesos críticos (ver `Governance/panel-validacion.md`).  
- **Soporte técnico** — mantiene hooks, CI y despliegue a GitHub Pages.

---
