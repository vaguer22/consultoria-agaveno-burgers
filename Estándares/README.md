# 📂 Estándares — Manuales protocolos y formatos

## Propósito metodológico
- **Establecer el marco normativo y operativo** que garantiza consistencia, defendibilidad y trazabilidad en la ejecución del proyecto.  
- **Proveer formatos y protocolos estandarizados** para levantar información con rigor metodológico.  
- **Facilitar uniformidad** en diagnóstico planeación e implementación.  
- **Conectar Fase II Diagnóstico** con las fases posteriores mediante reglas claras de documentación y control de calidad.

---

## Contenido principal recomendado
- **Manuales operativos**: guías por rol (cocina barra servicio reparto) con pasos estandarizados.  
- **Protocolos normativos**: procedimientos de reuniones auditorías control de calidad seguridad e higiene.  
- **Formatos estandarizados**: plantillas para entrevistas cronometrajes matrices MEO SOPs y fichas de medida.  
- **Manual de estilo visual**: paleta tipografías estructura de presentaciones y uso de logos.  
- **Changelog de estándares**: registro de revisiones y mejoras continuas.  
- **Convenciones de nomenclatura**: reglas para identificar tipo documento área y fecha.

---

## Estructura de carpetas sugerida
- `/manuales`  
- `/protocolos`  
- `/formatos`  
- `/sop`  
- `/style-guide`  
- `/changelog`  
- `/templates`

---

## Convención de nombres y metadatos mínimos
**Convención de archivos**  
```text
YYYY-MM-DD_std_tipo_area_tema_vN.ext
Ejemplo: 2026-06-22_std_sop_cocina_armado-hamburguesa_v1.md
```

**Componentes obligatorios en el nombre**  
- **Fecha**: `YYYY-MM-DD`  
- **Prefijo**: `std` para estándar / `sop` para procedimiento operativo / `fmt` para formato  
- **Tipo**: sop / manual / protocolo / formato / style  
- **Área**: cocina / barra / servicio / admin / finanzas  
- **Tema**: palabra clave breve  
- **Versión**: `v1`, `v2`, ...  

**Metadatos mínimos dentro del documento** (primer bloque)  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Estado**: borrador / en revisión / aprobado  
- **Ámbito**: proyecto / sucursal / área  
- **Resumen**: 1–2 líneas con el propósito del documento

---

## Plantillas y ejemplos rápidos
**Plantilla SOP breve**
```markdown
# SOP ID: SOP-YYYYMMDD-XX
Fecha: YYYY-MM-DD
Autor: Nombre y rol
Área: cocina / barra / servicio
Título: Nombre del procedimiento
Objetivo: 1 línea
Alcance: roles y límites
Materiales y equipos: lista
Pasos: 1. Paso uno 2. Paso dos
Criterios de calidad: indicadores y tolerancias
Registro asociado: ruta al formato
Estado: borrador / aprobado
```

**Plantilla formato de cronometraje**
```markdown
Fecha | Observador | Área | Actividad | Tiempo medido (s) | Condiciones | Notas
```

**Plantilla ficha de entrevista**
```markdown
Fecha: YYYY-MM-DD
Entrevistado: nombre y rol
Entrevistador: nombre
Área: cocina/barra/servicio
Preguntas clave: lista
Resumen hallazgos: 2–3 líneas
Acciones sugeridas: responsable y plazo
Evidencia: ruta
```

---

## Buenas prácticas y flujo de actualización
- Versionar cada cambio y archivar la versión anterior en `/changelog`.  
- Validar estándares críticos con el comité de gobernanza antes de publicar como **aprobado**.  
- Mantener los **formatos en editable** (Markdown/Excel) y las versiones firmadas en PDF.  
- Separar **raw templates** de versiones finalizadas; usar `/templates` para plantillas maestras.  
- Documentar la **fuente de evidencia** que respalda cada estándar (pilotos métricas entrevistas).

---

## Checklist antes de publicar un estándar
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos (fecha autor estado ámbito resumen).  
- [ ] Evidencia que respalda el estándar referenciada.  
- [ ] Versión anterior archivada en `/changelog`.  
- [ ] Aprobación registrada en `Governance/panel-validacion` si aplica.  
- [ ] Formato final exportado a PDF en caso de firma.

---

## Historial de cambios ejemplo
| **Fecha** | **Commit** | **Descripción** | **Responsable** |
|-----------|------------|-----------------|-----------------|
| 2026-06-22 | `init/estandares-readme` | Creación del README en /Estándares | Equipo consultor |

---

## Contacto y responsables
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador de Estándares).  
- **Correo interno**: `estandares@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: contacto en `Governance/` para aprobaciones y disputas.

---

## Nota final
Este README está listo para copiar como `README.md` dentro de la carpeta `Estándares/`.  
Úsalo como **referencia única** para asegurar que todos los procesos se documenten y ejecuten con calidad, coherencia y trazabilidad.
