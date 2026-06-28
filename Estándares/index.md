```
date: 2026-06-28
author: Adrian — Responsable de Estándares
version: v1.2
status: borrador
area: estandares
summary: Índice operativo de Estándares; estructura, frontmatter obligatorio, plantillas, convenciones de nombres y buenas prácticas simplificadas para mantener consistencia documental.
linked_issues: []
linked_prs: []
```
---

# Estándares

## Propósito
Centralizar plantillas, normas y procedimientos operativos para asegurar **consistencia**, **calidad** y **trazabilidad** en la documentación. Servir como fuente única para crear, validar y versionar SOPs, KPIs, registros de riesgo y lecciones aprendidas.

---

## Estructura recomendada
- **templates/** — Plantillas maestras: `sop-template.md`, `kpi-template.md`, `risk-template.md`, `lesson-template.md`, `entregable-template.md`.  
- **sops/** — SOPs por área; cada SOP con frontmatter y checklist.  
- **kpis/** — Definiciones validadas de KPIs.  
- **risk-register/** — Registro de riesgos y planes de mitigación.  
- **lessons-learned/** — Lecciones documentadas y acciones recomendadas.  
- **changelog.md** — Historial de cambios en estándares y plantillas.  
- **assets/** — Imágenes y recursos asociados a estándares.

---

## Convención de nombres
**Formato recomendado**  
```text
YYYY-MM-DD_tipo_area_tema_vN.md
Ejemplo: 2026-06-27_sop_cocina_armado-hamburguesa_v1.md
```
**Reglas clave**  
- **tipo**: `sop` / `kpi` / `risk` / `lesson` / `entregable` / `template`.  
- **area**: cocina / barra / servicio / reparto / finanzas / general.  
- **vN**: versión incremental.

---

## Frontmatter obligatorio y Frontmatter mínimo
**Regla**: todos los archivos `.md` en Estándares deben incluir frontmatter YAML para facilitar búsqueda, automatización y trazabilidad.

**Frontmatter mínimo**
```yaml
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: borrador / aprobado / final
area: cocina / barra / servicio / reparto / finanzas / general
summary: Breve descripción del documento
```
---

**Frontmatter recomendado**
```yaml
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: borrador / aprobado / final
area: cocina / barra / servicio / reparto / finanzas / general
document_id: SOP-YYYYMMDD-01 / KPI-YYYYMMDD-01 / RSK-YYYYMMDD-01
effective_date: YYYY-MM-DD
next_review: YYYY-MM-DD
owner: Nombre — Rol
linked_issues: ["#123"]
linked_prs: ["#456"]
summary: Resumen ejecutivo
```

---

## Plantillas obligatorias
- **sop-template.md** — Propósito, alcance, pasos, checklist, criterios de calidad, responsable, frontmatter completo.  
- **kpi-template.md** — Nombre, definición, fórmula, unidad, frecuencia, fuente, responsable, meta, frontmatter.  
- **risk-template.md** — Descripción, probabilidad, impacto, mitigación, responsable, evidencia.  
- **lesson-template.md** — Contexto, hallazgo, impacto, recomendación, responsable.  
- **entregable-template.md** — Formato estándar para reportes y entregables.

---

## Buenas prácticas operativas simplificadas
1. **Incluye frontmatter**: todo documento debe tener el frontmatter mínimo antes de editar.  
2. **Usa plantillas**: siempre parte de `templates/` para crear SOPs, KPIs o registros.  
3. **No sobrescribir versiones**: cuando cambies algo, crea `vN+1` y explica el cambio en `changelog.md`.  
4. **Registra aprobaciones**: vincula `linked_issues` o `linked_prs` y anota la decisión en el documento.  
5. **Adjunta evidencia**: fotos, actas o datos relevantes en `assets/` y referencia en el frontmatter.  
6. **Revisión periódica**: respeta `next_review` y actualiza el documento según el ciclo definido.  
7. **Claridad y accesibilidad**: escribe pasos concretos y usa listas y checklists para que cualquiera pueda ejecutar el SOP.

---

## Control de cambios y trazabilidad
- **Changelog**: cada cambio debe registrarse en `changelog.md` con fecha, autor, motivo y `document_id`.  
- **Linked records**: usar `linked_issues` y `linked_prs` para conectar discusiones y aprobaciones.  
- **Versionado de archivos**: mantener `vN` en nombres de archivo y actualizar `version` en frontmatter.

---

## Privacidad y evidencia
- **No subir PII** sin anonimizar.  
- **Evidencia**: almacenar en `assets/` y referenciar en frontmatter con `evidence_files`.  
- **Acceso**: controlar permisos del repositorio según sensibilidad del contenido.

---

## Roles y contacto
- **Owner de Estándares** — mantiene plantillas y coordina actualizaciones.  
- **Responsable de área** — autoriza cambios en SOPs de su área.  
- **Panel de validación** — aprueba estándares críticos (ver `Governance/panel-validacion.md`).  
- **Soporte técnico** — gestiona pipelines y despliegue a GitHub Pages.

---

## Cómo solicitar cambios
1. Abrir un **issue** con etiqueta `estandares`.  
2. Adjuntar propuesta en PR usando la plantilla correspondiente desde `templates/`.  
3. Referenciar `document_id` en frontmatter y en el issue.  
4. Esperar revisión y aprobación del owner o panel de validación.

---
