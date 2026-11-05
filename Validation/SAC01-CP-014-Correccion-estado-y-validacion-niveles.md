---
course_id: SAC01
artifact_id: SAC01-CP-014
artifact_type: curricular_change_record
status: APPLIED
approval_authority: user
approval_context: active_conversation
current_course_version: NOT_DECLARED
proposed_course_version: NOT_ASSIGNED
change_date: 2026-11-05
---

# SAC01-CP-014 — Corrección de estado y validación de niveles propuestos

## Decisión aplicada

Se corrige la referencia desactualizada de `LEARNING_PATH.md`: la matriz maestra está `FINAL / APPROVED`, no `DRAFT — PENDING_REVIEW`.

Se aclara que el nivel esperado es un desempeño propuesto para el alcance de cada clase, no una certificación de dominio global ni una secuencia obligatoriamente ascendente cuando se introduce un subalcance distinto.

## Evidencia y justificación

- `MATRIZ_COMPETENCIAS.md` declara `status: FINAL` y `approval_status: APPROVED`.
- `LEARNING_PATH.md` conservaba una referencia contradictoria a matriz pendiente.
- La revisión de la ruta identifica secuencias de una misma competencia con niveles no monotónicos: C02 en M01, C05, C12, C13, C17 y C18. Los títulos y el mapeo disponibles no bastan para cambiar esos valores sin revisar los planes concretos.

## Cambio exacto

| Artefacto | Antes | Después |
|---|---|---|
| `LEARNING_PATH.md` | La matriz se describía como `DRAFT — PENDING_REVIEW`. | La matriz se describe como `FINAL / APPROVED`, con límites explícitos de esa aprobación. |
| `LEARNING_PATH.md` | No había regla para interpretar secuencias no monotónicas. | Se exige declarar el subalcance en el plan posterior o mantener el mapeo pendiente de revisión. |

## Artefactos y alcance afectados

- Curso: `SAC01`.
- Ruta: `LEARNING_PATH.md`.
- Competencias a validar: C02, C05, C12, C13, C17 y C18.
- No se cambian IDs, niveles individuales, objetivos, criterios, materiales ni estado del estudiante.

## Impacto en progreso y migración

No hay migración: no se modifica evidencia, evaluación o estado individual. Los planes afectados deberán registrar su subalcance antes de que un cambio de nivel individual pueda proponerse y validarse.

## Seguimiento requerido

1. Revisar los planes de las clases con secuencias no monotónicas.
2. Para cada una, registrar el subalcance o proponer un nivel distinto con justificación.
3. Asignar una versión activa de curso antes de declarar artefactos finales.
