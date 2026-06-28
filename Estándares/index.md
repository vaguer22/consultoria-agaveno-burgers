# 📂 Estándares — Manuales, protocolos y formatos

## 🎯 Propósito
Ser el **marco normativo y operativo** del proyecto, asegurando que todos los procesos se documenten y ejecuten con **consistencia, defendibilidad y trazabilidad**.  
La carpeta concentra manuales, protocolos y formatos que sirven como referencia oficial para el equipo consultor y operativo.

---

## 📑 Subcarpetas

---

#### 1. `sop/`
- **Qué guarda:** Procedimientos Operativos Estandarizados (Standard Operating Procedures).  
- **Propósito:** Documentar paso a paso cómo se realizan las tareas críticas en cocina, barra, servicio o reparto.  
- **Formato:** Markdown con frontmatter + checklist; versión final en PDF para firma.  
- **Ejemplo:** `2026-06-22_sop_cocina_armado-hamburguesa_v1.md`.

---

#### 2. `manuales/`
- **Qué guarda:** Guías prácticas por rol (ej. manual del cocinero, manual del bartender).  
- **Propósito:** Capacitar al personal con instrucciones claras y consistentes.  
- **Formato:** Markdown con secciones de objetivos, responsabilidades, procedimientos y criterios de calidad.  
- **Ejemplo:** `2026-06-22_manual_servicio_atencion-cliente_v1.md`.

---

#### 3. `protocolos/`
- **Qué guarda:** Normas y procedimientos normativos (reuniones, auditorías, seguridad e higiene).  
- **Propósito:** Asegurar cumplimiento de estándares regulatorios y de calidad.  
- **Formato:** Markdown con pasos, responsables y criterios de cumplimiento.  
- **Ejemplo:** `2026-06-22_protocolo_seguridad-higiene_v1.md`.

---

#### 4. `formatos/`
- **Qué guarda:** Plantillas para levantar información (entrevistas, cronometrajes, matrices MEO, fichas de medida).  
- **Propósito:** Estandarizar la recolección de datos y asegurar trazabilidad.  
- **Formato:** Markdown/CSV/Excel según necesidad; siempre con metadatos.  
- **Ejemplo:** `2026-06-22_fmt_cronometraje_cocina_v1.xlsx`.

---

#### 5. `style-guide/`
- **Qué guarda:** Lineamientos visuales (paleta de colores, tipografía, estructura de presentaciones, uso de logos).  
- **Propósito:** Mantener coherencia visual en todos los documentos y presentaciones.  
- **Formato:** Markdown + ejemplos gráficos en PNG/SVG.  
- **Ejemplo:** `2026-06-22_style_presentaciones_v1.md`.

---

#### 6. `templates/`
- **Qué guarda:** Plantillas Markdown para SOPs, KPIs, riesgos, lecciones aprendidas y entregables.  
- **Propósito:** Servir como punto de partida para crear nuevos documentos con consistencia.  
- **Formato:** Archivos `.md` con frontmatter YAML y estructura predefinida.  
- **Ejemplo:** `sop-template.md`, `kpi-template.md`, `risk-template.md`.

---

### 🔗 Cómo se relacionan entre sí
- **`sop/`** se alimenta de pilotos (`Pilots/`) y métricas (`Metrics/`).  
- **`manuales/`** y **`protocolos/`** se actualizan con aprendizajes (`Lessons-Learned/`).  
- **`formatos/`** son usados en campo y luego exportados a `Reports/`.  
- **`style-guide/`** asegura que tanto `Reports/` como `Assets/` mantengan coherencia visual.  
- **`templates/`** son la base para crear cualquier documento nuevo en las demás subcarpetas.

---

## ✅ Buenas prácticas
- Usar siempre **nombres de archivo con convención**: `YYYY-MM-DD_std_tipo_area_tema_vN.md`.  
- Incluir **frontmatter YAML** con metadatos mínimos (fecha, autor, versión, estado, área, fase, resumen).  
- Versionar cambios críticos y conservar historial en `changelog.md`.  
- Separar **documentos en borrador** de los **aprobados** para evitar confusión.  
- Revisar periódicamente los manuales y protocolos para mantenerlos actualizados.  

---

## 📬 Contacto
- **Responsable de Estándares**: Coordinador designado en `Governance/roles-responsabilidades.md`.  
- **Escalamiento**: Panel de validación → ver `Governance/panel-validacion.md`.  
