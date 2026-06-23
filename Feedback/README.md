# 📂 Feedback

## 🎯 Propósito metodológico
- **Centralizar la retroalimentación sistemática** de clientes, consultores y personal operativo.  
- **Convertir comentarios en insumos de mejora continua**, asegurando que cada observación tenga respuesta o acción definida.  
- **Cerrar el ciclo de comunicación**: registrar, priorizar y dar seguimiento a las acciones derivadas del feedback.

---

## 📑 Contenido principal recomendado
- **/cliente** → opiniones del sponsor y equipo directivo; evaluaciones sobre entregables y estrategia.  
- **/consultores** → observaciones del equipo consultor sobre metodología, plantillas y aprendizajes técnicos.  
- **/operativos** → retroalimentación del personal de cocina, barra y servicio sobre aplicabilidad práctica.  
- **/sintesis** → informes consolidados por fase con resumen de comentarios, acciones implementadas y lecciones aprendidas.  
- **changelog.md** → registro de cambios y ajustes derivados del feedback.  
- **/templates** → formatos estandarizados para captura de comentarios.

---

## 🗂 Estructura de carpetas sugerida
- `/cliente`  
- `/consultores`  
- `/operativos`  
- `/sintesis`  
- `/templates`  
- `/changelog`

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_origen_fase_tipo_tema_vN.ext
Ejemplo: 2026-06-23_operativos_faseII_sugerencia-proceso-v1.md
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Origen**: cliente / consultores / operativos.  
- **Fase**: Inicio / Diagnóstico / Planeación / Implementación / Cierre.  
- **Tipo**: comentario / sugerencia / queja / reconocimiento.  
- **Versión**: `v1`, `v2`, ... para control de cambios.

**Metadatos mínimos en cada registro** (primer bloque del archivo)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Origen**: cliente / consultor / operativo  
- **Fase**: fase del proyecto  
- **Resumen**: 1–2 líneas con el punto clave  
- **Acción propuesta**: responsable y plazo sugerido

---

## 🧾 Formato estandarizado para captura
Usar Markdown o CSV con columnas:
`fecha | fase | origen | autor | comentario | tipo | prioridad | acción propuesta | responsable | estado`

**Tipos**: positivo / negativo / sugerencia  
**Prioridad**: alta / media / baja  
**Estado**: abierto / en progreso / cerrado

---

## ✅ Buenas prácticas para colaboradores
- Registrar feedback **inmediatamente** tras la recolección.  
- Vincular cada comentario a un **ID de acción** si requiere seguimiento.  
- Mantener `/sintesis` actualizada con acciones y resultados.  
- Evitar duplicados: antes de crear un nuevo registro, buscar coincidencias por tema.  
- Marcar información sensible y seguir protocolo de confidencialidad.

---

## 🔁 Ciclo de gestión del feedback
1. **Captura** → registrar comentario con metadatos.  
2. **Clasificación** → origen, tipo y prioridad.  
3. **Asignación** → responsable y plazo.  
4. **Ejecución** → acción documentada en `/sintesis`.  
5. **Cierre** → registrar resultado y lección aprendida en `/changelog` y `Lessons-Learned`.

---

## 🧾 Checklist antes de cerrar un registro
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos.  
- [ ] Acción propuesta asignada con responsable y plazo.  
- [ ] Evidencias o notas de seguimiento adjuntas.  
- [ ] Estado actualizado a cerrado si aplica.  
- [ ] Entrada reflejada en `/sintesis` y `/changelog` si generó cambio.

---

## 📝 Historial de cambios ejemplo
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/feedback-readme` | Creación del README en /Feedback | Equipo consultor |
| 2026-06-24 | `add/cliente-feedback-v1` | Subida de encuesta de satisfacción del sponsor | Coordinador de proyecto |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador de Calidad).  
- **Correo interno**: `feedback@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: indicar contacto en Governance para decisiones críticas.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Feedback/`.  
Úsalo como **guía operativa** para capturar, priorizar y cerrar retroalimentación de forma trazable y orientada a resultados.
