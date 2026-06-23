### Buenas Prácticas

A continuación se presenta la **guía operativa** para mantener calidad, trazabilidad y seguridad en el repositorio. Aplica a todos los colaboradores y se integra con `Estándares/`, `Metrics/`, `Change-Log/` y `Governance/`.

---

#### Consistencia en Markdown
- **Formato único**: usar Markdown para toda la documentación viva; exportar a PDF/PPT solo las versiones finales en `/exports`.  
- **Estructura mínima**: título, metadatos (Fecha; Autor; Versión; Estado), resumen, cuerpo y referencias a evidencia.  
- **Encabezados semánticos**: H1 para título, H2 para secciones principales, H3 para subsecciones; evitar saltos arbitrarios.  
- **Enlaces relativos**: referenciar archivos dentro del repo con rutas relativas para mantener portabilidad.  
- **Imágenes y evidencias**: subir archivos fuente a la carpeta correspondiente (`/ejecucion`, `/assets`) y enlazarlos desde Markdown; no incrustar datos sensibles.  
- **Plantillas**: usar las plantillas en `Estándares/templates` para informes, SOPs y fichas de medida.  
- **Revisión de estilo**: cada PR que modifique documentación debe pasar un control de formato (linter Markdown) y revisión de contenido.

---

#### Registro de métricas y KPIs
- **Fuente única de verdad**: almacenar raw data en `Metrics/` y resúmenes en `Reports/kpis`.  
- **Definición clara**: cada KPI debe incluir **definición**, **fórmula**, **frecuencia**, **fuente de datos** y **responsable**.  
- **Formato de datos**: usar CSV/Excel para raw data; incluir una hoja con diccionario de campos.  
- **Trazabilidad**: cada gráfico o KPI en informes debe enlazar al archivo de raw data y al script o notebook que generó la visualización.  
- **Versionado**: actualizar la versión del dataset cuando se corrigen o re-procesan datos; registrar el cambio en `Change-Log/changelog.md`.  
- **Validaciones**: automatizar checks básicos (valores nulos, rangos esperados, duplicados) en CI antes de aceptar cambios en `Metrics/`.

---

#### Documentación de aprendizajes y riesgos
- **Captura inmediata**: registrar lecciones y riesgos en `Lessons-Learned/` y `Risk-Register/` el mismo día que se identifican.  
- **Formato mínimo**: fecha; origen; descripción; evidencia; impacto; acción propuesta; responsable; estado.  
- **Vinculación**: cada lección o riesgo debe referenciar pilotos, SOPs o entregables afectados.  
- **Cierre formal**: cuando una lección genera un cambio operativo, actualizar `Estándares/` y dejar registro en `Change-Log/`.  
- **Síntesis periódica**: generar resúmenes mensuales en `/sintesis` para facilitar decisiones ejecutivas.  
- **Banco de buenas prácticas**: documentar condiciones de aplicabilidad para que otras sucursales repliquen con éxito.

---

#### Seguridad y manejo de Secrets
- **Nunca** almacenar credenciales en el repositorio.  
- **Secrets centralizados**: usar GitHub Secrets, vaults o el gestor corporativo; documentar el proceso de rotación en `Integration/docs/README.secrets.md`.  
- **Acceso mínimo**: aplicar principio de menor privilegio para quienes pueden leer/usar secrets.  
- **Referencias en código**: parametrizar conexiones y leer credenciales desde variables de entorno; evitar hardcode.  
- **Auditoría**: registrar cambios de secrets y accesos en el `changelog` de Integración.  
- **Respuesta a exposición**: runbook en `/Integration/docs/runbooks.md` con pasos para rotación inmediata y notificación a Governance.

---

#### Checklist operativo
- [ ] Documento en Markdown con metadatos completos.  
- [ ] Nombre de archivo sigue convención `YYYY-MM-DD_tipo_area_tema_vN.ext`.  
- [ ] Raw data referenciado y validado.  
- [ ] KPI con definición, fórmula y fuente.  
- [ ] Evidencia adjunta o enlace relativo.  
- [ ] PR con revisores asignados según RACI.  
- [ ] Entrada en `Change-Log/changelog.md` generada o prevista.  
- [ ] Secrets y credenciales no incluidos en el commit.

---

#### Responsables y gobernanza
- **Autores**: crean y mantienen contenido operativo.  
- **Coordinadores de carpeta**: validan estructura y cumplimiento de convenciones.  
- **Revisores**: verifican calidad técnica y consistencia con `Estándares/`.  
- **Panel de Validación**: aprueba cambios en políticas, SOPs y estándares críticos.  
- **Contacto**: usar los correos listados en los READMEs de cada carpeta para escalamiento.

