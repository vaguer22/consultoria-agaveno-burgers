# 📂 Carpeta Lessons-Learned / Aprendizajes y buenas prácticas
---
### Propósito metodológico 🎯
- **Consolidar la memoria organizativa** del proyecto: capturar aprendizajes, aciertos y errores para que la organización los use en futuras iniciativas.  
- **Transformar experiencia en conocimiento accionable**, identificando prácticas replicables y riesgos a evitar.  
- **Cerrar el ciclo de mejora continua**: asegurar que lo aprendido en la Fase V trascienda el proyecto y se integre en procesos, entrenamientos y gobernanza.

---

### Contenido y estructura 📂
- **/operativos** — Lecciones del personal de cocina, barra, servicio y reparto; ejemplos prácticos y mejoras en SOPs.  
- **/clientes** — Retroalimentación de clientes y evidencia de impacto en la experiencia.  
- **/consultores** — Reflexiones metodológicas, ajustes de enfoque y recomendaciones técnicas.  
- **/sintesis** — Informe consolidado con aprendizajes clave, métricas asociadas y recomendaciones estratégicas.  
- **/banco-practicas** — Listado de buenas prácticas con contexto, impacto y condiciones de aplicación.  
- **/changelog.md** — Registro de cómo los aprendizajes se integraron en protocolos, métricas y entrenamientos.

---

### Convención de nombres y plantillas 🧾
**Convención de archivos**  
```text
YYYY-MM-DD_origen_tema_vN.ext
Ejemplo: 2026-07-20_operativos_checklist-visual-cocina_v1.md
```

**Metadatos mínimos en cada entrada**  
- **Fecha**: `YYYY-MM-DD`  
- **Autor**: nombre y rol  
- **Origen**: operativos / clientes / consultores  
- **Contexto**: fase, sucursal, turno  
- **Resumen**: 1–2 líneas con la lección clave  
- **Acción propuesta**: responsable y plazo

**Plantilla breve de lección** (usar Markdown)
```markdown
# Lección ID: LL-YYYYMMDD-XX
**Fecha**: YYYY-MM-DD
**Origen**: operativos / clientes / consultores
**Contexto**: sucursal, turno, fase
**Descripción**: ¿Qué pasó? (breve)
**Por qué importa**: impacto observado
**Evidencia**: ruta o enlace al archivo
**Acción propuesta**: pasos, responsable, plazo
**Estado**: abierta / en progreso / cerrada
```

---

### Buenas prácticas y checklist ✅
- **Capturar la lección el mismo día** que se identifica; enlazar siempre a la evidencia (cronometrajes, fotos, actas).  
- **Clasificar por origen y fase** para facilitar búsquedas y análisis transversales.  
- **Priorizar replicabilidad**: describir condiciones necesarias para que la práctica funcione en otro contexto.  
- **Actualizar protocolos** cuando una lección derive en un cambio operativo; registrar la actualización en `Change-Log/`.  

**Checklist antes de cerrar una lección**
- [ ] Nombre del archivo cumple la convención.  
- [ ] Metadatos completos.  
- [ ] Evidencia asociada adjunta o referenciada.  
- [ ] Acción propuesta con responsable y plazo.  
- [ ] Entrada reflejada en `/sintesis` si corresponde.  
- [ ] `changelog.md` actualizado si la lección generó un cambio formal.

---

### Historial y responsables 🧾
- **/changelog.md** debe contener entradas que expliquen cómo cada lección fue incorporada en políticas, entrenamientos o métricas.  
- **Responsable de carpeta**: Nombre del responsable (ej. Coordinador de Lecciones Aprendidas).  
- **Correo interno**: `lessons@el-agaveno.example` (reemplazar por el real).  
- **Escalamiento**: indicar contacto en `Governance/` para decisiones que impliquen cambios de alcance o presupuesto.

---

### Nota final 📌
Este README está listo para copiar y pegar como `README.md` dentro de la carpeta `Lessons-Learned/`.  
Úsalo como **archivo vivo de aprendizaje**: documenta lo que funcionó y lo que no, facilita la transferencia de conocimiento y convierte la experiencia del proyecto en ventaja competitiva para *El Agaveño Burgers*.
