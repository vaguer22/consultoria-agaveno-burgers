### 📂 Assets — Mapas conceptuales Dashboards y Presentaciones ejecutivas

#### 🎯 Propósito metodológico
- **Traducir datos y diagnósticos en recursos visuales** claros, coherentes y defendibles.  
- **Facilitar la comunicación ejecutiva** con el cliente y el equipo mediante presentaciones y dashboards estandarizados.  
- **Soportar la toma de decisiones** en Planeación y Cierre entregando artefactos listos para validación y entrega.

---

#### 📑 Contenido principal recomendado
- **Mapas conceptuales y diagramas**: flujos de proceso, MEO, esquemas inputs→outputs.  
- **Dashboards de métricas**: vistas operativas y ejecutivas de KPIs por turno, área y canal.  
- **Presentaciones ejecutivas**: slides por fase con narrativa visual y evidencia.  
- **Plantillas visuales**: manual de estilo, paleta de colores, tipografías e iconografía.  
- **Borradores y exports**: `/drafts` para iteración; `/exports` para versiones finales (PDF, PNG, PPTX).  
- **Activos fuente**: archivos editables (PowerPoint, Figma, Excel, .pptx, .xlsx) organizados y versionados.

---

#### 🗂 Estructura de carpetas sugerida y convención de nombres
- `/maps` → mapas conceptuales y diagramas fuente.  
- `/dashboards` → archivos de dashboard, snapshots y definiciones.  
- `/presentations` → slides por fase y versiones finales.  
- `/templates` → plantillas visuales y manual de estilo.  
- `/drafts` → borradores en proceso.  
- `/exports` → PDFs, PNGs y versiones listas para cliente.  

**Convención de archivos**  
```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-06-25_presentation_cierre_kpis_v1.pptx
```
- **Tipo**: map / dashboard / presentation / template / export.  
- **Área**: cocina / servicio / delivery / ejecutivo.  
- **Versión**: `v1`, `v2` para control de cambios.

---

#### 🧩 Plantillas recomendadas y metadatos mínimos
- **Plantillas**: slide ejecutiva (1 slide resumen + 3 slides de evidencia), slide de hallazgos, slide de recomendaciones, dashboard operativo.  
- **Metadatos mínimos** en cada archivo (primer bloque o en el nombre):  
  - **Fecha**: `YYYY-MM-DD`  
  - **Autor**: nombre y rol  
  - **Estado**: draft / review / final  
  - **Resumen**: 1 línea con el mensaje clave

---

#### ✅ Buenas prácticas y checklist antes de exportar
- Mantener **archivos fuente editables** y exports separados.  
- Usar la **plantilla oficial** para todas las presentaciones externas.  
- Verificar consistencia de colores, tipografías y logos según el manual de estilo.  
- Incluir **fuentes de datos** en cada slide que muestre KPIs (referencia a `Metrics/`).  
- **Checklist** antes de exportar:  
  - [ ] Nombre cumple convención.  
  - [ ] Metadatos completos.  
  - [ ] Datos validados y reconciliados.  
  - [ ] Version final guardada en `/exports`.  
  - [ ] Slide de resumen ejecutivo incluida.

---

#### 🧾 Historial de cambios y contacto
- Mantener `changelog.md` con fecha, commit y responsable por cada versión importante.  
- **Responsable de carpeta**: Nombre del diseñador o analista (ej. Diseñador de Insights).  
- **Correo interno**: `assets@el-agaveno.example` (reemplazar por el real).  
