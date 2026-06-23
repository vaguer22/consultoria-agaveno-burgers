### Colaboración

#### Visión general
La **sección de Colaboración** define cómo el equipo comunica hallazgos, propone cambios y valida entregables dentro del repositorio. Su objetivo es garantizar que las contribuciones sean **ordenadas, revisables y trazables**, alineadas con los roles definidos en `Governance/` y registradas automáticamente en `Change-Log/`.

---

#### Canales y propósito
- **Issues** — Reportar hallazgos, bugs, solicitudes de mejora y decisiones pendientes.  
- **Pull Requests (PRs)** — Proponer cambios en archivos; incluir contexto, evidencia y pruebas.  
- **Discussions** — Debates estratégicos, propuestas de alcance y consultas abiertas que no requieren un Issue inmediato.  
- **Comunicaciones fuera de GitHub** — Usar solo para coordinación operativa; siempre registrar la decisión final en Issues/PRs.

---

#### Flujo de trabajo recomendado
1. **Detectar** → Crear un **Issue** con: título claro, descripción, evidencia, prioridad y responsable provisional.  
2. **Proponer** → Abrir una **branch** desde `main` siguiendo la convención (ver abajo) y crear un **PR** que referencia el Issue.  
3. **Revisar** → Asignar revisores según RACI; usar comentarios en PR para discusión técnica y de contenido.  
4. **Aprobar** → Revisión aprobada por los roles requeridos; si afecta `Estándares/` o `Governance/`, requerir aprobación del Panel de Validación.  
5. **Merge** → Merge con squash o merge commit según política; el workflow actualiza `Change-Log/changelog.md` automáticamente.  
6. **Cerrar** → Cerrar Issue y registrar evidencia final en `Reports/` o la carpeta correspondiente.

---

#### Convenciones y plantillas
**Naming branches**
```text
feature/<area>-<breve-descripcion>
fix/<area>-<breve-descripcion>
hotfix/<area>-<breve-descripcion>
ex: feature/implementacion-piloto-cocina
```

**Etiquetas recomendadas (labels)**
- `priority:high` `priority:medium` `priority:low`  
- `type:bug` `type:improvement` `type:task` `type:decision`  
- `area:cocina` `area:servicio` `area:governance` `area:training`

**Plantilla mínima para Issues**
```markdown
## Título
**Descripción**:  
**Evidencia**: (ruta o adjunto)  
**Impacto**: alto/medio/bajo  
**Propuesta**: pasos sugeridos  
**Responsable provisional**: nombre  
**Fecha**:
```

**Plantilla mínima para PR**
```markdown
## Resumen del cambio
**Relacionado con Issue**: #ID  
**Qué cambia**: lista breve  
**Evidencia / Tests**: cómo validar  
**Revisores requeridos**: roles o nombres  
**Checklist**:
- [ ] Metadatos actualizados
- [ ] Tests / validaciones
- [ ] Documentación actualizada
```

---

#### Roles y responsabilidades
- **Autores**: proponen cambios y adjuntan evidencia.  
- **Revisores**: validan contenido técnico y cumplimiento de estándares.  
- **Aprobadores**: roles con autoridad para aprobar cambios en `Estándares/` y `Governance/`.  
- **Coordinador de carpeta**: responsable de mantener orden en cada carpeta (ver `README` de cada carpeta).  
Las responsabilidades concretas y la RACI están definidas en `Governance/raci`.

---

#### Transparencia y Change-Log
- **Regla**: todo PR mergeado debe generar o actualizar una entrada en `Change-Log/changelog.md`.  
- **Automatización**: un workflow de GitHub Actions añade la entrada estándar (fecha | carpeta | decisión | motivo | impacto | responsable) al hacer merge en `main`.  
- **Evidencia**: vincular siempre el commit/PR con el Issue y con los documentos finales en `Reports/`, `Pilots/` o `Estándares/`.

---

#### Buenas prácticas y checklist antes de abrir un PR
- [ ] Existe un Issue que justifica el cambio o la mejora.  
- [ ] El branch sigue la convención de nombres.  
- [ ] Metadatos y encabezados en documentos actualizados (fecha, autor, estado).  
- [ ] Evidencia y raw data referenciados o adjuntos.  
- [ ] Tests o validaciones mínimas incluidas (si aplica).  
- [ ] Revisores asignados según RACI.  
- [ ] Si afecta políticas, aprobación del Panel de Validación solicitada.  
- [ ] `changelog.md` será actualizado automáticamente; verificar entrada generada.

---

#### Escalamiento y contacto
- **Dudas operativas** → abrir Issue con etiqueta `type:question`.  
- **Conflictos de decisión** → escalar a `Governance/panel-validacion`.  
- **Soporte técnico de integraciones** → `Integration/` responsable (ver `Integration/README`).  
- **Contacto general**: usar los correos listados en los READMEs de cada carpeta.

---

#### Nota final
La colaboración efectiva depende de disciplina: **documentar, referenciar evidencia y seguir las aprobaciones**. Este marco asegura que cada cambio sea revisable, defendible y trazable dentro del ciclo de vida del proyecto.
