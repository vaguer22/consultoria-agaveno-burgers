```
date: 2026-06-28
author: Adrian — Responsable de Governance
version: v1.2
status: borrador
area: governance
summary: Versión simplificada del índice de Governance: estructura, frontmatter mínimo, pasos claros y contactos.
linked_issues: []
linked_prs: []
```
# Governance

## Propósito
Definir de forma clara y práctica **quién decide**, **cómo se aprueba** y **qué metadatos** debe tener cada documento del repositorio.

---

## Estructura (lo esencial)
- **policies/** — Políticas y normas.  
- **roles-responsabilidades.md** — Quién hace qué.  
- **panel-validacion.md** — Quién aprueba y cómo.  
- **workflows/** — Pasos para procesos clave (ej.: aprobar un SOP).  
- **templates/** — Plantillas listas para usar.  
- **changelog.md** — Registro simple de cambios.  
- **evidence/** — Actas y documentos de respaldo.

---

## Frontmatter mínimo (usar siempre) yaml

```
date: YYYY-MM-DD
author: Nombre — Rol
version: v1.0
status: borrador / vigente / archivado
area: governance
summary: Una frase que explique el documento
```

**Consejo:** para políticas críticas añade `policy_id`, `owner` y `next_review`.

---

## Pasos rápidos para publicar o cambiar una política
1. **Crear**: duplicar la plantilla desde `templates/` y completar el frontmatter.  
2. **Proponer**: abrir un *issue* describiendo el cambio.  
3. **Enviar PR**: crear una PR con la nueva versión (`vN+1`) y enlazar el *issue*.  
4. **Revisar**: asignar reviewers del panel de validación.  
5. **Aprobar**: registrar la aprobación en `approval-template.md` y actualizar `changelog.md`.  
6. **Publicar**: marcar `status: vigente`.

---

## Buenas prácticas (fáciles de seguir)
- **Siempre** incluye el frontmatter mínimo antes de editar.  
- **No sobrescribas** versiones: crea `vN+1` y explica el cambio.  
- **Registra aprobaciones** en el documento y en `changelog.md`.  
- **Adjunta evidencia** en `evidence/` cuando aplique.  
- **Respeta fechas** de revisión (`next_review`) para mantener políticas actualizadas.  
- **Escribe claro**: usa listas y checklists; evita párrafos largos.

---

## Roles y contacto (rápido)
- **Owner de Governance** — mantiene el índice y coordina aprobaciones.  
- **Panel de validación** — revisa y aprueba políticas críticas.  
- **Responsables de área** — validan documentos de su dominio.  
- **Soporte técnico** — gestiona despliegue y accesos.

**Cómo escalar:** abrir un *issue* con etiqueta `governance` y referenciar `policy_id` en el frontmatter.
