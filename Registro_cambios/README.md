### 📂 Change-Log / Registro-Cambios

## 🎯 Propósito metodológico
- **Ser el sistema de trazabilidad metodológica** del proyecto, documentando cada ajuste, decisión y cambio realizado.  
- **Garantizar evidencia escrita y defendible** para evitar pérdida de contexto o improvisaciones.  
- **Conectar todas las carpetas del repositorio** mediante un registro centralizado que facilite auditoría y aprendizaje.

---

## 📑 Contenido principal recomendado
- **Archivo principal** `changelog.md` con registro cronológico: fecha, carpeta, decisión, motivo, impacto y responsable.  
- **/decisiones** con documentos que detallan decisiones clave y evidencia de validación.  
- **/ajustes** para modificaciones menores y iteraciones operativas.  
- **/versiones** con copias de versiones anteriores de documentos críticos.  
- **/sintesis** con informes periódicos que resumen cambios acumulados y su efecto metodológico.  
- **/templates** con formatos estandarizados para registrar decisiones y ajustes.

---

## 🗂 Estructura sugerida
| **Subcarpeta** | **Propósito** | **Ejemplo de archivo** |
|---|---|---|
| `/decisiones` | Documentar decisiones clave y su validación | `2026-07-10_decision_redefinir-kpis.md` |
| `/ajustes` | Registrar modificaciones operativas y de formato | `2026-07-12_ajuste_cronograma_v2.md` |
| `/versiones` | Archivar versiones previas de documentos críticos | `2026-06-30_propuesta-tecnica_v1.pdf` |
| `/sintesis` | Resúmenes periódicos de cambios y su impacto | `2026-07_sintesis-cambios.md` |
| `/templates` | Plantillas para entradas de changelog y actas | `template_decision.md` |
| `/changelog` | Archivo maestro con registro cronológico | `changelog.md` |

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_tipo_carpeta_tema_vN.ext
Ejemplo: 2026-07-10_decision_governance_raci-v1.md
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: decision / ajuste / version / sintesis / template.  
- **Carpeta**: governance / reports / pilots / metrics / training / integration.  
- **Versión**: `v1`, `v2`, ... para control de cambios.  
- **Formato**: Markdown para registros vivos; PDF para versiones firmadas.

**Formato sugerido para cada entrada en `changelog.md`**  
- **Fecha** | **Carpeta** | **Decisión** | **Motivo** | **Impacto** | **Responsable**  
- Ejemplo: `2026-07-10 | Governance | Actualizar RACI cocina | Piloto mostró solapamiento de roles | Mejora en tiempos de respuesta | Ana Pérez`

---

## 🧾 Plantillas y ejemplos rápidos
**Plantilla decisión** (usar Markdown)
```markdown
# Decisión ID: DEC-YYYYMMDD-XX
**Fecha**: YYYY-MM-DD
**Carpeta afectada**: Governance / Pilots / Metrics
**Decisión**: Texto breve y claro
**Motivo**: Resumen de evidencia
**Impacto estimado**: Operativo / Financiero / Cultural
**Acciones**: Lista de pasos y responsables
**Estado**: aprobado / en revisión / implementado
**Evidencia**: enlace o ruta al documento
```

**Plantilla ajuste breve**
```markdown
**Fecha**: YYYY-MM-DD
**Origen**: piloto / feedback / auditoría
**Descripción del ajuste**: texto corto
**Archivo afectado**: ruta
**Responsable**: nombre
**Estado**: abierto / cerrado
```

---

## ✅ Buenas prácticas y flujo recomendado
- Registrar **cada decisión** en `/decisiones` y resumirla en `changelog.md` el mismo día.  
- Archivar versiones previas en `/versiones` antes de publicar una actualización.  
- Vincular siempre la entrada del changelog con la **evidencia** (acta, correo, informe, commit).  
- Priorizar claridad: **qué** se cambió, **por qué**, **quién** lo aprobó y **qué** impacto tiene.  
- Mantener una **síntesis mensual** en `/sintesis` para facilitar revisiones ejecutivas.

---

## 🧾 Checklist antes de cerrar una entrada
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos (fecha, carpeta, responsable).  
- [ ] Evidencia asociada adjunta o referenciada.  
- [ ] Estado y versión actualizados.  
- [ ] Entrada reflejada en `/sintesis` si corresponde.

---

## 📝 Historial de cambios ejemplo
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|---|---|---|---|
| 2026-07-10 | `add/decision-raci` | Registro de actualización RACI cocina | Ana Pérez |
| 2026-07-12 | `add/ajuste-cronograma` | Ajuste de cronograma por disponibilidad | Coordinador de Proyecto |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador de Gobernanza).  
- **Correo interno**: `changelog@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: contacto en `Governance/` para validaciones formales.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Change-Log/`.  
Úsalo como **archivo de memoria metodológica**: documenta decisiones, protege contexto y facilita auditoría y aprendizaje continuo.
