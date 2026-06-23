# 📂 Formación 
---
🎯 ### Propósito metodológico
- **Ser el repositorio de formación práctica** para el personal operativo y administrativo.  
- **Asegurar adopción sostenible** de las mejoras mediante guías claras, materiales accesibles y evidencia de transferencia.  
- **Conectar Fase IV (Implementación) con Fase V (Cierre)** garantizando que el conocimiento quede instalado en la organización.

---

📑 ### Contenido principal recomendado
- **Guías rápidas (Quick Guides)** 📘  
  - Instrucciones paso a paso para tareas críticas (armado de producto, control de inventario, atención al cliente).  
  - Formato visual, breve y listo para impresión o consulta en pantalla.  
- **Manual de capacitación** 📚  
  - Módulos estructurados con objetivos de aprendizaje, contenidos, ejercicios y evaluaciones.  
- **Material audiovisual** 🎥  
  - Videos cortos de procedimientos estandarizados; infografías y pósters para áreas de trabajo.  
- **Plantillas de entrenamiento** 🧾  
  - Checklists para supervisores; formularios de evaluación y rúbricas de desempeño.  
- **Registro de sesiones** 🗓️  
  - Evidencia de capacitaciones (fecha, participantes, temas, asistencia, feedback).  
- **/sintesis** 📎  
  - Informe consolidado de resultados de capacitación, métricas de adopción y recomendaciones.

---

🗂 ### Estructura sugerida y convención de nombres
**Estructura de carpetas**
- `/quick-guides`  
- `/manuales`  
- `/videos`  
- `/templates`  
- `/registros`  
- `/sintesis`  
- `/exports` (versiones finales: PDF / PPTX)

**Convención de archivos**  
```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-07-10_quickguide_cocina_armado-hamburguesa_v1.pdf
```
- **Tipo**: quickguide / manual / video / template / registro / sintesis  
- **Área**: cocina / barra / servicio / admin / delivery  
- **Versión**: `v1`, `v2`, ... para control de cambios

**Metadatos mínimos en cada recurso** (primer bloque del archivo o en el encabezado)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor / Instructor**: nombre y rol  
- **Duración** (si aplica): minutos  
- **Público objetivo**: rol o turno  
- **Resumen**: 1–2 líneas con el objetivo de aprendizaje

---

🧾 ### Plantillas, requisitos mínimos y formatos recomendados
- **Guía rápida (Markdown / PDF)**: objetivo; pasos numerados; tiempo estimado; foto/diagrama; checklist de verificación.  
- **Módulo de capacitación (Manual)**: objetivos, contenidos, ejercicios prácticos, evaluación y criterios de aprobación.  
- **Video**: 1–3 minutos por procedimiento; incluir subtítulos y lista de materiales; nombrar con la convención.  
- **Registro de sesión**: fecha, lista de asistentes, duración, evaluaciones pre/post, feedback y firma del responsable.  
- **Requisito mínimo para publicar**: material validado por responsable de Training y versión final exportada a `/exports`.

---

✅ ### Buenas prácticas, checklist y contacto
**Buenas prácticas**
- Priorizar formatos visuales y pasos accionables para uso en piso.  
- Mantener `raw` (fuentes de video, archivos editables) separado de versiones finales.  
- Versionar cambios y documentar mejoras en `/sintesis` y `changelog` si aplica.  
- Vincular materiales de Training con `Pilots/`, `Reports/` y `Governance/` para trazabilidad.

---

🧾 **Checklist antes de publicar un recurso**
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos (fecha, autor, público).  
- [ ] Material revisado y aprobado por responsable de Training.  
- [ ] Versión final exportada a `/exports`.  
- [ ] Registro de la sesión (si aplica) subido a `/registros`.  
- [ ] Evidencia de evaluación o feedback incluida.

---

**Contacto y responsables**
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador de Training).  
- **Correo interno**: `training@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: indicar contacto en `Governance/` para decisiones sobre alcance o recursos.

---

**Nota final**  
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Training/`.  
Úsalo como **guía operativa** para diseñar, ejecutar y documentar la transferencia de conocimiento de forma práctica, trazable y orientada a la sostenibilidad de las mejoras.
