### Entregables Clave

---

#### Tabla resumen de entregables
| **Entregable** | **Descripción** | **Responsable** | **Criterio de aceptación** | **Formato; Ruta** |
|---|---|---:|---|---|
| **Informe diagnóstico** | Documento que consolida observaciones in situ, cronometrajes, entrevistas y matriz MEO.   [Página actual](citation-section://1396814856/12) | Analista de Diagnóstico | Contiene línea base de tiempos; matriz MEO; lista priorizada de necesidades; validado por cliente. | Markdown/PDF; `Reports/diagnostico/` |
| **Plan estratégico / Roadmap** | Paquete con medidas priorizadas, fichas de medida (KPIs, criterios) y cronograma Gantt.   [Página actual](citation-section://1396814856/16) | Líder de Planeación | Roadmap con dependencias y responsables; fichas de medida con KPIs y criterios de aceptación. | Markdown/Gantt/PDF; `Roadmap/` |
| **SOPs validados** | Procedimientos estandarizados resultantes de pilotos y ciclos Kaizen, listos para operación.   [Página actual](citation-section://1396814856/20) | Coordinador de Operaciones | SOPs probados en piloto; checklist de cumplimiento ≥ umbral acordado; aprobados por panel. | Markdown/PDF; `Estándares/sop/` |
| **Informe final de consultoría** | Informe consolidado con KPIs comparativos (baseline vs final), evidencia y recomendaciones estratégicas.   [Página actual](citation-section://1396814856/22) | Equipo consultor / Coordinador de Cierre | Resumen ejecutivo; KPIs consolidados con fuentes; anexos con raw data; aprobado por cliente. | Markdown/PDF; `Reports/final/` |
| **Presentación ejecutiva** | Slide deck para entrega al cliente con narrativa visual de impacto y próximos pasos.   [Página actual](citation-section://1396814856/23) | Responsable de Comunicaciones / Diseñador | Slide deck ≤ 15 slides; incluye KPIs clave, decisiones y plan de sostenibilidad; versión final exportada. | PPTX/PDF; `Assets/presentaciones/` |

---

#### Detalle operativo y flujo de entrega
- **Versionado**: cada entregable debe seguir la convención `YYYY-MM-DD_tipo_tema_vN.ext` y registrar la entrada en `Change-Log/changelog.md`.  
- **Evidencia**: todo entregable que incluya métricas debe adjuntar o referenciar raw data en `Metrics/` o `Reports/exports`.  
- **Aprobación**: entregables en `Estándares/` o que modifiquen gobernanza requieren aprobación del **Panel de Validación** (ver `Governance/panel-validacion`).   [Página actual](citation-section://1396814856/16)  
- **Publicación**: versión final exportada a `/exports` y copia editable conservada en la carpeta de trabajo correspondiente.

---

#### Cronograma típico de entregas (ejemplo)
- **Semana 0–2**: Recolección y análisis para **Informe diagnóstico**.   [Página actual](citation-section://1396814856/12)  
- **Semana 3–4**: Diseño de **Plan estratégico** y Roadmap; validación inicial.   [Página actual](citation-section://1396814856/16)  
- **Semana 5–8**: Pilotos y ajuste de **SOPs**; registro en `Pilots/` y `Estándares/`.   [Página actual](citation-section://1396814856/20)  
- **Semana 9–10**: Consolidación de KPIs y redacción del **Informe final**; preparación de **Presentación ejecutiva**.   [Página actual](citation-section://1396814856/22)  [Página actual](citation-section://1396814856/23)

---

#### Checklist mínimo antes de entregar
- [ ] Archivo cumple convención de nombres.  
- [ ] Metadatos completos (fecha, autor, versión, estado).  
- [ ] KPIs con definiciones, fórmulas y fuentes documentadas.  
- [ ] Raw data referenciado o adjunto.  
- [ ] Evidencia de validación (acta, firma, correo) incluida.  
- [ ] Versión final exportada a `/exports`.  
- [ ] Entrada en `Change-Log/changelog.md` con motivo y responsable.

---

#### Recomendaciones prácticas
- Mantener **plantillas** para cada entregable en `Estándares/templates` para acelerar producción y asegurar consistencia.  
- Vincular cada entregable con su **ID de proyecto** y con los Issues/PRs que originaron los cambios para trazabilidad.  
- Priorizar la **claridad ejecutiva** en la presentación final: una slide con impacto cuantificado (números antes/después) debe aparecer al inicio.   [Página actual](citation-section://1396814856/23)
