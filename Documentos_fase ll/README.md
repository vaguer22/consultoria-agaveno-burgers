# 📂 Documentos_fase II — Evidencias técnicas y administrativas

## 🎯 Propósito metodológico
- **Servir como repositorio central de evidencias** que sustentan el diagnóstico y las decisiones estratégicas.  
- **Garantizar rigor, trazabilidad y consistencia metodológica** en la captura y análisis de datos.  
- **Conectar Fase II (Diagnóstico) con Fase III (Planeación)** aportando insumos objetivos para diseñar y priorizar intervenciones.

---

## 📑 Contenido principal recomendado
- **Informes de entrevistas**: transcripciones, resúmenes ejecutivos y fichas por entrevistado.  
- **Cronometrajes y observaciones directas**: registros de tiempos (pedido → entrega), raw data y análisis.  
- **Matrices de análisis**: MEO (Medición de Eficiencia Operativa), impacto/esfuerzo, RACI y tablas comparativas.  
- **Base documental de soporte**: manuales internos, reportes administrativos y normativas aplicables.  
- **Hipótesis de diagnóstico**: supuestos vinculados a evidencia cualitativa y cuantitativa.  
- **Bitácoras de campo**: notas de consultores, plantillas estandarizadas y registros de visitas.

---

## 🗂 Estructura de carpetas sugerida
- `/entrevistas` → transcripciones, resúmenes, fichas y consentimientos.  
- `/cronometrajes` → raw data, hojas de cálculo y gráficos de tiempos.  
- `/matrices` → MEO, impacto/esfuerzo, RACI y tablas comparativas.  
- `/bitacoras` → notas diarias, observaciones y plantillas usadas.  
- `/soporte` → manuales, protocolos, reportes financieros y documentos legales.  
- `/exports` → PDFs y versiones finales listas para entrega.

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-06-22_entrevista_cocina_turno-matutino_v1.md
```

**Componentes obligatorios en el nombre**  
- **Fecha**: `YYYY-MM-DD`  
- **Tipo**: entrevista / cronometraje / matriz / bitacora / soporte  
- **Área**: cocina / barra / servicio / admin / finanzas  
- **Tema**: palabra clave breve  
- **Versión**: `v1`, `v2`, ... para control de cambios

**Metadatos mínimos en cada documento** (primer bloque del archivo)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Fuente**: entrevista / observación / documento interno  
- **Lugar**: sucursal / turno / área  
- **Resumen**: 1–2 líneas con el hallazgo clave

---

## 🔬 Plantillas recomendadas (usar Markdown)
- **Ficha de entrevista**: datos, rol, preguntas clave, respuestas destacadas, conclusiones.  
- **Registro de cronometraje**: actividad, tiempo medido, observador, condiciones, notas.  
- **Matriz MEO**: proceso, tiempo estándar, variabilidad, cuellos de botella.  
- **Plantilla de bitácora**: fecha, hora, consultor, actividad, observaciones, acciones sugeridas.

---

## 🔗 Relación con fases del proyecto
- **Fase II Diagnóstico** → principal repositorio de evidencia técnica: entrevistas, cronometrajes y matrices.  
- **Fase III Planeación** → insumos para priorizar iniciativas, diseñar pilotos y definir KPIs.

---

## ✅ Buenas prácticas para colaboradores
- Subir archivos inmediatamente tras la recolección y etiquetar con la convención.  
- Mantener **raw data** (Excel, CSV) y **resúmenes** (Markdown/PDF) separados.  
- Marcar documentos sensibles y seguir el protocolo de confidencialidad.  
- Incluir siempre metadatos al inicio del documento.  
- Usar `/drafts` para versiones en trabajo y `/exports` para versiones finales.

---

## 🧾 Checklist antes de cerrar un informe
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos (fecha, autor, fuente, lugar, resumen).  
- [ ] Raw data asociado subido en `/cronometrajes` o `/soporte`.  
- [ ] Evidencias multimedia (fotos, videos) guardadas en `/soporte` o `/evidencias`.  
- [ ] Versión final exportada a `/exports` con `vN` actualizado.  
- [ ] Referencias cruzadas en `Documentos_fase II` y `Metrics/` si aplica.

---

## 📝 Historial de cambios (ejemplo)
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/doc-faseII-readme` | Creación del README en /Documentos_fase II | Equipo consultor |
| 2026-06-24 | `add/matriz-MEO-v1` | Subida de matriz MEO inicial | Analista operativo |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del analista o rol (ej. Analista de Diagnóstico).  
- **Correo interno**: `diagnostico@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: indicar responsable de gobernanza para decisiones críticas.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Documentos_fase II`.  
Úsalo como **guía operativa y de trazabilidad**: facilita la estandarización de la captura de evidencia y asegura que el diagnóstico se base en datos verificables.
