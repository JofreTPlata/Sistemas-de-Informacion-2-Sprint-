# 📊 Sprint 1 – Informe Scrum  
**Proyecto:** Admisiones — Examen de Ingreso (UMSS)  
**Equipo:** [Ana, Pedro, Carla, Luis, María]  
**Sprint:** 7 días  
**Fecha inicio:** [2025-09-23] — **Fecha fin:** [2025-09-30]  
**Metodología:** Scrum / Iteración fija (Sprint)  
**Motto:** "La mejora continua es la clave del éxito"

---

## 🎯 Objetivo del Sprint
Implementar y validar las funcionalidades críticas del proceso de admisión para el examen de ingreso:  
- Registro de postulantes al examen.  
- Proceso de pago de 500 Bs (opciones QR / transacción).  
- Consulta de nota por parte del postulante.  
- Validación de pagos por el personal de admisión.  

El sprint entrega funcionalidades mínimas operativas con evidencia verificable y documentación.

---

## 🧾 Resumen 
En este Sprint 1 se planificaron **24 subtareas** derivadas de 4 historias principales. Cada subtarea tiene responsable, estimación en horas, y se exige evidencia para considerar la tarea completada (Definition of Done). El control del avance se hará con un **Task Board** (TASK / IN PROGRESS / DONE) y un **Burndown Chart** actualizado diariamente. Se mantiene trazabilidad con convenciones de nombres en archivos y commits.

---

## 🧩 Historias de usuario (detalladas)

| ID     | Historia (resumen)                                                                        | Complejidad |
|--------|-------------------------------------------------------------------------------------------:|------------:|
| US-01  | Registro al examen: como postulante nuevo deseo registrarme para rendir el examen.        | 5           |
| US-02  | Pago por examen: como postulante deseo pagar 500 Bs (QR / transacción) para habilitarme.  | 8           |
| US-03  | Revisar nota: como postulante deseo consultar mi nota después del examen.                 | 3           |
| US-04  | Validación de pago: como personal de admisión deseo validar pagos para habilitar postulantes. | 8           |

**Notas:** cada historia tiene criterios de aceptación mínimos (formulario con validaciones, comprobante, flujo de pago con manejo de errores, login y visualización de nota, listado y verificación para personal).

---

## 🗂️ Backlog (Task Board planificado — 24 subtareas)
> **Instrucción:** copia exactamente esta tabla en `sprint_backlog.xlsx` y usa `SubtaskID` en commits / archivos de evidencia.

| SubtaskID | Historia | Título (subtask)                                                    | Asignado | EstH |
|-----------|---------:|---------------------------------------------------------------------|----------|-----:|
| 01.01     | US-01    | Especificación de campos y reglas de validación                     | Jose     | 4    |
| 01.02     | US-01    | Implementar interfaz de registro (formulario)                       | Jofre / Jose    | 6    |
| 01.03     | US-01    | Validación front/back de credenciales y campos                      | Alberto    | 4    |
| 01.04     | US-01    | Generar comprobante con ID único y exportar a PDF                   | Alberto     | 4    |
| 01.05     | US-01    | Integración con base de datos y pruebas de integridad               | Jofre / Jose    | 4    |
| 02.01     | US-02    | Diseño de interfaz de pago (QR y transacción)                       | Alberto      | 4    |
| 02.02     | US-02    | Implementar generación y visualización de QR de pago                | Jose / Jofre    | 4    |
| 02.03     | US-02    | Implementar pago por transacción (simulación / pasarela)           |  Gerson    | 6    |
| 02.04     | US-02    | Flujo de confirmación y espera de validación de pago                | Gerson     | 4    |
| 02.05     | US-02    | Interfaz y mensajes de error de pago                                | Gerson    | 3    |
| 02.06     | US-02    | Instrucciones de pago (texto y PDF)                                 | Gerson / Alejadra      | 2    |
| 03.01     | US-03    | Implementar login de postulante                                    | Alberto / Alejandra    | 4    |
| 03.02     | US-03    | Interfaz de consulta de documentación y nota                        | Jose / Jofre    | 4    |
| 03.03     | US-03    | Gestión UI de errores de credenciales                               | Jofre / Jose     | 3    |
| 03.04     | US-03    | Pruebas de visualización y privacidad                               | Gerson    | 4    |
| 04.01     | US-04    | Interfaz para listar pagos pendientes y comprobantes                | Alejandra      | 6    |
| 04.02     | US-04    | Visualización y verificación de comprobantes                        | Alejandra    | 4    |
| 04.03     | US-04    | Marcar postulante como habilitado y actualizar estado               | Alejandra    | 4    |
| 04.04     | US-04    | Generar constancia/acta de validación (PDF con metadatos)           | Gerson / Alejandra     | 4    |
| 04.05     | US-04    | Notificación al postulante con instrucciones de subsanación         | Gerson    | 2    |
| 04.06     | US-04    | Registro de auditoría (quién validó, cuándo, comprobante id)        | Gerson      | 4    |
| MISC.01   | Cross    | Integración end-to-end (pago ↔ registro ↔ validación)               | Alejandra    | 6    |
| MISC.02   | Cross    | Documentación operativa y guía de usuario/funcionamiento            | Gerson    | 4    |

