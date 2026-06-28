```markdown
date: 2026-06-28
author: Adrian — Responsable de Integración
version: v1.1
status: borrador
area: integration
summary: Índice operativo para Integration; estructura por subcarpetas, frontmatter obligatorio, convenciones de nombres y buenas prácticas simplificadas para integraciones reproducibles y trazables.
linked_issues: []
linked_prs: []
```
# Integration

## Propósito
Centralizar y organizar los **scripts, workflows y conectores** que permiten automatizar procesos, sincronizar datos y mantener trazabilidad de las integraciones.  
La carpeta asegura que cada integración sea **documentada, probada y controlada**.

---

## Estructura recomendada (subcarpetas)
- **`scripts/`** — Código para consumir APIs y transformar datos.  
- **`workflows/`** — Pipelines y automatizaciones (ej.: GitHub Actions).  
- **`connectors/`** — Configuración de integraciones con sistemas externos (POS, CRM, encuestas).  
- **`logs/`** — Registros de ejecución y errores.  
- **`tests/`** — Scripts y resultados de pruebas.  
- **`docs/`** — Documentación técnica y guías rápidas.  
- **`changelog.md`** — Registro de cambios y versiones de integraciones.  
- **`assets/`** — Recursos multimedia asociados.

---

## Convención de nombres
**Formato recomendado**  
```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-07-01_script_pos_sync_v1.py
Ejemplo: 2026-07-02_workflow_dashboard_update_v1.yml
Ejemplo: 2026-07-03_connector_crm_auth_v1.json
Ejemplo: 2026-07-04_log_integration_pipeline_v1.log
Ejemplo: 2026-07-05_test_pos_export_v1.py
Ejemplo: 2026-07-06_doc_integration_setup_v1.md
```
**Campos clave**: fecha; tipo (script/workflow/connector/log/test/doc); área; tema; versión `vN`.

---

## Frontmatter obligatorio (mínimo)
Todos los `.md` en `Integration/` y subcarpetas deben incluir frontmatter YAML.

```yaml
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: borrador / activo / archivado
area: integration / pos / crm / api / general
summary: Breve descripción de la integración
linked_issues: []
linked_prs: []
```

Campos opcionales recomendados: `workflow_id`, `trigger`, `responsible`, `source_files`.

---

## Plantillas mínimas por subcarpeta
- **scripts/**: `script_id`, `language`, `dependencies`, `purpose`.  
- **workflows/**: `workflow_id`, `trigger`, `steps`, `expected_output`.  
- **connectors/**: `system`, `auth_method`, `endpoints`, `status`.  
- **logs/**: `run_id`, `date`, `status`, `errors`.  
- **tests/**: `test_id`, `scope`, `expected_result`, `actual_result`.  
- **docs/**: `title`, `audience`, `summary`, `steps`.

---

## Flujo operativo recomendado (resumido)
1. **Diseñar** el script o workflow en su carpeta correspondiente.  
2. **Probar** en `tests/` y documentar resultados.  
3. **Registrar** ejecución en `logs/`.  
4. **Documentar** en `docs/` cómo usarlo.  
5. **Aprobar** cambios vía issue/PR y registrar en `changelog.md`.  
6. **Publicar** integración como activa.

---

## Buenas prácticas operativas (fáciles de entender)
1. **Identifica**: define claramente qué integra y por qué.  
2. **Registra**: guarda logs de cada ejecución.  
3. **Documenta**: explica pasos y dependencias en `docs/`.  
4. **Prueba**: valida en `tests/` antes de producción.  
5. **Versiona**: usa `vN` en nombres y actualiza `changelog.md`.  
6. **Asegura trazabilidad**: enlaza issues y PRs en el frontmatter.

---

## Ejemplos de nombres de archivo por subcarpeta
- `scripts/2026-07-01_script_pos_sync_v1.py`  
- `workflows/2026-07-02_workflow_dashboard_update_v1.yml`  
- `connectors/2026-07-03_connector_crm_auth_v1.json`  
- `logs/2026-07-04_log_integration_pipeline_v1.log`  
- `tests/2026-07-05_test_pos_export_v1.py`  
- `docs/2026-07-06_doc_integration_setup_v1.md`

---

## Roles y contacto
- **Responsable de Integración** — coordina scripts y workflows.  
- **Desarrollador** — crea y mantiene código en `scripts/`.  
- **Analista de datos** — valida integraciones y revisa `logs/`.  
- **Panel de validación** — aprueba workflows críticos.  
- **Soporte técnico** — asegura despliegue y mantenimiento de CI/CD.
