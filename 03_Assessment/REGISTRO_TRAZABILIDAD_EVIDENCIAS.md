---
course_id: SAC01
course_version: 1.3
route_version: 1.3
version: 1.4
artifact_id: TRACE-SAC01-v1.4
artifact_type: competency_evidence_traceability
status: DRAFT_FOR_REVIEW
language: es
supersedes: 1.3
change_proposal: SAC01-CP-013
---

# Registro de trazabilidad de competencias y evidencias — Ruta v1.3

## 1. Estado y límites

Esta versión resuelve los desajustes plan–registro identificados en la auditoría v1.0 y conserva el historial de versiones. Mantiene los IDs nuevos `EV-*` y los registros históricos intactos. El estado v4.0.9 conserva el progreso histórico; la ruta v1.3 sigue pendiente de aprobación curricular; las filas indicadas como `PENDING_REVIEW` o `PARTIAL_ALIGNMENT` no son vínculos confirmados. No se evalúa ni modifica el progreso del estudiante.

## 2. Convención de IDs

`EV-<CLASS_ID>-01` identifica la evidencia principal de una clase. Se conserva si el propósito y contrato evaluativo no cambian. Un cambio sustancial del propósito requiere nueva entrada, no reasignación de evidencia histórica.

## 3. Trazabilidad revisada

| Clase | Competencia primaria propuesta | Competencia secundaria / límite | Evidencia | Criterios locales que debe observar la rúbrica | Niveles CR-* candidatos | Estado |
|---|---|---|---|---|---|---|
| CL01.01.01 | C01 | No certificar competencias adicionales | EV-CL01.01.01-01 — explicación operativa de arquitectura aplicada a un caso | Definición operativa; relaciones/propiedades; propósito; límites del caso | CR-C01-IDENTIFY, CR-C01-EXPLAIN; APPLY solo si el caso es nuevo | PENDING_REVIEW |
| CL01.02.01 | C01 | C02 fuera de alcance de esta evidencia | EV-CL01.02.01-01 — mapa de elementos, responsabilidades y relaciones | Elementos/responsabilidades; relaciones; consecuencia/propiedad; límites del modelo | CR-C01-EXPLAIN; CR-C01-APPLY solo con caso nuevo | PENDING_REVIEW |
| CL01.02.02 | C01 | No certifica C02 ni C06; las vistas son introductorias | EV-CL01.02.02-01 — comparación de representaciones de estructura y runtime | Distinción estático/runtime; interacción; pregunta que responde cada representación; límites | CR-C01-EXPLAIN; CR-C01-APPLY solo con caso nuevo | PENDING_REVIEW |
| CL01.03.01 | C02 | Contexto sistémico debe aparecer en el caso | EV-CL01.03.01-01 — clasificación razonada en un caso nuevo | Clasificación; impacto local/sistémico; justificación; contexto | CR-C02-IDENTIFY, CR-C02-EXPLAIN, CR-C02-APPLY | PENDING_REVIEW |
| CL01.04.01 | C02, condicionada a la nueva actividad explícita | La matriz stakeholder sola no certifica C02 ni C18 | EV-CL01.04.01-01 — matriz stakeholder → preocupación → implicación más clasificación de alcance | Stakeholders; preocupaciones; implicación sin prescribir tecnología; clasificación arquitectura vs diseño/implementación; hechos/supuestos | CR-C02-IDENTIFY, CR-C02-EXPLAIN; CR-C02-APPLY en caso nuevo | PENDING_REVIEW |
| CL01.05.01 | C02 como introducción a reconocer decisiones con impacto | No certificar C05; no exigir comparación sistemática ni usar JUSTIFY como criterio de dominio | EV-CL01.05.01-01 — contexto, decisión provisional y consecuencia | Contexto; decisión; consecuencia arquitectónica plausible; incertidumbre | CR-C02-IDENTIFY, CR-C02-EXPLAIN | PENDING_REVIEW |
| CL02.01.01 | C03 | Evidencia parcial de C03, no dominio completo | EV-CL02.01.01-01 — clasificación de necesidades/requisitos/calidad/restricciones | Clasificación; razón; solución vs requisito; datos faltantes | CR-C03-IDENTIFY, CR-C03-EXPLAIN | PENDING_REVIEW |
| CL02.02.01 | C03 | Evidencia parcial de C03, no dominio completo | EV-CL02.02.01-01 — tabla de trazabilidad de requisitos, drivers y ASR | Origen; relevancia arquitectónica; distinciones; incertidumbre | CR-C03-EXPLAIN, CR-C03-APPLY si el caso es nuevo | PENDING_REVIEW |
| CL02.03.01 | C03 | Evidencia parcial de C03, no dominio completo | EV-CL02.03.01-01 — escenario de calidad con seis partes | Seis partes; observabilidad; neutralidad; desconocidos | CR-C03-EXPLAIN, CR-C03-APPLY si el caso es nuevo | PENDING_REVIEW |
| CL02.04.01 | C04 | Evidencia de clase; no basta por sí sola para dominio longitudinal si la matriz exige transferencia adicional | EV-CL02.04.01-01 — registro de riesgo | Riesgo/consecuencia; prioridad; incertidumbre/técnica; proporcionalidad | CR-C04-IDENTIFY, CR-C04-EXPLAIN, CR-C04-JUSTIFY | PENDING_REVIEW |
| CL02.05.01 | C05 | Generar alternativas, sin exigir todavía selección final | EV-CL02.05.01-01 — al menos dos alternativas viables | Diferencia real; relación con drivers; viabilidad; supuestos | CR-C05-IDENTIFY, CR-C05-EXPLAIN, CR-C05-APPLY si se transfiere a caso nuevo | PENDING_REVIEW |
| CL02.05.02 | C05 | La decisión puede ser provisional y explicitar incertidumbre | EV-CL02.05.02-01 — matriz comparativa y registro de decisión | Criterios derivados de drivers; consecuencias; trade-off; decisión/límites | CR-C05-EXPLAIN, CR-C05-JUSTIFY, CR-C05-APPLY si se transfiere | PENDING_REVIEW |

