---
course_id: SAC01
artifact_id: RUBRICS-SAC01
artifact_type: assessment_rubrics
status: DRAFT_FOR_REVIEW
language: es
change_proposal: SAC01-CP-013
---

# Rúbricas preliminares para evidencias

## Estado y uso

Borrador de trabajo derivado de los 12 planes curriculares y de los niveles de la Matriz de Competencias. No constituye una rúbrica aprobada. Los umbrales propuestos permiten revisión, pero deben validarse contra la [matriz maestra de competencias](../MATRIZ_COMPETENCIAS.md), cuyo estado sigue `DRAFT — PENDING_REVIEW`, y con una aplicación piloto. No se ha evaluado ninguna evidencia del estudiante con este documento.

## Escala común propuesta

| Nivel | Descriptor general |
|---|---|
| 0 — No demostrado | La respuesta falta, es irrelevante o contiene errores conceptuales que impiden evaluar el objetivo. |
| 1 — Parcial | Reconoce algunos elementos, pero omite relaciones importantes, confunde categorías o no justifica lo suficiente. |
| 2 — Competente para la clase | Cumple el resultado específico con razonamiento correcto, evidencia pertinente y límites/incertidumbres explícitos. |
| 3 — Sólido | Además de cumplir, anticipa consecuencias relevantes, compara alternativas cuando corresponde y explica límites de su conclusión. |

**Umbral preliminar:** nivel 2 o superior en todos los criterios esenciales. Un nivel 0 en un criterio esencial requiere refuerzo y nueva aplicación. Esta regla debe revisarse antes de uso formal.

## Rúbricas por evidencia propuesta

### EV-CL01.01.01-01 — Concepto y propósito de arquitectura

| Criterio | Qué observar | Esencial |
|---|---|---|
| Definición operativa | Explica arquitectura sin reducirla a una lista de componentes o a código | Sí |
| Relaciones y propiedades | Conecta elementos, relaciones y propiedades relevantes del caso | Sí |
| Propósito | Explica qué decisiones o cambios condiciona la arquitectura | Sí |
| Límites | Reconoce qué información del caso falta | No |

### EV-CL01.02.01-01 — Elementos, responsabilidades y relaciones

| Criterio | Qué observar | Esencial |
|---|---|---|
| Elementos y responsabilidades | Identifica los elementos relevantes y su responsabilidad | Sí |
| Relaciones | Representa dependencias/interacciones sin contradicciones importantes | Sí |
| Consecuencias | Explica una propiedad o consecuencia de la relación | Sí |
| Claridad | La representación puede ser interpretada por otra persona | No |

### EV-CL01.02.02-01 — Estructura y runtime

| Criterio | Qué observar | Esencial |
|---|---|---|
| Distinción estático/runtime | No confunde estructura con comportamiento durante la ejecución | Sí |
| Secuencia o interacción | Explica cómo colaboran elementos durante un escenario | Sí |
| Vista elegida | La representación corresponde a la pregunta planteada | Sí |
| Límites | Declara qué comportamiento no está modelado | No |

### EV-CL01.03.01-01 — Arquitectura, diseño e implementación

| Criterio | Qué observar | Esencial |
|---|---|---|
| Clasificación | Clasifica decisiones del caso con una razón válida | Sí |
| Impacto | Distingue impacto local de consecuencias sistémicas | Sí |
| Justificación | Explica qué estructura, propiedad o cambio queda condicionado | Sí |
| Contexto | Reconoce que el impacto depende del sistema y sus restricciones | No |

### EV-CL01.04.01-01 — Stakeholders, preocupaciones y alcance de impacto

| Criterio | Qué observar | Esencial |
|---|---|---|
| Stakeholders | Identifica al menos dos participantes pertinentes | Sí |
| Preocupaciones | Diferencia preocupaciones de negocio, técnicas u operativas | Sí |
| Implicación arquitectónica | Relaciona una preocupación con una implicación plausible sin saltar a una tecnología | Sí |
| Clasificación del impacto | Clasifica una implicación como arquitectónica o local de diseño/implementación y justifica el alcance mediante propiedades o consecuencias del sistema | Sí |
| Hechos y supuestos | Distingue información conocida de hipótesis | No |

### EV-CL01.05.01-01 — Registro introductorio de decisión

