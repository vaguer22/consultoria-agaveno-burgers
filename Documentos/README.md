# 📂 Documentos

## Propósito metodológico
- **Servir como base documental central** del proyecto, concentrando insumos técnicos y administrativos.
- **Garantizar evidencia escrita, organizada y trazable** para las fases iniciales del trabajo consultivo.
- **Soportar el diagnóstico**: aquí se registran observaciones, entrevistas y hallazgos que alimentan decisiones posteriores.

---

## Contenido principal recomendado
- **Pre‑diagnóstico inicial**: observaciones preliminares y reflexiones conjuntas con la empresa.  
- **Registros de necesidades**: listados de problemáticas operativas, administrativas y de servicio.  
- **Bitácoras de campo**: notas in situ, cronometrajes, plantillas de observación y checklists.  
- **Revisión documental básica**: manuales internos, reportes financieros y protocolos previos.  
- **Hipótesis iniciales**: supuestos sobre causas y líneas de investigación para el diagnóstico formal.  
- **Carpeta indexada de evidencias**: PDFs, fotos, hojas de cálculo y archivos fuente organizados por tema.

---

## Estructura de carpetas sugerida
- `/entrevistas` → transcripciones, resúmenes y fichas de entrevistado.  
- `/cronometrajes` → registros de tiempos, raw data y análisis.  
- `/bitacoras` → notas diarias y observaciones de campo.  
- `/evidencias` → fotos, videos y documentos escaneados.  
- `/revisiones` → documentos secundarios y referencias.  

---

## Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_tipo_area_tema.ext
Ejemplo: 2026-06-15_pre-diagnostico_cocina.md
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: pre-diagnostico, entrevista, cronometraje, bitacora, revision.  
- **Área**: cocina, barra, servicio, admin, finanzas.  
- **Tema** breve y claro.  
- **Formato**: preferir Markdown para notas y resúmenes; mantener PDFs/Excel en `/evidencias`.  

**Metadatos mínimos en cada documento** (primer bloque del archivo)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Fuente**: entrevista / observación / documento interno  
- **Resumen**: 1–2 líneas con el hallazgo clave

---

## Relación con fases del proyecto
- **Fase I Inicio** → acopio de la carta acuerdo, pre‑diagnóstico y percepciones iniciales.  
- **Fase II Diagnóstico** → entrevistas, cronometrajes, matrices de análisis y línea base de evidencias.  

---

## Buenas prácticas para colaboradores
- Subir archivos a la subcarpeta correspondiente inmediatamente después de la recolección.  
- Mantener versiones finales en `/evidencias` y borradores en `/drafts` si aplica.  
- Referenciar siempre el **ID de piloto** o **número de visita** cuando aplique.  
- Evitar nombres genéricos como `nota1.docx`; usar la convención de nombres.  

---

## Historial de cambios ejemplo
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/documentos-readme` | Creación del README en /Documentos | Equipo consultor |

---

## Checklist antes de cerrar un documento
- [ ] Nombre cumple convención.  
- [ ] Metadatos completos (fecha, autor, fuente, resumen).  
- [ ] Archivo guardado en la subcarpeta correcta.  
- [ ] Evidencias asociadas (fotos, raw data) enlazadas o copiadas en `/evidencias`.  
- [ ] Si es sensible, marcar y seguir protocolo de confidencialidad.

---

## Contacto y responsables
- **Responsable de carpeta**: Nombre del consultor o rol (ej. Coordinador de Diagnóstico).  
- **Correo interno**: `equipo-consultoria@el-agaveno.example` (reemplazar por el real).  
