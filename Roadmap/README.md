# Roadmap — Cronogramas diagramas de Gantt y hitos estratégicos
---
### Propósito metodológico
- **Servir como sistema de navegación temporal** del proyecto, mostrando fases, entregables, responsables y tiempos.  
- **Asegurar trazabilidad visual y documental** para que cliente y equipo anticipen ajustes y validen avances.  
- **Consolidar cronogramas, hitos y mapas de ruta** en versiones actualizadas y defendibles.

---

### Contenido principal recomendado
- **Gantt**: diagramas por fase con dependencias, duración y responsables.  
- **Hitos**: listado de entregables críticos con fecha, responsable y criterio de aceptación.  
- **Cronogramas**: planes detallados por semana/mes para coordinación operativa.  
- **Visuals**: mapas de ruta gráficos para presentaciones ejecutivas.  
- **Exports**: versiones PDF/PPT listas para entrega externa.  
- **Changelog**: registro de cambios en cronogramas y hitos.

---

### Estructura y convención de nombres
**Estructura sugerida**
- `/gantt`  
- `/hitos`  
- `/cronogramas`  
- `/visuals`  
- `/exports`  
- `/changelog`

**Convención de archivos**
```text
YYYY-MM-DD_tipo_fase_tema_vN.ext
Ejemplo: 2026-07-01_gantt_planeacion_roadmap-v1.mpp
```
- **Fecha**: `YYYY-MM-DD` para ordenar cronológicamente.  
- **Tipo**: gantt / hito / cronograma / visual / export / changelog.  
- **Fase**: inicio / diagnostico / planeacion / implementacion / cierre.  
- **Versión**: `v1`, `v2` para control de cambios.  
- **Formato**: editable (MS Project, Excel, Google Sheets) y export (PDF, PNG, PPTX).

**Metadatos mínimos en cada archivo**
- **Fecha**  
- **Autor**  
- **Responsable**  
- **Estado**: borrador / en revisión / aprobado  
- **Resumen**: 1 línea con objetivo del cronograma o hito

---

### Plantillas formatos y ejemplos rápidos
**Plantilla hito breve**
```markdown
Hito ID: HTO-YYYYMMDD-XX
Fecha objetivo: YYYY-MM-DD
Título: Entrega de diagnóstico
Responsable: Nombre
Criterio de aceptación: lista corta
Estado: abierto / cumplido
Evidencia: ruta o enlace
```

**Formato cronograma semanal (Excel/Sheet)**
- Columnas: Semana inicio | Actividad | Responsable | Duración días | Dependencias | Estado | Comentarios

**Recomendación visual**
- Mantener una versión operativa (actualización semanal) y una ejecutiva (resumen mensual).  
- Incluir leyenda de dependencias y una línea de tiempo visible para hitos críticos.

---

### Flujo recomendado buenas prácticas y checklist
**Flujo de trabajo**
1. Crear cronograma maestro en `/gantt` con dependencias y responsables.  
2. Desglosar en cronogramas operativos por semana en `/cronogramas`.  
3. Registrar hitos en `/hitos` y vincularlos a tareas del Gantt.  
4. Actualizar estado semanalmente y exportar snapshot a `/exports`.  
5. Registrar cualquier ajuste en `/changelog`.

**Checklist antes de publicar o actualizar**
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos (fecha, autor, responsable, estado).  
- [ ] Dependencias y responsables definidos para cada tarea.  
- [ ] Hitos con criterio de aceptación y responsable asignado.  
- [ ] Snapshot exportado a `/exports` si corresponde.  
- [ ] Entrada en `/changelog` con motivo y responsable del cambio.

**Buenas prácticas**
- Versionar cambios y conservar snapshots mensuales para auditoría.  
- Señalar riesgos de calendario en la descripción del cronograma y notificar a Governance si afectan entregables críticos.  
- Usar colores consistentes para fases y estados según el Manual de Estándares visuales.  
- Mantener una vista simplificada para presentaciones ejecutivas y una vista detallada para operación.

---

### Historial contacto y responsables
- **Changelog**: mantener `changelog.md` con fecha, cambio, motivo y responsable.  
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador de Roadmap).  
- **Correo interno**: `roadmap@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: contacto en `Governance/` para ajustes de alcance o plazos.
