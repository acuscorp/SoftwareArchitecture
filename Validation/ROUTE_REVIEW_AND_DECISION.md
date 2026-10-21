---
course_id: SAC01
artifact_id: REVIEW-SAC01-ROUTE
artifact_type: curricular_review_decision
status: STRUCTURE_APPROVED_WITH_DELIVERY_GATES
language: es
review_date: 2026-10-21
---

# Dictamen de revisión curricular — SAC01

## Decisión

Se aprueba **el mapa curricular y su estructura general** para servir como referencia de planificación, con condiciones de entrega por clase. Esta decisión no certifica el dominio del estudiante, no aprueba automáticamente planes de clase, lecturas o evaluaciones, y no resuelve ni migra evidencias individuales. La [matriz maestra de competencias](../MATRIZ_COMPETENCIAS.md) es la fuente de referencia para Software Architecture y AI Solution Architecture; mantiene `DRAFT — PENDING_REVIEW`.

La ruta curricular se revisó conforme al estándar curricular acordado. El dictamen confirma la coherencia estructural básica del mapa: 15 módulos, 63 submódulos, 77 clases y 176 subclases explícitas; los identificadores se conservan. La jerarquía propia de Arquitectura se mantiene.

## Criterios revisados

| Criterio | Resultado | Justificación / límite |
|---|---|---|
| Identidad del curso | PASS | `course_id: SAC01` y el estándar curricular declarados. |
| Jerarquía e IDs | PASS | Módulo → submódulo → clase → subclase; IDs estables. Conteos registrados por la auditoría estructural. |
| Resultados y progresión | PASS WITH GATES | Resultados por módulo y progresión identificable. El detalle didáctico/evidencia se define en cada plan de clase. |
| Prerrequisitos | PASS WITH GATES | Hay entradas observables y dependencias; comprobarlas contra los planes antes de impartir cada clase. |
| Bibliografía | FIX — pendiente por clase | Las fuentes principales están identificadas, pero no todas las lecturas y secciones se han cotejado en contenido. No presentar asignaciones provisionales como obligatorias verificadas. |
| Alineación competencia–actividad–rúbrica | FIX — pendiente por artefacto | Los planes CL01.02.02 y CL01.04.01 tienen correcciones documentadas, pero permanecen `DRAFT_FOR_REVIEW`. No usar como materiales finales hasta completar revisión y validación. |
| Evidencia y estado individual | PASS — sin migración | El estado personal se mantiene separado de la ruta; `CL01-E01` queda en revisión y `CL01-M01` no evaluada. |
| Enlaces e índice | PASS estructural | El índice común y los IDs se preservan; revisar enlaces al añadir nuevos artefactos. |

## Condiciones obligatorias antes de impartir una clase

1. Confirmar que el plan tiene `course_id`, ruta curricular vigente, `artifact_id`, competencia primaria, objetivo observable y prerrequisitos.
2. Verificar la lectura asignada en la edición disponible; marcar como provisional cualquier lectura que solo se cotejó por índice.
3. Confirmar que actividad, evidencia y criterios miden el objetivo sin anticipar contenidos de módulos posteriores.
4. Revisar errores comunes, retroalimentación/remediación, referencias y duración prevista.
5. Aplicar la puerta `DRAFT → REVIEW → FIX → RE-CHECK → READY`; cualquier `FIX` material sin resolver bloquea `READY`.

## Discrepancias y estado del estudiante

- `CL01-E01`: conflicto histórico entre `COMPLETED / VALIDATED` y `IN_PROGRESS / PARTIAL`. Vista canónica: `PENDING_REVIEW` hasta cotejar evidencia original y criterios.
- `CL01-M01`: `IN_PROGRESS / NOT_EVALUATED`; no ejecutar ni marcar dominio sin una evaluación real.
- No mapear evidencia histórica a clases nuevas por similitud temática solamente.

## Dictamen operativo

La ruta curricular queda aprobada **como mapa curricular para planificación**. Los planes, lecturas, rúbricas y migración de progreso conservan sus propios estados y puertas de validación. No se declara que todas las clases estén listas para impartirse.

## Registro de decisión

- Decisión: `STRUCTURE_APPROVED_WITH_DELIVERY_GATES`.
- Alcance: estructura y mapa curricular de la ruta curricular.
- No cubre: validación didáctica de todas las clases, verificación completa de todas las lecturas, evaluación del estudiante ni migración de `COURSE_STATE`.
- Próximo paso: validar los artefactos de la siguiente clase que se impartirá, comenzando por CL01.01.01 y su evidencia histórica asociada.