## 4. Cómo interpretar `CR-*`

Los IDs `CR-Cxx-IDENTIFY`, `CR-Cxx-EXPLAIN`, `CR-Cxx-JUSTIFY` y `CR-Cxx-APPLY` representan niveles generales de dominio definidos por la matriz, no criterios completos de contenido. La rúbrica debe puntuar los criterios locales de la tabla anterior y usar `CR-*` para indicar el nivel de razonamiento que aporta esa evidencia. No todas las clases deben medir los cuatro niveles.

## 5. Estados

- `PENDING_REVIEW`: vínculo propuesto, requiere revisión.
- `PARTIAL_ALIGNMENT`: existe un desajuste plan–trazabilidad o la competencia primaria no puede determinarse con suficiente claridad.
- `CONFIRMED`: solo tras validar resultado, evidencia, competencia, nivel y rúbrica.
- `NOT_CREATED`, `NOT_EVALUATED`, `COMPLETED` y `MASTERY_VALIDATED` describen estados de la evidencia o del progreso y solo se asignarán con evidencia real y evaluación; no se establecen en este documento.

## 6. Protección de históricos y bloqueos

No renombrar ni reasignar `CL01-E01`, `CL01-M01`, `CL01-A01`–`CL01-A05` ni `CL01-Q01`. `course_id: SAC01` es el identificador vigente para artefactos nuevos. La ruta v1.3 y los planes siguen pendientes de aprobación formal. Las lecturas Fairbanks de CL02.05.01 y CL02.05.02 requieren verificación textual. Esta versión no modifica el estado del estudiante.

## 7. Acciones resueltas en esta versión

1. CL01.02.01 se alinea con C01; C02 queda fuera de su evidencia principal.
2. CL01.02.02 se alinea con C01 por su foco en estructura, runtime y comportamiento; la noción introductoria de vistas no certifica C06.
3. CL01.04.01 conserva C02 solo porque el plan v1.1 exige clasificar explícitamente una implicación arquitectónica frente a una decisión local. Si esa actividad no se imparte, la evidencia queda `PARTIAL_ALIGNMENT`.
4. CL01.05.01 solo aporta IDENTIFY/EXPLAIN a C02; no evalúa JUSTIFY ni certifica C05.
5. Las 12 evidencias siguen `PENDING_REVIEW` hasta revisar la versión final de cada plan, probar la rúbrica con productos y confirmar gobierno curricular.
6. Los enlaces a niveles `CR-*` son propuestas de nivel; los criterios locales son los elementos puntuables.


## Actualización de identidad del curso — 2026-10-20

**Registro histórico de identidad (2026-10-20):** una versión anterior adoptó `SWARCH-001` conforme a la decisión archivada `DECISION_COURSE_ID_SWARCH-001_v1.0.md`. Una instrucción explícita posterior estableció `SAC01` para los artefactos nuevos. El identificador histórico no se borra ni se usa como identidad vigente.