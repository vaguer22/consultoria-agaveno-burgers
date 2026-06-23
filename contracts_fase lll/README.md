# 📂 Contracts — Acuerdos formales que validan la planeación

## 🎯 Propósito metodológico
- **Consolidar los compromisos formales** que surgen tras el diagnóstico y la planeación estratégica.  
- **Garantizar respaldo legal y ético** de propuestas y planes de acción, evitando ambigüedades.  
- **Servir como puente de validación** entre la planeación conceptual y la implementación práctica.

---

## 📑 Contenido principal recomendado
- **Propuesta Técnica validada**: documento que integra metodología, fases, cronograma y entregables ajustados tras el diagnóstico.  
- **Contratos de prestación de servicios**: cláusulas legales y financieras que formalizan la ejecución del plan.  
- **Actas de validación de planeación**: evidencia de aceptación de planes estratégicos y tácticos.  
- **Carta de compromiso ampliada**: versión extendida de la carta acuerdo inicial, alineada con objetivos y recursos asignados.  
- **Changelog de acuerdos** (opcional): registro de modificaciones en contratos y propuestas técnicas para trazabilidad.

---

## 🗂 Estructura de carpetas sugerida
- `/propuesta-tecnica` → propuesta validada y versiones revisadas.  
- `/contratos` → contratos firmados, anexos y comprobantes de firma.  
- `/actas` → actas de reuniones con acuerdos y firmas.  
- `/carta-compromiso` → carta inicial y versión ampliada.  
- `/changelog` → historial de cambios y motivos.  
- `/templates` → plantillas estándar (propuesta, acta, cláusulas comunes).

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_tipo_documento_area_tema_vN.ext
Ejemplo: 2026-06-30_propuesta-tecnica_planeacion_kpis_v1.pdf
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: propuesta / contrato / acta / carta / anexo / changelog.  
- **Área o tema**: planeación / implementación / legal / financiero.  
- **Versión**: `v1`, `v2`, ... para control de cambios.  
- **Formato**: PDF para documentos firmados; Markdown/Word para borradores y plantillas.

**Metadatos mínimos en cada documento**  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Estado**: borrador / en revisión / firmado  
- **Partes**: consultor / cliente  
- **Resumen**: 1 línea con el propósito del documento

---

## ✅ Buenas prácticas legales y operativas
- Guardar **una copia firmada en PDF** para cada documento legal en `/contratos` o `/carta-compromiso`.  
- Mantener borradores y versiones intermedias en `/changelog` con notas de revisión y motivo del cambio.  
- No incluir información sensible (números de cuenta, datos bancarios) en archivos sin protección; seguir protocolo de confidencialidad.  
- Referenciar siempre el **ID del proyecto** y la **fecha de firma** en actas y anexos.  
- Al actualizar un contrato, conservar la versión anterior en `/changelog` y documentar el motivo y la aprobación.

---

## 🧾 Checklist antes de cerrar un documento contractual
- [ ] Nombre del archivo cumple la convención.  
- [ ] Documento firmado (si aplica) y guardado en PDF.  
- [ ] Metadatos completos (fecha, autor, estado, partes, resumen).  
- [ ] Anexos y evidencias (correos, aprobaciones) adjuntados o referenciados.  
- [ ] Changelog actualizado con motivo y responsable del cambio.  
- [ ] Copia enviada a las partes interesadas y registrada en actas.

---

## 📝 Historial de cambios ejemplo
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/contracts-readme` | Creación del README en /Contracts | Equipo consultor |
| 2026-06-30 | `add/propuesta-tecnica-v2` | Subida de propuesta técnica validada | Coordinador de proyecto |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador Legal).  
- **Correo interno**: `contratos@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: contacto en Governance para disputas o aclaraciones contractuales.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Contracts/`.  
Úsalo como **portada ejecutiva**: explica el propósito, guía el manejo de documentos y asegura la trazabilidad legal y operativa de la planeación y su ejecución.
