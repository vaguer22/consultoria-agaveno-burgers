# 📂 Feedback_fase II
---
La carpeta **Feedback** centraliza la retroalimentación recibida durante la **Fase II Diagnóstico** y las fases posteriores. Su objetivo es convertir percepciones de clientes, personal operativo y consultores en **acciones concretas** que mejoren la implementación y la calidad metodológica del proyecto.

---

### Propósito metodológico
- **Capturar y organizar** percepciones de stakeholders relevantes.  
- **Transformar comentarios** en acciones de mejora continua con trazabilidad.  
- **Validar en campo** la aplicabilidad de hallazgos, SOPs y recomendaciones.  
- **Cerrar el ciclo** entre evidencia técnica y ajustes prácticos.

---

### Estructura recomendada de carpetas
#### cliente
- Documentos con opiniones del sponsor y equipo directivo.  
- Evaluaciones sobre claridad, pertinencia e impacto estratégico.

#### operativos
- Retroalimentación del personal de cocina, barra, servicio y reparto.  
- Observaciones sobre factibilidad y carga operativa de SOPs.

#### consultores
- Notas internas del equipo consultor: metodología, plantillas, aprendizajes.  
- Lecciones de campo y propuestas de ajuste metodológico.

#### sintesis
- Informes consolidados por fase con: resumen de comentarios; acciones implementadas; lecciones aprendidas; recomendaciones para la siguiente fase.

#### assets
- Elementos gráficos o plantillas visuales usadas en resúmenes y presentaciones.

---

### Archivos clave
- **changelog.md**  
  - Registro de cambios derivados del feedback.  
  - Formato sugerido por línea: `YYYY-MM-DD | archivo | autor | tipo de feedback | acción tomada | estado`.

- **plantillas de captura**  
  - Archivos `tmpl_feedback_<origen>_<YYYY-MM-DD>.md` o `.csv` para recolección estandarizada.  
  - Campos mínimos: **fecha | fase | autor | rol | comentario | tipo (positivo/negativo/sugerencia) | prioridad | acción propuesta | responsable | estado**.

---

### Formato estandarizado sugerido para captura en Markdown
**Nombre de archivo ejemplo**: `tmpl_feedback_operativos_2026-06-22.md`  
**Campos obligatorios**  
- **Fecha**:  
- **Fase**:  
- **Autor**:  
- **Rol**:  
- **Área**:  
- **Comentario**:  
- **Tipo**: positivo; negativo; sugerencia  
- **Acción propuesta**:  
- **Prioridad**: alta; media; baja  
- **Responsable**:  
- **Estado**: pendiente; en progreso; resuelto

---

### Proceso recomendado para manejo del feedback
1. **Recepción**  
   - Registrar cada comentario usando la plantilla correspondiente.  
2. **Clasificación**  
   - Etiquetar por fase, área y prioridad.  
3. **Análisis**  
   - Evaluar impacto y factibilidad; asignar responsable y plazo.  
4. **Acción**  
   - Implementar ajuste, actualizar SOP o plantilla según corresponda.  
5. **Verificación**  
   - Validar en campo y registrar evidencia en `sintesis/`.  
6. **Cierre**  
   - Actualizar `changelog.md` y marcar estado como resuelto.

---

### Convenciones de nomenclatura
- **Formato general**: `feedback_<origen>_<area>_<YYYY-MM-DD>.md`  
  - **Ejemplo**: `feedback_cliente_directivo_2026-06-22.md`  
- **Prefijos sugeridos**: `feedback_` (entrada de retroalimentación), `tmpl_` (plantilla), `synth_` (síntesis por fase).  
- **Reglas**: usar minúsculas; guiones bajos para separar; fecha ISO `YYYY-MM-DD` al final.

---

### Changelog de feedback
- **Archivo**: `changelog_feedback.md`  
- **Formato de entrada**: `YYYY-MM-DD | fuente | archivo afectado | autor | acción tomada | resultado`  
- **Ejemplo**: `2026-06-22 | operativos | std_sop_cocina_2026-06-22.md | Juan López | Ajuste en paso 3 para reducir tiempo | pendiente verificación`

---

### Buenas prácticas para contribuciones
- **Registrar siempre** cada comentario en la plantilla antes de subir archivos.  
- **Commits**: mensajes claros que incluyan `feedback/` y referencia al archivo afectado.  
- **Revisión**: toda acción derivada del feedback debe pasar por PR con al menos una revisión técnica y una revisión operacional.  
- **Metadatos**: incluir en la cabecera del archivo `Autor`, `Fecha`, `Versión`, `Área`, `Estado`.  
- **Trazabilidad**: vincular cada entrada de feedback con la evidencia en `Documentos/` o `Evidencia/` cuando aplique.

---

### Checklist mínimo para cada entrada de feedback
- [ ] Fecha y autor registrados  
- [ ] Fase y área especificadas  
- [ ] Tipo de comentario definido  
- [ ] Acción propuesta documentada  
- [ ] Responsable asignado  
- [ ] Estado inicial marcado  
- [ ] Entrada en `changelog_feedback.md` vinculada

---

### Narrativa conceptual
La carpeta **Feedback** es el espacio de escucha activa del repositorio: documenta cómo las percepciones de clientes y personal operativo se convierten en ajustes metodológicos y mejoras prácticas. Su función es garantizar que la consultoría sea **colaborativa, defendible y sostenible**, reforzando la cultura de mejora continua en cada fase del proyecto.
