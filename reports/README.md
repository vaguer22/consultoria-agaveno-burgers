# 📂 Reports 

## 🎯 Propósito metodológico
- **Ser el sistema de evidencia y comunicación** del proyecto, consolidando los reportes que documentan avances, hallazgos y resultados de pilotos.  
- **Asegurar que cada fase tenga un informe defendible y trazable**, con datos objetivos y conclusiones claras.  
- **Conectar Fase IV Implementación con Fase V Cierre**, mostrando cómo las medidas aplicadas generan impacto real.

---

## 📑 Contenido principal recomendado
- **/inicio** → informe de arranque, acuerdos iniciales y evidencia de condiciones de inicio.  
- **/diagnostico** → informe diagnóstico con hallazgos clave, brechas y oportunidades.  
- **/planeacion** → informe de planeación, roadmap validado y priorización de medidas.  
- **/implementacion** → informes de pilotos, resultados de pruebas controladas, ciclos Kaizen y KPIs comparativos antes y después.  
- **/cierre** → informe final consolidado y presentación ejecutiva con resultados, aprendizajes y recomendaciones.  
- **/logs** → bitácoras de reuniones, actas de decisiones y evidencia de seguimiento.  
- **changelog.md** → registro de cambios en informes, control de versiones y auditoría documental.

---

## 🗂 Estructura de carpetas sugerida
- `/inicio`  
- `/diagnostico`  
- `/planeacion`  
- `/implementacion`  
- `/cierre`  
- `/logs`  
- `/exports` → PDFs y PPTX listos para entrega externa  
- `/changelog`

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_fase_tipo_tema_vN.ext
Ejemplo: 2026-06-30_implementacion_piloto-cocina_resultados_v1.pdf
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Fase**: inicio / diagnostico / planeacion / implementacion / cierre.  
- **Tipo**: informe / resumen / acta / presentacion / evidencia.  
- **Versión**: `v1`, `v2`, ... para control de cambios.  
- **Formato**: PDF para versiones finales; Markdown/Word para borradores y notas; PPTX para presentaciones.

**Metadatos mínimos en cada informe** (primer bloque del archivo o en el encabezado)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Fase**: fase del proyecto  
- **Resumen ejecutivo**: 2–4 líneas con el hallazgo o decisión clave  
- **Estado**: borrador / en revisión / aprobado

---

## 🧾 Plantillas recomendadas
- **Informe estándar**: portada, resumen ejecutivo, metodología, hallazgos, evidencia, KPIs, conclusiones, recomendaciones, anexos.  
- **Resumen ejecutivo**: 1 página con KPIs clave, impacto cuantificado y decisiones requeridas.  
- **Acta de reunión**: asistentes, acuerdos, responsables, plazos.  
- **Reporte de piloto**: objetivo del piloto, diseño, métricas antes/después, lecciones y decisión de escalamiento.

---

## 📊 Requisitos mínimos para un informe de implementación
- **Definir objetivo del informe** y público objetivo.  
- **Incluir KPIs comparativos** antes y después con fuente de datos.  
- **Adjuntar evidencia** (fotos, raw data, cronometrajes) o referenciar su ubicación en `/logs` o `/exports`.  
- **Registrar acciones y responsables** para cualquier recomendación.  
- **Versionar** y actualizar `changelog.md` con motivo del cambio.

---

## ✅ Buenas prácticas para colaboradores
- Mantener **raw data** separado de los informes resumidos.  
- Subir la versión final en `/exports` y conservar borradores en la carpeta de la fase correspondiente.  
- Referenciar siempre el **ID del proyecto** y la **fecha** en el encabezado.  
- Cuando un informe genera una decisión operativa, registrar el acuerdo en `/logs` y actualizar `Change-Log`.  
- Evitar duplicados: antes de crear un nuevo informe, buscar versiones previas por tema y fecha.

---

## 🔁 Flujo recomendado de trabajo para un informe de piloto
1. **Recopilar raw data** y evidencia en `/logs` y `/implementacion`.  
2. **Generar borrador** en Markdown con metadatos completos.  
3. **Revisión interna** por consultores y stakeholders clave.  
4. **Aprobación** por el comité de validación y registro en `/logs`.  
5. **Exportar versión final** a PDF/PPTX en `/exports` y actualizar `changelog.md`.

---

## 🧾 Checklist antes de publicar un informe
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos (fecha, autor, fase, resumen ejecutivo).  
- [ ] KPIs con fuentes y metodología de cálculo documentadas.  
- [ ] Evidencias asociadas adjuntas o referenciadas.  
- [ ] Responsable asignado para seguimiento de recomendaciones.  
- [ ] Versión final exportada a `/exports`.  
- [ ] Entrada en `changelog.md` con motivo y responsable.

---

## 📝 Historial de cambios ejemplo
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/reports-readme` | Creación del README en /Reports | Equipo consultor |
| 2026-07-05 | `add/piloto-cocina-report-v1` | Subida del informe de piloto cocina v1 | Líder de implementación |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador de Reportes).  
- **Correo interno**: `reports@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: indicar contacto en Governance para discrepancias o aprobaciones.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Reports/`.  
Úsalo como **portada ejecutiva** de la carpeta: guía la producción de informes, asegura trazabilidad y facilita la comunicación del impacto durante la fase de implementación y el cierre del proyecto.