| Criterio | Qué observar | Esencial |
|---|---|---|
| Contexto | Describe el problema que requiere decisión | Sí |
| Decisión provisional | Expresa la decisión con alcance comprensible | Sí |
| Consecuencia | Explica al menos una consecuencia arquitectónica plausible | Sí |
| Incertidumbre | Registra un supuesto o dato pendiente | No |

### EV-CL02.01.01-01 — Necesidades y requisitos

| Criterio | Qué observar | Esencial |
|---|---|---|
| Clasificación | Distingue necesidad, funcionalidad, calidad y restricción | Sí |
| Razonamiento | Justifica la clasificación con el enunciado | Sí |
| Tecnología vs requisito | Reconoce una solución propuesta como solución, no automáticamente requisito | Sí |
| Información faltante | Evita inventar métricas o restricciones | No |

### EV-CL02.02.01-01 — Drivers y ASR

| Criterio | Qué observar | Esencial |
|---|---|---|
| Trazabilidad | Conecta driver con requisito/necesidad de origen | Sí |
| Relevancia arquitectónica | Explica por qué el driver puede condicionar decisiones | Sí |
| Distinciones | No confunde driver, ASR y tecnología elegida | Sí |
| Incertidumbre | Señala datos que faltan para priorizar | No |

### EV-CL02.03.01-01 — Escenario de atributo de calidad

| Criterio | Qué observar | Esencial |
|---|---|---|
| Seis partes | Incluye fuente, estímulo, entorno, artefacto, respuesta y medida de respuesta | Sí |
| Observabilidad | La respuesta/medida puede comprobarse o se marca como pendiente | Sí |
| Neutralidad de solución | No prescribe tecnología antes de especificar la necesidad | Sí |
| Incertidumbre | No inventa datos desconocidos | No |

### EV-CL02.04.01-01 — Riesgo arquitectónico

| Criterio | Qué observar | Esencial |
|---|---|---|
| Riesgo y consecuencia | Formula un riesgo con consecuencia plausible para el sistema o proyecto | Sí |
| Prioridad | Explica por qué merece atención frente a otros riesgos | Sí |
| Técnica | Vincula una técnica con la incertidumbre que intenta reducir | Sí |
| Proporcionalidad | Justifica por qué la profundidad de análisis es adecuada | Sí |

### EV-CL02.05.01-01 — Alternativas arquitectónicas

| Criterio | Qué observar | Esencial |
|---|---|---|
| Pluralidad real | Propone al menos dos alternativas plausibles y diferentes | Sí |
| Drivers | Relaciona cada alternativa con drivers/restricciones | Sí |
| Viabilidad | Declara supuestos y condiciones de viabilidad | Sí |
| Apertura | No elige solo por familiaridad ni presenta una opción como universal | No |

### EV-CL02.05.02-01 — Comparación y decisión

| Criterio | Qué observar | Esencial |
|---|---|---|
| Criterios | Usa criterios explícitos derivados de los drivers | Sí |
| Consecuencias | Describe beneficios, costes o efectos relevantes por alternativa | Sí |
| Trade-off | Explica qué se gana y qué se sacrifica | Sí |
| Decisión y límites | Registra decisión provisional, supuestos, incertidumbre y reversibilidad cuando aplique | Sí |



## 3.1 Enlace revisado con competencias y niveles de dominio

Los criterios locales de cada rúbrica son los criterios puntuables. Los códigos `CR-*` son niveles generales de dominio de la matriz, no sustitutos de los criterios de contenido. Esta tabla registra el enlace propuesto y evita evaluar niveles fuera del resultado de la clase.

