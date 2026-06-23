# 📂 Governance

## 🎯 Propósito metodológico
- **Establecer el marco de gobernanza** que asegura orden, claridad y trazabilidad desde el inicio del proyecto.  
- **Definir roles y responsabilidades** de todos los actores: consultores, sponsor, gerencia y personal operativo.  
- **Documentar protocolos de comunicación y escalamiento** para evitar ambigüedades y garantizar coordinación efectiva.  
- **Sostener coherencia metodológica** a lo largo de todas las fases del proyecto.

---

## 📑 Contenido principal recomendado
- **Roles y responsabilidades**: descripciones de cargos, alcance por fase y expectativas de entrega.  
- **Protocolos de comunicación**: canales oficiales, frecuencia de reportes y formatos estándar.  
- **Políticas de gobernanza**: reglas de participación, validación de decisiones y trazabilidad documental.  
- **Panel de validación rápida**: comité para aprobaciones operativas y registro de actas.  
- **Matrices RACI**: asignación clara de Responsable, Aprobador, Consultado e Informado por actividad.  
- **Protocolos de crisis**: procedimientos y responsables para incidentes críticos.  
- **Templates y formularios**: actas, solicitudes de cambio, formularios de escalamiento y registro de decisiones.  
- **Changelog**: historial de decisiones, cambios de política y revisiones de gobernanza.

---

## 🗂 Estructura de carpetas sugerida
- `/roles` → descripciones de puestos, organigrama y perfiles por fase.  
- `/protocolos` → comunicaciones, reportes, reuniones y escalamiento.  
- `/raci` → matrices por proceso y actividad.  
- `/panel-validacion` → actas del comité y decisiones rápidas.  
- `/crisis` → planes de contingencia y contactos de emergencia.  
- `/templates` → plantillas reutilizables (actas, solicitudes, formatos).  
- `/changelog` → registro cronológico de cambios y motivos.

---

## 🧭 Convención de nombres y guía de uso
**Convención de archivos**  
```text
YYYY-MM-DD_tipo_documento_tema_vN.ext
Ejemplo: 2026-06-22_raci_cocina_v1.md
```

**Reglas rápidas**  
- **Fecha** al inicio para ordenar cronológicamente.  
- **Tipo**: roles / protocolo / raci / acta / crisis / template / changelog.  
- **Versión**: `v1`, `v2`, ... para control de cambios.  
- **Formato**: Markdown para documentos vivos; PDF para versiones firmadas o aprobadas.

**Metadatos mínimos en cada documento**  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Estado**: borrador / en revisión / aprobado  
- **Ámbito**: proyecto / sucursal / área  
- **Resumen**: 1 línea con el propósito del documento

---

## 🔁 Protocolos de comunicación y escalamiento
- **Canales oficiales**: correo corporativo, GitHub Issues/Discussions, reuniones semanales.  
- **Frecuencia de reportes**: informe semanal operativo; informe ejecutivo quincenal.  
- **Formato de reporte**: resumen ejecutivo, KPIs clave, riesgos abiertos, acciones pendientes.  
- **Escalamiento**:  
  - Nivel 1: Supervisor operativo (respuesta 24 h).  
  - Nivel 2: Gerente operativo (respuesta 48 h).  
  - Nivel 3: Sponsor / Comité de Gobernanza (respuesta 72 h).  
- **Registro**: toda decisión de escalamiento debe quedar registrada en `/panel-validacion` y referenciada en `Change-Log`.

---

## 🧩 Matrices RACI y toma de decisiones
- Mantener una **RACI por proceso clave** (ej. recepción de pedidos, producción, entrega, inventario).  
- Actualizar RACI cuando se implementen pilotos o cambios operativos.  
- Incluir en cada RACI: actividad, responsable, aprobador, consultados e informados, y evidencia de validación.

---

## 🚨 Protocolos de crisis
- **Definición de crisis**: desviaciones críticas que afectan seguridad, cumplimiento legal o continuidad del servicio.  
- **Pasos inmediatos**: notificar al responsable de crisis; activar plan de contingencia; documentar acciones en `/crisis`.  
- **Roles de contingencia**: líder de respuesta, comunicaciones, operaciones y finanzas.  
- **Postmortem**: informe de lecciones aprendidas y actualización de políticas en `/changelog`.

---

## 🧾 Plantillas recomendadas
- **Acta de reunión**: fecha, asistentes, acuerdos, responsables, plazos.  
- **Solicitud de cambio**: descripción, motivo, impacto, aprobación requerida.  
- **Registro de decisión**: ID, fecha, decisión, responsable, evidencia.  
- **Formato de escalamiento**: incidente, impacto, acciones tomadas, estado.

---

## ✅ Buenas prácticas para colaboradores
- Referenciar siempre el **ID del proyecto** y la **fecha** en documentos de gobernanza.  
- No ejecutar cambios operativos sin la aprobación registrada en `/panel-validacion`.  
- Mantener versiones anteriores en `/changelog` y documentar el motivo del cambio.  
- Proteger documentos sensibles y seguir el protocolo de confidencialidad.  
- Revisar RACI y protocolos al inicio de cada fase o cuando se implemente un piloto.

---

## 🧾 Checklist antes de publicar una política
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos (fecha, autor, estado, ámbito, resumen).  
- [ ] Aprobación registrada en `/panel-validacion` si aplica.  
- [ ] Versión anterior archivada en `/changelog`.  
- [ ] Notificación enviada a los roles afectados según RACI.

---

## 📝 Historial de cambios ejemplo
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/governance-readme` | Creación del README en /Governance | Equipo consultor |
| 2026-06-25 | `add/raci-procesos` | Subida de RACI inicial para cocina y servicio | Líder de proyecto |

---

## 📬 Contacto y responsables
- **Responsable de Governance**: Nombre del responsable (ej. Coordinador de Gobernanza).  
- **Correo interno**: `governance@el-agaveno.example` (reemplazar por el real).  
- **Comité de validación**: lista de miembros y roles con contacto directo.

---

## 📌 Nota final
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Governance/`.  
Úsalo como **guía operativa y de control**: define quién hace qué, cómo se comunica el equipo y cómo se toman y registran las decisiones para que el proyecto avance con orden y transparencia.
