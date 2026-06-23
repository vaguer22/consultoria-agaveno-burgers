# 📂 Contracts — Acuerdos y Propuestas Técnicas

## 🎯 Propósito metodológico
- **Formalizar los compromisos** entre el equipo consultor y la empresa cliente.  
- **Asegurar transparencia, trazabilidad y defendibilidad** de la intervención.  
- **Servir como base legal y ética** del proyecto, conectando la fase de Inicio con las siguientes etapas.

---

## 📑 Contenido principal recomendado
- **Carta Acuerdo**: objetivos, alcance, entregables, interlocutores y responsabilidades.  
- **Propuesta Técnica**: metodología, fases, cronograma, entregables y requerimientos.  
- **Contratos formales**: cláusulas legales, condiciones de pago, plazos y obligaciones.  
- **Actas de compromiso**: acuerdos firmados en reuniones clave y validaciones formales.  
- **Changelog de acuerdos** (opcional): registro de modificaciones y versiones de documentos.

---

## 🗂 Estructura de carpetas sugerida
- `/carta-acuerdo` → versiones firmadas y borradores autorizados.  
- `/propuesta-tecnica` → propuesta inicial y versiones revisadas.  
- `/contratos` → contratos legales, anexos y comprobantes de firma.  
- `/actas` → actas de reuniones con acuerdos y firmas.  
- `/changelog` → historial de cambios en acuerdos y notas de revisión.  
- `/templates` → plantillas estándar (carta, acta, cláusulas comunes).

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_tipo_documento_version.ext
Ejemplo: 2026-06-22_carta-acuerdo_v1.pdf
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: carta-acuerdo / propuesta / contrato / acta / anexo.  
- **Versión**: `v1`, `v2`, etc., para control de cambios.  
- **Formato**: PDFs para documentos firmados; Markdown/Word para borradores y plantillas.

**Metadatos mínimos en cada documento** (primer bloque o en el nombre del archivo)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Estado**: borrador / en revisión / firmado  
- **Partes**: consultor / cliente  
- **Resumen**: 1 línea con el propósito del documento

---

## ✅ Buenas prácticas legales y operativas
- Mantener **una copia firmada** en `/carta-acuerdo` y `/contratos` (PDF).  
- Guardar borradores y versiones intermedias en `/changelog` con notas de revisión.  
- No incluir información sensible (números de cuenta, datos bancarios) en archivos sin protección; seguir protocolo de confidencialidad.  
- Referenciar siempre el **ID del proyecto** y la **fecha de firma** en actas y anexos.  
- Cuando se actualice un contrato, conservar la versión anterior en `/changelog` y documentar el motivo del cambio.

---

## 📝 Checklist antes de cerrar un documento contractual
- [ ] Nombre del archivo cumple la convención.  
- [ ] Documento firmado (si aplica) y guardado en PDF.  
- [ ] Metadatos completos (fecha, autor, estado, partes, resumen).  
- [ ] Anexos y evidencias (correos, aprobaciones) adjuntados o referenciados.  
- [ ] Changelog actualizado con motivo y responsable del cambio.  
- [ ] Copia enviada a las partes interesadas y registrada en actas.

---

## 🧾 Historial de cambios (ejemplo)
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/contracts-readme` | Creación del README en /Contracts | Equipo consultor |
| 2026-06-24 | `add/carta-acuerdo-v1` | Subida de carta acuerdo firmada | Coordinador legal |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador Legal).  
- **Correo interno**: `contratos@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: indicar contacto en Governance para disputas o aclaraciones contractuales.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Contracts/`.  
Úsalo como **portada ejecutiva**: explica el propósito, guía el manejo de documentos y asegura la trazabilidad legal del proyecto.
