```
date: 2026-06-28
author: Adrian — Responsable de Integración
version: v1.0
status: borrador
area: integration
summary: Índice operativo de Integration; estructura de carpetas, frontmatter mínimo y buenas prácticas simplificadas para automatización y trazabilidad.
linked_issues: []
linked_prs: []
```
# Integration

## Propósito
Documentar y organizar los **scripts, workflows y conectores** que permiten sincronizar datos, reducir tareas manuales y asegurar trazabilidad en tiempo real.  
La carpeta funciona como el **motor invisible del repositorio**, conectando planeación con implementación.

---

## Estructura
- **scripts/** — Código en Python/Node.js para consumir APIs y transformar datos.  
- **workflows/** — Archivos YAML de GitHub Actions y pipelines CI/CD.  
- **connectors/** — Configuración de integraciones con sistemas externos (POS, CRM, encuestas).  
- **logs/** — Registro de ejecuciones, errores y resultados.  
- **tests/** — Scripts de prueba para validar integraciones antes de producción.  
- **docs/** — Documentación técnica y guías rápidas.  
- **changelog.md** — Registro de cambios en scripts y workflows.

---

## Frontmatter mínimo (usar siempre)
```
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: borrador / activo / archivado
area: integration
summary: Breve descripción del script o workflow
```

**Consejo:** para workflows críticos añadir `workflow_id`, `trigger` y `linked_issues`.

---

## Convenciones de nombres
```
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-06-28_script_notion_sync_v1.py
Ejemplo: 2026-06-28_workflow_dashboard_update_v1.yml
```
- **tipo**: script / workflow / connector / log / test / doc.  
- **area**: notion / pos / encuesta / dashboard / general.  
- **vN**: versión incremental.

---

## Buenas prácticas (fáciles de seguir)
1. **Incluye frontmatter**: cada archivo debe tener metadatos básicos.  
2. **Usa nombres claros**: fecha, tipo, área y versión.  
3. **No sobrescribas**: crea nueva versión (`vN+1`) y registra en `changelog.md`.  
4. **Prueba antes de producción**: guarda casos en `tests/` y documenta resultados.  
5. **Registra logs**: cada ejecución debe generar un archivo en `logs/`.  
6. **Documenta**: explica en `docs/` cómo usar scripts y workflows.  
7. **Mantén trazabilidad**: enlaza `linked_issues` y `linked_prs` en el frontmatter.

---

## Roles y contacto
- **Responsable de Integración** — coordina scripts y workflows.  
- **Desarrollador** — crea y mantiene código en `scripts/`.  
- **Analista de datos** — valida integraciones y revisa `logs/`.  
- **Panel de validación** — aprueba workflows críticos.  
- **Soporte técnico** — asegura despliegue y mantenimiento de CI/CD.

**Cómo pedir un cambio:** abrir un *issue* con etiqueta `integration`, adjuntar propuesta y referenciar `workflow_id` o script afectado.
