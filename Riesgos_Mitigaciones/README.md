# 📂 Risk-Register — Riesgos y mitigaciones
---
## 🎯 Propósito metodológico
- **Ser el sistema de gestión de riesgos** del proyecto, donde se identifican, clasifican y documentan los riesgos que afectan la operación y la consultoría.  
- **Asegurar mitigaciones definidas y trazables** para cada riesgo, evitando improvisaciones y fortaleciendo la resiliencia del proyecto.  
- **Conectar diagnóstico con implementación** mostrando cómo los riesgos detectados se gestionan en tiempo real.

---

## 📑 Contenido principal recomendado
- **/identificacion** Registro inicial de riesgos por área y matriz de probabilidad e impacto.  
- **/analisis** Evaluaciones detalladas de riesgos críticos y escenarios.  
- **/mitigacion** Planes de acción, protocolos de contingencia y responsables.  
- **/seguimiento** Evidencia de riesgos enfrentados durante pilotos e implementación y efectividad de mitigaciones.  
- **/sintesis** Informe consolidado de riesgos gestionados y recomendaciones.  
- **changelog.md** Historial de cambios en clasificación y mitigaciones.

---

## 🗂 Estructura sugerida
| **Subcarpeta** | **Propósito** | **Ejemplo de archivo** |
|---|---|---|
| `/identificacion` | Listado inicial y matriz riesgo | `2026-07-01_identificacion_riesgos-cocina.md` |
| `/analisis` | Evaluaciones y escenarios | `2026-07-05_analisis_riesgo-falta-personal.md` |
| `/mitigacion` | Planes de acción y responsables | `2026-07-06_mitigacion_plan-rotacion-personal_v1.md` |
| `/seguimiento` | Registros de eventos y efectividad | `2026-07-12_seguimiento_incidente-inventario.md` |
| `/sintesis` | Informe consolidado y lecciones | `2026-07_sintesis-riesgos.md` |
| `/changelog` | Registro maestro de cambios | `changelog.md` |

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_tipo_area_tema_vN.ext
Ejemplo: 2026-07-06_mitigacion_cocina_plan-rotacion_v1.md
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: identificacion / analisis / mitigacion / seguimiento / sintesis / version.  
- **Área**: cocina / barra / servicio / finanzas / tecnologia.  
- **Versión**: v1, v2, v3 para control de cambios.  
- **Formato**: Markdown para registros vivos; PDF para planes aprobados.

**Metadatos mínimos en cada registro**  
- **Fecha**  
- **Autor**  
- **Riesgo ID** único (ej. RSK-001)  
- **Descripción breve**  
- **Probabilidad** alta media baja  
- **Impacto** alto medio bajo  
- **Responsable**  
- **Estado** abierto en progreso mitigado cerrado

---

## 🔧 Plantillas y formato recomendado
**Plantilla riesgo breve**
```markdown
# Riesgo ID RSK-YYYYMMDD-XX
Fecha: YYYY-MM-DD
Área: cocina / barra / servicio / finanzas / tecnologia
Descripción: breve
Probabilidad: alta / media / baja
Impacto: alto / medio / bajo
Mitigación propuesta: pasos resumidos
Responsable: nombre
Plazo: YYYY-MM-DD
Estado: abierto / en progreso / mitigado / cerrado
Evidencia: ruta o enlace
```

**Plantilla plan de mitigación**
- **Objetivo**: qué se busca evitar o reducir  
- **Acciones**: lista numerada con responsables y plazos  
- **Recursos**: personas, materiales, presupuesto estimado  
- **Indicadores de éxito**: cómo medir efectividad  
- **Plan de comunicación**: a quién informar y cuándo

---

## 🔁 Flujo recomendado de gestión de riesgos
1. **Identificar** riesgo y asignar Riesgo ID.  
2. **Clasificar** por probabilidad e impacto y priorizar.  
3. **Analizar** causas raíz y escenarios.  
4. **Diseñar mitigación** con responsables y plazos.  
5. **Ejecutar** acciones y registrar en `/seguimiento`.  
6. **Evaluar** efectividad y actualizar estado.  
7. **Documentar** lecciones en `/sintesis` y registrar cambios en `changelog.md`.

---

## ✅ Checklist antes de cerrar un riesgo
- [ ] Riesgo ID asignado y archivo creado.  
- [ ] Metadatos completos y responsable definido.  
- [ ] Plan de mitigación documentado y aprobado.  
- [ ] Evidencia de ejecución subida a `/seguimiento`.  
- [ ] Indicadores de éxito medidos y reportados.  
- [ ] Estado actualizado a mitigado o cerrado.  
- [ ] Entrada en `changelog.md` con motivo y responsable.

---

## 🧾 Buenas prácticas y recomendaciones
- Priorizar riesgos que afecten seguridad, cumplimiento legal o continuidad del servicio.  
- Mantener trazabilidad cruzada entre `Risk-Register` y `Pilots` `Metrics` `Governance` `Reports`.  
- Revisar y actualizar la matriz de riesgos semanalmente durante la implementación.  
- Probar planes de contingencia en pilotos cuando sea posible.  
- No almacenar credenciales ni datos sensibles en los registros de riesgo.

---

## 📝 Historial de cambios ejemplo
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|---|---:|---|---|
| 2026-07-01 | `init/risk-register` | Creación del README y estructura inicial | Coordinador de Riesgos |
| 2026-07-12 | `add/mitigacion-inventario` | Plan de mitigación por faltantes de stock | Analista operativo |

---

## 📬 Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable Riesgos  
- **Correo interno**: `risk@el-agaveno.example` reemplazar por el real  
- **Escalamiento**: contacto en `Governance` para decisiones críticas

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Risk-Register/`.  
Úsalo como **guía operativa** para identificar, gestionar y documentar riesgos de forma clara, trazable y orientada a la mitigación efectiva.