| Evidencia | Competencia / estado | Niveles candidatos | Ajuste obligatorio para evaluación |
|---|---|---|---|
| EV-CL01.01.01-01 | C01, propuesta | IDENTIFY, EXPLAIN; APPLY si el caso es nuevo | Evaluar definición, relaciones/propiedades y propósito; no exigir justificación de alternativas. |
| EV-CL01.02.01-01 | C01 primaria propuesta | EXPLAIN; APPLY si hay transferencia | El plan corregido declara C01, conforme a esta matriz de trazabilidad. No usar esta evidencia para certificar C02. |
| EV-CL01.02.02-01 | C01 primaria propuesta | EXPLAIN; APPLY si hay transferencia | El plan corregido declara C01, conforme a esta matriz de trazabilidad. La elección de representación es introductoria y no certifica C06. |
| EV-CL01.03.01-01 | C02, propuesta | IDENTIFY, EXPLAIN, APPLY | Usar un caso nuevo; aceptar que una clasificación dependa del contexto si la justificación es defendible. |
| EV-CL01.04.01-01 | C02 condicionada a ejecutar el criterio de clasificación de impacto | IDENTIFY, EXPLAIN; APPLY en caso nuevo | La matriz de stakeholders por sí sola no demuestra C02. Es obligatorio clasificar una implicación como arquitectónica o local de diseño/implementación y justificar su alcance. Si no se ejecuta, marcar PARTIAL_ALIGNMENT. |
| EV-CL01.05.01-01 | C02 como introducción; no certificar C05 | IDENTIFY, EXPLAIN | Mantener el ejercicio breve. No puntuar JUSTIFY ni comparación sistemática. Registrar incertidumbre sin exigir ADR completo. |
| EV-CL02.01.01-01 | C03 parcial | IDENTIFY, EXPLAIN | No confundir solución tecnológica con requisito; registrar información faltante. |
| EV-CL02.02.01-01 | C03 parcial | EXPLAIN; APPLY en caso nuevo | Exigir trazabilidad requisito/necesidad → driver/ASR y separar tecnología elegida. |
| EV-CL02.03.01-01 | C03 parcial | EXPLAIN; APPLY en caso nuevo | Comprobar las seis partes y permitir marcar medidas/desconocidos pendientes. |
| EV-CL02.04.01-01 | C04 | IDENTIFY, EXPLAIN, JUSTIFY | La técnica propuesta debe reducir una incertidumbre concreta; la prioridad debe justificarse por consecuencia/impacto. |
| EV-CL02.05.01-01 | C05, etapa de generación | IDENTIFY, EXPLAIN; APPLY si hay transferencia | Exigir alternativas distintas y plausibles, pero no selección final ni trade-off completo. Lectura pendiente de validación textual. |
| EV-CL02.05.02-01 | C05, comparación/decisión | EXPLAIN, JUSTIFY; APPLY si hay transferencia | Comparar alternativas con criterios comunes derivados de drivers; explicar ganancias y sacrificios, supuestos e incertidumbre. Lectura pendiente de validación textual. |

## Reglas de evaluación y retroalimentación

1. Puntuar cada criterio de 0 a 3 con una observación que cite la parte concreta de la evidencia.
2. No asignar nivel por fluidez, extensión o uso de terminología si el razonamiento no lo demuestra.
3. Si falla un criterio esencial, registrar `REQUIRES_REINFORCEMENT`; ofrecer retroalimentación y un caso nuevo o modificado para volver a aplicar.
4. Registrar por separado el resultado de la actividad (`COMPLETED`) y el dominio (`MASTERY_VALIDATED`). Completar una tarea no implica dominio.
5. Para competencias C03–C05, una rúbrica de una sola clase no valida por sí sola toda la competencia; se necesita evidencia acumulada y transferencia según la matriz.
6. No puntuar ni cambiar estados hasta que exista una evidencia real entregada por el estudiante.

## Pendientes antes de aprobación

- Los planes resuelven el mapeo primario de CL01.02.02 a C01 y hacen explícito en CL01.04.01 el criterio de clasificación de impacto requerido para sostener C02. Ambos siguen en borrador hasta revisión curricular.
- Cotejar cada criterio con la matriz de competencias cuando se apruebe formalmente; la matriz de competencias sigue en borrador.
- Confirmar aprobación curricular de la ruta; `course_id: SAC01` ya está establecido para artefactos nuevos.
- Revisar los planes de clase y las lecturas definitivas.
- Pilotar la rúbrica con una evidencia de ejemplo y revisar consistencia entre evaluadores.
- Registrar fecha y responsable de aprobación.


## Actualización de identidad del curso — 2026-10-20

**Registro histórico de identidad (2026-10-20):** una decisión anterior adoptó `SWARCH-001`. Posteriormente se estableció `SAC01` para los artefactos nuevos. El identificador histórico no se usa como identidad vigente.