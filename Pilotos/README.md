# 📂 Pilots

## 🎯 Propósito metodológico
- **Servir como laboratorio de experimentación** donde se diseñan, ejecutan y documentan pruebas piloto y eventos Kaizen.  
- **Validar hipótesis de mejora** en entornos controlados antes de escalar a la operación completa.  
- **Proveer evidencia práctica y medible** que conecte la implementación (Fase IV) con el cierre y lecciones (Fase V).

---

## 📑 Contenido principal recomendado
- **/charters** → documentos de inicio de cada piloto o Kaizen: hipótesis, objetivos SMART, alcance y criterios de éxito.  
- **/ejecucion** → registros diarios de implementación: cronometrajes, fotos, observaciones y checklists.  
- **/resultados** → KPIs comparativos antes/después, análisis de impacto y evaluación de criterios de aceptación.  
- **/retroalimentacion** → comentarios del personal operativo y validación de aplicabilidad práctica.  
- **/sintesis** → informe consolidado del piloto con recomendaciones para escalar, ajustar o descartar la medida.  
- **changelog.md** → registro de iteraciones, cambios en el diseño del piloto y decisiones tomadas.  
- **/exports** → versiones finales en PDF/PPT listas para entrega.

---

## 🗂 Estructura de carpetas sugerida
- `/charters`  
- `/ejecucion`  
- `/resultados`  
- `/retroalimentacion`  
- `/sintesis`  
- `/exports`  
- `/changelog`

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_piloto_area_tema_vN.ext
Ejemplo: 2026-07-01_piloto_cocina_reorden-flujo_v1.md
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: piloto / kaizen / reporte / evidencia.  
- **Área**: cocina / barra / servicio / delivery / admin.  
- **Versión**: `v1`, `v2`, ... para control de cambios.  
- **Formato**: Markdown para documentación viva; PDF/PPT para entregables finales.

**Metadatos mínimos en cada documento** (primer bloque del archivo)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **ID piloto**: identificador único (ej. PIL-001)  
- **Objetivo**: 1 línea con el objetivo SMART  
- **Criterio de éxito**: métricas y umbrales

---

## 🧾 Plantillas recomendadas (usar Markdown)
- **Charter de piloto**: objetivo SMART; hipótesis; alcance; duración; recursos; criterios de éxito; responsables.  
- **Registro de ejecución**: fecha, hora, actividad, observador, evidencia (foto/archivo), notas.  
- **Reporte de resultados**: KPIs antes/después, análisis estadístico simple, conclusiones y decisión (escalar/ajustar/descartar).  
- **Ficha de retroalimentación**: origen (operativo/cliente/consultor), comentario, prioridad, acción propuesta, responsable, estado.

---

## 🔬 Requisitos mínimos para ejecutar un piloto
- **Charter aprobado** con objetivos y criterios de éxito claros.  
- **Raw data** (cronometrajes, POS, encuestas) accesible y referenciado.  
- **Responsables asignados** para ejecución, monitoreo y análisis.  
- **Periodo de prueba definido** y control de variables (turnos, días, menú).  
- **Plan de comunicación** para informar a operativos y stakeholders.

---

## 🔁 Flujo recomendado (corto y práctico)
1. **Diseñar** → crear charter y aprobar en panel de validación.  
2. **Preparar** → entrenar al personal, preparar materiales y definir recolección de datos.  
3. **Ejecutar** → aplicar la prueba según protocolo y registrar evidencia diaria.  
4. **Analizar** → comparar KPIs antes/después; validar criterios de éxito.  
5. **Decidir** → escalar, ajustar o descartar; documentar en `/sintesis` y actualizar `changelog.md`.  
6. **Transferir** → si se escala, generar plan de rollout y actualizar `Governance/` y `Training/`.

---

## ✅ Buenas prácticas para colaboradores
- Mantener **raw data** separado de resúmenes y reportes.  
- Subir evidencia (fotos, cronometrajes) a `/ejecucion` inmediatamente después de la recolección.  
- Versionar documentos y actualizar `changelog.md` en cada iteración.  
- Vincular cada piloto con su **ID** en `Reports/` y `Metrics/` para trazabilidad.  
- Documentar lecciones aprendidas en `Lessons-Learned/` tras el cierre del piloto.

---

## 🧾 Checklist antes de cerrar un piloto
- [ ] Charter aprobado y firmado (o acta de validación).  
- [ ] Raw data completo y validado.  
- [ ] KPIs comparativos calculados y documentados.  
- [ ] Retroalimentación del personal registrada.  
- [ ] Decisión documentada: escalar / ajustar / descartar.  
- [ ] Informe consolidado en `/sintesis` y versión final en `/exports`.  
- [ ] Entrada en `changelog.md` con motivo y responsable.

---

## 📝 Historial de cambios (ejemplo)
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-07-01 | `init/pilots-readme` | Creación del README en /Pilots | Equipo consultor |
| 2026-07-10 | `add/charter-piloto-001` | Subida del charter PIL-001 | Líder de implementación |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Líder de Pilotos).  
- **Correo interno**: `pilotos@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: indicar contacto en Governance para decisiones críticas.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Pilots/`.  
Úsalo como **guía operativa** para diseñar, ejecutar y documentar pilotos de forma rigurosa, trazable y orientada a resultados.
