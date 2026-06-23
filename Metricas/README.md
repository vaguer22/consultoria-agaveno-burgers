# 📂 Metrics — Línea base de KPIs

## 🎯 Propósito metodológico
- **Establecer una línea base objetiva** de indicadores clave (KPIs) para medir eficiencia, calidad y satisfacción.  
- **Asegurar decisiones fundamentadas en datos verificables y replicables.**  
- **Conectar Fase II (Diagnóstico) con Planeación, Implementación y Cierre** mediante métricas consistentes y trazables.

---

## 📑 Contenido principal recomendado
- **KPIs operativos**  
  - Tiempo promedio de servicio (pedido → entrega).  
  - Tasa de errores en pedidos.  
  - Nivel de merma e inventario.  

- **KPIs emocionales**  
  - Índice de satisfacción del cliente (CSAT).  
  - Clima laboral y percepción del personal.  

- **KPIs financieros**  
  - Ticket promedio por canal (presencial vs delivery).  
  - Margen y rentabilidad por producto.  
  - Dependencia de proveedores clave.  

- **Protocolos de registro**  
  - Plantillas estandarizadas para captura en POS, encuestas y auditorías.  
  - Checklist de observación en campo.  
  - Procedimiento de validación cruzada con reportes internos.  

- **Dashboards y visualizaciones**  
  - Gráficas comparativas por turno, área y canal.  
  - Tableros en Notion / Excel / BI para seguimiento operativo.  

- **Histórico y evolución**  
  - Carpeta indexada con registros mensuales y series temporales.  
  - Documentación de variaciones, anomalías y tendencias.

---

## 🗂 Estructura de carpetas sugerida
- `/kpis-operativos` → hojas de cálculo y definiciones métricas.  
- `/kpis-emocionales` → encuestas, resultados y análisis cualitativo.  
- `/kpis-financieros` → reportes de ticket, margen y proveedores.  
- `/protocolos` → plantillas, formatos POS y guías de captura.  
- `/dashboards` → exports, capturas y definiciones de visualizaciones.  
- `/historico` → series mensuales, raw data y versiones archivadas.  
- `/changelog` → registro de cambios en definiciones y cálculos.

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM_tipo_kpi_area_tema_vN.ext
Ejemplo: 2026-06_kpi_operativo_cocina_tiempo-servicio_v1.xlsx
```

**Reglas rápidas**  
- **Fecha** (YYYY-MM o YYYY-MM-DD) para ordenar series.  
- **Tipo**: kpi / protocolo / dashboard / export / historico.  
- **Área**: cocina / barra / servicio / delivery / finanzas.  
- **Versión**: `v1`, `v2`, ... para control de cambios.  
- **Formato**: Excel/CSV para raw data; Markdown/PDF para definiciones y guías.

**Metadatos mínimos en cada archivo** (primer bloque o en el nombre)  
- **Fecha**: periodo de medición.  
- **Autor/Analista**: nombre y rol.  
- **Definición KPI**: fórmula y fuente de datos.  
- **Frecuencia**: diaria / semanal / mensual.  
- **Estado**: borrador / validado / publicado.

---

## 🔧 Definiciones y protocolos clave (ejemplos)
- **Tiempo promedio de servicio** = tiempo desde confirmación de pedido hasta entrega al cliente; medir en segundos/minutos; fuente: POS + observación.  
- **Tasa de errores** = (nº pedidos con error / nº pedidos totales) × 100; incluir tipo de error (producto, preparación, entrega).  
- **CSAT** = % de respuestas positivas en encuesta post-servicio (escala 1–5; 4–5 = satisfecho).

**Protocolos de validación**  
- Validar raw data semanalmente; reconciliar POS vs. conteos manuales.  
- Documentar anomalías en `/changelog` con causa y corrección.

---

## 📊 Dashboards y visualizaciones
- **Recomendación**: mantener una versión “operativa” (actualización diaria) y una “ejecutiva” (resumen semanal/quincenal).  
- **Elementos mínimos en dashboard**: KPI principal, tendencia 30 días, comparación por turno, alertas de umbral.  
- **Export**: guardar snapshots mensuales en `/dashboards/exports` con fecha y versión.

---

## ✅ Buenas prácticas para colaboradores
- Registrar **definición** y **fuente** de cada KPI antes de publicar.  
- Mantener raw data separado de resúmenes y visualizaciones.  
- Versionar cambios en fórmulas y documentar motivo en `/changelog`.  
- Automatizar extracción cuando sea posible (POS → ETL → dashboard) y documentar el workflow en `/protocolos`.  
- Marcar datos sensibles y seguir protocolo de confidencialidad.

---

## 🧾 Checklist antes de publicar un KPI o dashboard
- [ ] Definición del KPI documentada y aprobada.  
- [ ] Fuente de datos identificada y accesible.  
- [ ] Raw data validado y reconciliado.  
- [ ] Visualización exportada a `/dashboards/exports`.  
- [ ] Entrada en `/changelog` si hubo cambio en cálculo o fuente.  
- [ ] Responsable asignado para seguimiento y actualización.

---

## 📝 Historial de cambios (ejemplo)
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/metrics-readme` | Creación del README en /Metrics | Equipo de Analítica |
| 2026-06-25 | `add/kpi-tiempo-servicio-v1` | Definición y plantilla de cronometraje | Analista operativo |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del analista (ej. Analista de Métricas).  
- **Correo interno**: `metrics@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: indicar contacto en Governance para discrepancias en definiciones.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Metrics/`.  
Úsalo como **guía de referencia** para estandarizar medición, asegurar trazabilidad y facilitar la toma de decisiones basada en datos.### 📂 Metrics — Línea base de KPIs
