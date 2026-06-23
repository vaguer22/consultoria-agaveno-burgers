# 📂 Reports_fase V  — Informe final con KPIs consolidados
---
## 🎯 Propósito metodológico
- **Ser el documento de cierre y transferencia** del proyecto, integrando hallazgos, resultados de pilotos y métricas clave.  
- **Consolidar KPIs línea base vs. KPIs finales** para mostrar el impacto cuantificable de las medidas implementadas.  
- **Entregar una presentación ejecutiva defendible** que sirva para validación con el cliente y replicabilidad futura.

---

### 📑 Contenido principal recomendado
- **Informe final** (`report_cierre_<fecha>.md`): resumen ejecutivo, narrativa por fases, evidencia de cumplimiento y conclusiones.  
- **KPIs consolidados**: comparativas antes/después, tablas, dashboards y análisis de tendencias.  
- **Resultados de pilotos**: síntesis de pruebas controladas, impacto por área y validación de hipótesis.  
- **Retroalimentación integrada**: percepciones de operativos y clientes sobre cambios y aceptación cultural.  
- **Recomendaciones estratégicas**: medidas para sostener resultados, plan de escalamiento y próximos pasos.  
- **/exports**: PDF y PPTX listos para entrega externa; material visual (gráficas, dashboards).  
- **changelog.md**: historial de versiones del informe y registro de revisiones.

---

### 🗂 Estructura de carpetas sugerida
- `/final` → borradores y versión de trabajo del informe final.  
- `/kpis` → hojas de cálculo, definiciones y visualizaciones consolidadas.  
- `/pilotos` → resúmenes y evidencias de cada piloto referenciado.  
- `/feedback` → síntesis de retroalimentación integrada.  
- `/exports` → PDF / PPTX / imágenes listas para entrega.  
- `/changelog` → control de versiones y notas de revisión.

---

### 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_report_cierre_tema_vN.ext
Ejemplo: 2026-07-15_report_cierre_el-agaveno_v1.md
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: report_cierre / kpi / piloto / feedback / export.  
- **Versión**: `v1`, `v2`, ... para control de cambios.  
- **Formato**: Markdown para versión viva; PDF/PPTX para entrega final.

**Metadatos mínimos en el informe** (primer bloque o encabezado)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor / Equipo**: nombres y roles  
- **Resumen ejecutivo**: 2–4 líneas con el hallazgo clave  
- **Periodo comparado**: fechas de línea base y periodo final  
- **Estado**: borrador / en revisión / aprobado

---

### 🔎 Contenido mínimo del Informe final
1. **Portada**: título, cliente, equipo, fecha y versión.  
2. **Resumen ejecutivo**: impacto cuantificado, KPIs clave y decisión recomendada.  
3. **Metodología**: fuentes de datos, alcance y limitaciones.  
4. **Narrativa por fases**: síntesis de Inicio, Diagnóstico, Planeación, Implementación y Cierre.  
5. **KPIs consolidados**: tablas comparativas, gráficos y análisis de variaciones.  
6. **Resultados de pilotos**: objetivos, diseño, métricas antes/después y decisión.  
7. **Retroalimentación**: síntesis de percepciones y evidencia de aceptación.  
8. **Recomendaciones**: acciones para sostenibilidad, responsables y plazos.  
9. **Anexos**: raw data, cronometrajes, actas y evidencias multimedia.

---

### ✅ Buenas prácticas y checklist antes de publicar
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos (fecha, autor, estado, periodo comparado).  
- [ ] KPIs con definiciones, fórmulas y fuentes documentadas.  
- [ ] Raw data y evidencias referenciadas o adjuntas en `/exports`.  
- [ ] Resumen ejecutivo claro y cuantificado (impacto en números).  
- [ ] Recomendaciones con responsables y plazos definidos.  
- [ ] Versión final exportada a PDF/PPTX en `/exports`.  
- [ ] `changelog.md` actualizado con motivo y responsable de la versión.

---

### 📊 Recomendaciones para visualizaciones
- Incluir **comparativa antes/después** con periodo de referencia visible.  
- Mostrar **tendencia temporal** (30/90/180 días) cuando aplique.  
- Añadir **nota metodológica** en cada gráfico: fuente, frecuencia y filtros aplicados.  
- Guardar snapshots mensuales en `/exports/dashboards` para auditoría.

---

### 🧾 Historial de cambios (ejemplo)
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-07-15 | `init/report-cierre-v1` | Creación del borrador del informe final | Equipo consultor |
| 2026-07-20 | `update/report-cierre-v2` | Incorporación de KPIs consolidados y feedback | Analista de métricas |

---

### 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador de Cierre).  
- **Correo interno**: `reports@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: contacto en `Governance/` para validaciones finales.

---

### 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Reports/`.  
Úsalo como **plantilla de cierre**: guía la consolidación de evidencia, facilita la entrega ejecutiva y asegura que el impacto del proyecto quede documentado, defendible y transferible.
