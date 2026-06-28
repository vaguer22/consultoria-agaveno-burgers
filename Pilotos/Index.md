# 📂 Pilots — Pruebas piloto y validación en campo

## 🎯 Propósito
Proveer un espacio controlado para diseñar, ejecutar y evaluar **pruebas piloto** que validen cambios operativos, recetas, layouts o iniciativas antes de su escalado.  
La carpeta centraliza protocolos de piloto, resultados, análisis y recomendaciones para tomar decisiones basadas en evidencia.

---

## 📑 Estructura y contenido
- **`design/`** → Documentos de diseño del piloto: objetivos, hipótesis, alcance, criterios de éxito.  
- **`execution/`** → Registros de ejecución: cronogramas, listas de control, logs de incidencias y observaciones de campo.  
- **`data/`** → Datos recolectados durante el piloto (raw y procesados): cronometrajes, ventas, encuestas, fotos de evidencia.  
- **`analysis/`** → Análisis cuantitativo y cualitativo: tablas, gráficos, conclusiones y recomendaciones.  
- **`reports/`** → Informe final del piloto con decisión: aprobado para escalar / ajustar y re-pilotar / descartado.  
- **`templates/`** → Plantillas para diseño, checklist de ejecución, formatos de recolección y reporte final.

---

## 🧭 Flujo recomendado
1. **Diseño**: documentar hipótesis, métricas y criterios de éxito en `design/`.  
2. **Aprobación**: someter diseño al panel de gobernanza si aplica.  
3. **Ejecución**: usar `execution/` para registrar cada corrida del piloto; mantener `data/` sincronizada.  
4. **Análisis**: consolidar y limpiar datos en `data/`, luego analizar en `analysis/`.  
5. **Decisión**: generar informe en `reports/` con recomendación clara y acciones siguientes.  
6. **Cierre**: si se aprueba el escalado, actualizar SOPs y Estándares; si no, documentar lecciones aprendidas.

---

## ✅ Criterios mínimos para un piloto reproducible
- **Hipótesis clara**: qué se prueba y por qué.  
- **Métricas definidas**: KPIs primarios y secundarios, método de medición y frecuencia.  
- **Duración y tamaño**: periodo del piloto y muestra mínima necesaria.  
- **Plan de recolección**: formatos y responsables por dato.  
- **Criterios de éxito**: umbrales cuantitativos y condiciones cualitativas.  
- **Registro de cambios**: versión del piloto y cambios durante la ejecución.

---

## 🔗 Relación con otras carpetas
- **Estándares/** → plantillas y protocolos que guían diseño y recolección.  
- **Metrics/** → KPIs usados para evaluar resultados y alimentar dashboards.  
- **Governance/** → aprobación de pilotos que afectan procesos críticos.  
- **Lessons-Learned/** → aprendizajes que surjan y recomendaciones para SOPs.  
- **Reports/** → informes ejecutivos y presentaciones para stakeholders.

---

## 📬 Contacto y responsabilidades
- **Responsable de pilotos**: Coordinador de Pilotos (ver `Governance/roles-responsabilidades.md`).  
- **Analista de datos**: persona encargada de consolidar `data/` y generar `analysis/`.  
- **Escalamiento**: Panel de validación → ver `Governance/panel-validacion.md`.  
