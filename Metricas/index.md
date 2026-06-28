# 📂 Metrics — Línea base de KPIs

## 🎯 Propósito
Centralizar definiciones, datos y visualizaciones que permiten medir la **eficiencia**, **calidad**, **satisfacción** y **rentabilidad** del proyecto.  
Esta carpeta garantiza que los KPIs sean **definidos, calculados y versionados** de forma consistente y trazable.

---

## 📑 Estructura y contenido
- **`raw/`** → Datos originales recolectados (CSV, Excel, exportaciones POS, encuestas crudas).  
- **`processed/`** → Datos transformados y tablas limpias; aquí van las definiciones formales de cada KPI (archivo `.md`) y los datasets listos para análisis.  
- **`dashboards/`** → Visualizaciones, reportes ejecutivos y archivos exportables (PNG, PDF, archivos de BI).  
- **`protocols/`** *(opcional)* → Procedimientos para recolección de datos y control de calidad de las mediciones.  
- **`historical/`** *(opcional)* → Series temporales consolidadas y snapshots mensuales/anuales.  
- **`changelog.md`** *(recomendado)* → Registro de cambios en definiciones, fuentes y transformaciones.

---

## 🧭 Convenciones de nombres
Use nombres consistentes para facilitar trazabilidad y automatización:

```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-06-01_raw_cocina_cronometraje_v1.csv
Ejemplo: 2026-06_kpi_cocina_tiempo-servicio_v1.md
```

**Campos clave en el nombre:** fecha; tipo (raw / processed / kpi / dashboard); área; tema; versión.

---

## 📋 Plantilla mínima para definiciones de KPI
Cada KPI documentado en `processed/` debe incluir al menos:

- **ID**: KPI-YYYYMMDD-XX  
- **Nombre**: Nombre claro del indicador  
- **Definición**: Qué mide y por qué importa  
- **Fórmula**: Expresión matemática o pseudocódigo  
- **Unidad**: minutos / % / MXN / unidades  
- **Frecuencia**: diaria / semanal / mensual  
- **Fuente de datos**: archivo o sistema (POS, encuesta, cronometraje)  
- **Responsable**: persona o área  
- **Meta**: objetivo cuantitativo  
- **Último valor**: valor más reciente y fecha  
- **Notas**: supuestos, filtros, transformaciones aplicadas

---

## ✅ Buenas prácticas
- **Raw → Processed → Dashboards**: mantener trazabilidad entre archivos; nunca sobrescribir datos crudos.  
- **Metadatos**: incluir fecha, autor y versión en cada archivo y en frontmatter YAML cuando aplique.  
- **Control de calidad**: documentar anomalías y reglas de limpieza en `processed/` (scripts o README).  
- **Versionado**: incrementar `vN` en el nombre de archivo ante cambios en definición o cálculo.  
- **Validación**: someter nuevas definiciones de KPI al panel de gobernanza antes de publicarlas.  
- **Exportación**: snapshots de dashboards y tablas clave deben guardarse en `dashboards/exports/` para auditoría.

---

## 🔗 Relación con otras carpetas
- **Estándares/** → plantillas y protocolos de recolección.  
- **Governance/** → aprobación de definiciones y cambios críticos.  
- **Pilots/** → datos de pilotos que alimentan ajustes de KPIs.  
- **Reports/** → exportes y presentaciones ejecutivas basadas en dashboards.  
- **Assets/** → imágenes y visuales usados en dashboards y reportes.

---

## 📬 Contacto
- **Responsable de métricas**: Analista de datos designado en `Governance/roles-responsabilidades.md`.  
- **Escalamiento**: Panel de validación → ver `Governance/panel-validacion.md`.  
