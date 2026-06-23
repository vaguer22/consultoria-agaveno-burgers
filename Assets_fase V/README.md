# 📂 Assets — Presentaciones de cierre y visuales de resultados
---
#### 🎯 Propósito metodológico
- **Traducir visualmente** los KPIs consolidados y hallazgos en narrativas gráficas claras y defendibles.  
- **Facilitar la comunicación ejecutiva** en la fase de cierre con recursos atractivos y comprensibles.  
- **Conectar Reports con entregables visuales** que validen la consultoría frente al cliente y actores clave.

---

#### 📑 Contenido principal recomendado
- **Presentaciones ejecutivas de cierre**  
  - Slides con resumen de KPIs antes/después, narrativa por fases y decisiones clave.  
- **Visuales de resultados**  
  - Dashboards comparativos por área y turno; mapas conceptuales; infografías de aprendizajes.  
- **/exports**  
  - Versiones finales en PDF y PPTX listas para entrega externa; imágenes y gráficos exportados.  
- **/drafts**  
  - Borradores de slides y dashboards en proceso de validación y retroalimentación.  
- **Plantillas visuales estandarizadas**  
  - Diseños modulares reutilizables y manual de estilo visual aplicado a todos los recursos de cierre.  
- **changelog.md**  
  - Registro de versiones, revisiones y motivos de cambio en activos visuales.

---

#### 🗂 Estructura de carpetas sugerida
- `/presentaciones` → slides en formato editable (PPTX, Google Slides) y versiones exportadas.  
- `/dashboards` → archivos fuente de dashboards, snapshots y exports.  
- `/infografias` → PNG/SVG y archivos editables.  
- `/maps` → mapas conceptuales y diagramas en formato editable.  
- `/drafts` → borradores en trabajo.  
- `/exports` → PDF / PPTX / imágenes listas para entrega.  
- `/templates` → plantillas y manual de estilo.  
- `/changelog` → historial de cambios.

---

#### 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-07-20_presentation_cierre_kpis-v1.pptx
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: presentation / dashboard / infographic / template / export / draft.  
- **Área**: cocina / barra / servicio / finanzas / general.  
- **Versión**: `v1`, `v2`, ... para control de cambios.  
- **Formato**: mantener fuentes editables separadas de exports (PPTX/PNG/PDF).

**Metadatos mínimos en cada activo** (primer bloque del archivo o en el nombre)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor / Diseñador**: nombre y rol  
- **Estado**: draft / en revisión / final  
- **Resumen**: 1 línea con el propósito del activo

---

#### ✅ Buenas prácticas y checklist antes de exportar
- **Consistencia visual**: aplicar el manual de estilo (colores, tipografías, logos).  
- **Claridad de datos**: cada gráfico debe incluir **fuente**, **periodo** y **nota metodológica**.  
- **Versionado**: actualizar `changelog.md` con motivo del cambio y responsable.  
- **Accesibilidad**: usar contrastes adecuados y textos alternativos en imágenes clave.  
- **Archivos finales**: exportar PDF/PPTX en `/exports` y conservar fuentes editables en `/presentaciones`.  
- **Checklist**  
  - [ ] Nombre del archivo cumple la convención.  
  - [ ] Metadatos completos (fecha, autor, estado, resumen).  
  - [ ] Fuentes de datos referenciadas en cada visual.  
  - [ ] Versión final exportada a `/exports`.  
  - [ ] `changelog.md` actualizado.

---

#### 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Diseñador de Comunicaciones).  
- **Correo interno**: `assets@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: contacto en `Governance/` para aprobaciones finales.

---

#### 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Assets/`.  
Úsalo como **guía visual** para consolidar y entregar recursos que hagan comprensible, defendible y memorable el impacto de la consultoría.
