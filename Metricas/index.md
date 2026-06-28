```
date: 2026-06-28
author: Adrian — Responsable de Métricas
version: v1.2
status: borrador
area: métricas
summary: Versión simplificada del índice de Metrics: estructura, frontmatter mínimo, convenciones y buenas prácticas fáciles de seguir.
linked_issues: []
linked_prs: []
```
# Metrics

## Propósito
Definir dónde y cómo se guardan las métricas, quién las mantiene y cómo se garantiza que sean **consistentes**, **reproducibles** y **auditables**.

---

## Estructura (lo esencial)
- **raw/** — Datos originales sin tocar (CSV, Excel, exportes POS).  
- **processed/** — Datos transformados y tablas limpias; definiciones de KPI en `.md`.  
- **dashboards/** — Visualizaciones y snapshots (PNG, PDF, HTML).  
- **templates/** — Plantillas para definiciones de KPI y reportes.  
- **changelog.md** — Registro simple de cambios en definiciones y fuentes.  
- **assets/** — Imágenes y recursos asociados a dashboards.

---

## Frontmatter mínimo (usar siempre)

```yaml
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: borrador / validado / final
area: métricas
kpi_id: KPI-YYYYMMDD-01
summary: Una frase que explique el KPI o dataset
source_files: ["raw/archivo.csv"]
frequency: diaria / semanal / mensual
responsible: Nombre — Rol
```

**Consejo:** añadir `target`, `formula` y `last_value` cuando corresponda.

---

## Convenciones de nombres
```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-06-01_raw_cocina_cronometraje_v1.csv
Ejemplo: 2026-06_kpi_cocina_tiempo-servicio_v1.md
```
- **tipo**: `raw` / `processed` / `kpi` / `dashboard` / `protocol`.  
- **area**: cocina / barra / servicio / delivery / finanzas.  
- **vN**: versión incremental.

---

## Buenas prácticas (fáciles de entender)
1. **Guarda el original**: sube siempre los archivos sin modificar a `raw/`.  
2. **Documenta transformaciones**: cada archivo en `processed/` debe tener un README o script que explique cómo se obtuvo.  
3. **Define el KPI claramente**: nombre, fórmula, unidad, frecuencia, fuente y responsable.  
4. **Versiona cambios**: cuando cambies una definición o cálculo, crea `vN+1` y anota el motivo en `changelog.md`.  
5. **Snapshots**: guarda una imagen o export (PNG/PDF/CSV) del dashboard clave en `dashboards/exports/` con fecha y autor.  
6. **No subir datos sensibles**: anonimiza o enmascara PII antes de commitear.  
7. **Revisa antes de publicar**: alguien distinto al autor valida la definición y los cálculos.

---

## Plantilla rápida para un archivo KPI (cuerpo mínimo)
- **Nombre del KPI**  
- **Definición** (qué mide y por qué importa)  
- **Fórmula** (texto o LaTeX)  
- **Unidad** (minutos / % / MXN)  
- **Frecuencia** (diaria / semanal / mensual)  
- **Fuente de datos** (archivo en `raw/`)  
- **Responsable**  
- **Meta**  
- **Último valor** (valor y fecha)  
- **Notas** (filtros, supuestos, transformaciones)

---

## Flujo simple de trabajo
1. **Ingesta**: subir datos a `raw/`.  
2. **Procesamiento**: crear `processed/` con scripts reproducibles.  
3. **Validación**: revisar resultados y actualizar `kpi` `.md`.  
4. **Publicación**: exportar snapshot a `dashboards/exports/` y registrar en `changelog.md`.

---

## Roles y contacto (rápido)
- **Responsable de métricas** — mantiene la carpeta y aprueba definiciones.  
- **Analista de datos** — procesa `raw/` → `processed/` y genera dashboards.  
- **Reviewer** — valida definiciones y cálculos antes de publicar.  
- **Soporte técnico** — ayuda con pipelines y despliegue.

**Cómo pedir un cambio:** abrir un *issue* con etiqueta `metrics`, adjuntar la propuesta y referenciar `kpi_id` si aplica.

---