---

## ✅ Definition of Done (DoD) — criterio obligatorio
> **Regla inquebrantable:** una subtarea **no** se marca DONE hasta que **TODOS** los ítems aplicables estén cumplidos y documentados.

1. **Entregable adjunto:** archivo con nombre que incluya `SubtaskID` y fecha (ej.: `01.04_comprobante_20250918.pdf`).  
2. **Peer review:** revisión por otro integrante (nombre + fecha) documentada en PR o comentario.  
3. **Commit con SubtaskID:** (si aplica) mensaje de commit incluye `SubtaskID`.  
4. **Pull Request + Merge:** (si aplica) PR con checklist DoD, aprobado y mergeado; screenshot guardado.  
5. **Pruebas:** pasos ejecutados y resultado documentado (archivo o captura).  
6. **Documentación mínima:** README o nota operativa que explique uso/despliegue (si aplica).  
7. **Evidencia legible con timestamp:** imagen o PDF con fecha visible o nombre con timestamp.  
8. **Registro en backlog:** `StartDay`/`EndDay` y `Evidence` completados.  
9. **Firma del revisor/QA:** nombre y fecha del responsable que certifica conformidad.

> *Nota:* ítems 3–4 son `NA` donde no haya código. Debe justificarse en la tarjeta.

---

## 🔁 Reglas operativas del Task Board
- Columnas: `TASK` → `IN PROGRESS` → `DONE`.  
- **Mover a IN PROGRESS:** responsable añade `StartDay` en backlog y comunica en el daily.  
- **Mover a DONE:** DoD completa y evidence adjunta; `EndDay` y `Evidence` en backlog.  
- **WIP limit:** máximo 3 subtareas en `IN PROGRESS` por persona (recomendado 2 si tareas de 6–8h).  
- **Daily standup:** 10–15 min; snapshot del tablero se toma después del daily.  
- **Bloqueos:** crear tarjeta `BLOCKER` con descripción, responsable y fecha; resolver en <24h o escalar.

---

## 📸 Evidencia diaria requerida (Day1..Day7)
Por cada día del sprint se debe entregar una carpeta `Sprint1/Day{n}/` con:

- Screenshot, Fotografias de como fuimos realizando la actividad

**Formato obligatorio:** usa exactamente los nombres de archivo sugeridos para facilitar revisión.

---

## 📉 Burndown Chart — método y código (total_tasks = 24)
- **Eje X:** días 0..7 (día0 inicio).  
- **Eje Y:** subtareas restantes (24).  
- **Línea ideal:** decrece linealmente (24 → 0).  
- **Línea real:** step (escalón), con puntos diarios (sin suavizado).

**Ejemplo de completions por día (suma = 24):** `[3,4,4,4,3,4,2]`

**Código Python (copiar/pegar)**
```python
# burndown_24.py
import matplotlib.pyplot as plt
import numpy as np

total_tasks = 24
# Reemplazar completions_per_day con tus valores reales (suma = total_tasks)
completions_per_day = [3,4,4,4,3,4,2]
days = np.arange(0, len(completions_per_day)+1)  # 0..7

ideal = [ total_tasks * (1 - d/(len(completions_per_day))) for d in days ]

remaining = [total_tasks]
rem = total_tasks
for c in completions_per_day:
    rem -= c
    remaining.append(max(rem,0))

plt.figure(figsize=(10,6))
plt.plot(days, ideal, '--', label='Ideal Remaining', color='gray')
plt.step(days, remaining, where='post', label='Actual Remaining (step)', color='tab:blue')
plt.plot(days, remaining, 'o', color='tab:blue')
plt.title('Burndown Chart - Sprint 1 (24 subtasks)')
plt.xlabel('Day')
plt.ylabel('Subtasks Remaining')
plt.xticks(days)
plt.grid(True, linestyle=':')
plt.legend()
plt.tight_layout()
plt.savefig('Sprint1_Day{n}_YYYYMMDD_Burndown.png', dpi=150)
plt.show()
