---
artifact_id: COMPETENCY_MATRIX_SOFTWARE_AND_AI_ARCHITECTURE
artifact_type: COMPETENCY_MATRIX
status: FINAL
approval_status: APPROVED
scope:
  - Software Architecture
  - AI Solution Architecture
---

# Matriz maestra de competencias — Software Architecture y AI Solution Architecture

## 1. Propósito

Esta matriz define las competencias que debe desarrollar y demostrar una persona a lo largo de dos niveles formativos relacionados:

1. **Software Architecture:** fundamentos y práctica de arquitectura de software, independientemente de que la solución use IA.
2. **AI Solution Architecture:** diseño de soluciones que incorporan modelos y sistemas de inteligencia artificial, reutilizando los fundamentos de arquitectura de software y añadiendo competencias específicas.

La matriz es la fuente de referencia para definir resultados de aprendizaje, alinear clases y diseñar criterios de evaluación. No sustituye la ruta curricular, los planes de clase, las rúbricas ni el registro de evidencias.

**Estado:** versión final aprobada por el responsable del curso para servir como matriz maestra de referencia. La aprobación establece la línea base curricular; no certifica por sí misma el dominio de estudiantes ni impide revisiones futuras versionadas.

## 2. Principios de diseño

- Mantener estables los identificadores existentes `C01`–`C18`; no reutilizarlos ni renumerarlos.
- Usar una matriz maestra compartida, en lugar de mantener matrices desconectadas por nivel.
- Identificar el nivel principal de cada competencia y marcar explícitamente las competencias transversales.
- Agregar competencias específicas de IA con identificadores `AI01`, `AI02`, etc., sin alterar los IDs existentes.
- No inferir dominio por haber leído, visto o practicado un tema una sola vez.
- Exigir evidencias observables, trazables a criterios concretos y proporcionales al alcance de cada competencia.
- Distinguir las competencias definidas de las competencias ya demostradas por una persona. Esta matriz no registra el progreso individual.

## 3. Niveles formativos

### Software Architecture

Desarrolla la capacidad de analizar contexto y requisitos, tomar y comunicar decisiones arquitectónicas, evaluar alternativas y diseñar sistemas mantenibles, seguros y evolutivos.

### AI Solution Architecture

Desarrolla la capacidad de diseñar soluciones completas que incorporan modelos de IA, datos, recuperación, herramientas y agentes cuando sean apropiados, evaluación, controles de riesgo y operación. No equivale solamente a saber usar un modelo o construir un prototipo.

### Competencias transversales

Se aplican a ambos niveles cuando corresponda. Su complejidad aumenta según el contexto, el riesgo, la escala y el impacto de la solución.

## 4. Niveles de dominio

Los cuatro niveles describen la progresión del razonamiento. No todas las clases tienen que exigir los cuatro niveles; cada plan debe declarar cuáles evalúa.

| Nivel | Definición general | Evidencia observable general |
|---|---|---|
| **IDENTIFICAR** | Reconoce un concepto, problema, restricción, riesgo o alternativa relevante en un caso. | Señala los elementos pertinentes y distingue los datos conocidos de los desconocidos. |
| **EXPLICAR** | Describe el concepto y las relaciones causales relevantes. | Explica por qué importa, cómo se relaciona con otros elementos y qué consecuencias puede tener. |
| **JUSTIFICAR** | Compara alternativas con criterios explícitos, restricciones, riesgos y trade-offs. | Defiende una decisión con razones y evidencia, declara supuestos e incertidumbre y reconoce desventajas. |
| **APLICAR** | Usa el razonamiento en un caso nuevo y suficientemente delimitado. | Produce una solución o artefacto coherente, explica sus decisiones y demuestra que responde al contexto y a los criterios. |

### IDs de criterios para trazabilidad

Los IDs de criterios siguen esta convención:

- `CR-<ID>-IDENTIFY`
- `CR-<ID>-EXPLAIN`
- `CR-<ID>-JUSTIFY`
- `CR-<ID>-APPLY`

Por ejemplo, `CR-C03-JUSTIFY` identifica el criterio de JUSTIFICAR para C03. Los IDs sirven para enlazar planes, evidencias y rúbricas; no certifican por sí mismos que una persona haya alcanzado ese nivel.

La descripción general de cada nivel se debe complementar con criterios específicos de la competencia. No se debe evaluar una competencia usando únicamente la definición genérica del nivel.

## 5. Catálogo de competencias existentes

Las competencias C01–C18 se conservan como identificadores históricos estables. La asignación de bloque procede de la matriz anterior y debe cotejarse con la ruta curricular vigente antes de aprobar la matriz.

| ID | Competencia | Nivel principal | Evidencia de dominio esperada |
|---|---|---|---|
| C01 | Definir arquitectura de software operativamente | Software Architecture | Explica estructuras, elementos, relaciones, propiedades y comportamiento relevante sin reducir la arquitectura a una lista de componentes. |
| C02 | Reconocer el impacto arquitectónico | Software Architecture | Distingue decisiones arquitectónicas de decisiones locales de diseño o implementación, justificando la clasificación según el contexto. |
| C03 | Traducir requisitos a drivers arquitectónicos | Software Architecture | Relaciona necesidades de stakeholders, requisitos, atributos de calidad, restricciones, ASR y riesgos; registra información faltante. |
| C04 | Analizar riesgos arquitectónicos | Software Architecture | Formula escenarios de riesgo, identifica incertidumbres y selecciona técnicas proporcionadas para investigarlas o reducirlas. |
| C05 | Analizar decisiones y trade-offs | Software Architecture | Compara alternativas plausibles mediante criterios explícitos y justifica consecuencias, costes, riesgos y compromisos. |
| C06 | Modelar y comunicar arquitectura | Software Architecture | Selecciona y construye vistas o modelos adecuados para stakeholders y preocupaciones concretas, indicando límites y supuestos. |
| C07 | Diseñar módulos y controlar acoplamiento y cohesión | Software Architecture | Justifica límites de módulos, responsabilidades y dependencias, y explica las consecuencias de cambio. |
| C08 | Seleccionar patrones de diseño por fuerzas y consecuencias | Software Architecture | Selecciona y aplica patrones ante fuerzas concretas, explica sus costes y evita usarlos como recetas sin contexto. |
| C09 | Delimitar dominio y bounded contexts | Software Architecture | Justifica límites del dominio y contextos delimitados a partir del lenguaje, las reglas y las responsabilidades del negocio. |
| C10 | Diseñar sistemas distribuidos | Software Architecture | Compara comunicación, consistencia, coordinación, tolerancia a fallos y resiliencia para un contexto específico. |
| C11 | Elegir estilos y estrategias de descomposición | Software Architecture | Justifica monolito, modularización o distribución según drivers, restricciones, operación y coste de cambio. |
| C12 | Diseñar APIs y contratos evolutivos | Software Architecture | Define contratos claros y justifica compatibilidad, versionado, manejo de errores y estrategia de evolución. |
| C13 | Diseñar arquitectura de datos | Software Architecture | Compara modelos y estrategias de almacenamiento, acceso, consistencia, ciclo de vida y gobierno de datos según las necesidades. |
| C14 | Diseñar seguridad, resiliencia y observabilidad | Software Architecture | Analiza amenazas y modos de fallo; propone controles y señales operativas, explicando eficacia, límites y costes. |
| C15 | Diseñar cloud y evolución arquitectónica | Software Architecture | Propone una estrategia de despliegue, evolución o migración vinculada a restricciones, riesgos, operación y criterios de éxito. |
| C16 | Diseñar arquitectura para AI Engineering | Puente hacia AI Solution Architecture | Integra modelos, datos, aplicación y evaluación en una arquitectura coherente, identificando riesgos y límites propios de los componentes de IA. |
| C17 | Evaluar arquitecturas | Transversal | Compara arquitecturas con criterios explícitos, evidencia, coste, riesgo e incertidumbre, y comunica las limitaciones de la evaluación. |
| C18 | Ejercer la práctica profesional del arquitecto | Transversal | Comunica y documenta decisiones, facilita acuerdos entre stakeholders y defiende recomendaciones de forma responsable y trazable. |

## 6. Competencias específicas propuestas para AI Solution Architecture

Los IDs `AI01`–`AI10` son nuevos y se proponen para completar el segundo nivel. Su redacción, granularidad y cobertura curricular quedan pendientes de revisión.

| ID | Competencia | Evidencia de dominio esperada | Dependencias principales |
|---|---|---|---|
| AI01 | Determinar la idoneidad de IA para una necesidad | Compara una solución con IA frente a alternativas convencionales; define el valor esperado, las limitaciones, los criterios de éxito y cuándo no conviene usar IA. | C03, C05, C17, C18 |
| AI02 | Seleccionar y delimitar modelos y servicios de IA | Compara modelos locales, alojados o servicios administrados según capacidad, calidad, latencia, coste, privacidad, licencias y restricciones operativas. | C03, C05, C14, C15, C17 |
| AI03 | Diseñar arquitectura de datos y conocimiento para IA | Define procedencia, permisos, preparación, calidad, actualización, retención y ciclo de vida de los datos utilizados por la solución. | C03, C13, C14 |
| AI04 | Diseñar recuperación de información y RAG | Justifica estrategia de ingesta, fragmentación, embeddings, indexación, recuperación, reranking y generación; evalúa relevancia, fidelidad, citas y fallos de recuperación. | C05, C06, C13, AI03, AI07 |
| AI05 | Diseñar ingeniería de contexto | Define cómo seleccionar, priorizar, comprimir, actualizar y suministrar contexto a modelos o agentes; controla límites de contexto, contaminación y pérdida de información relevante. | C05, C06, C13, AI02, AI03 |
| AI06 | Diseñar agentes, herramientas y orquestación | Determina si se requieren agentes; define herramientas, permisos, límites de autonomía, estado, coordinación, manejo de errores, escalamiento y mecanismos de control. | C07, C10, C12, C14, AI01, AI02 |
| AI07 | Diseñar evaluación y verificación de sistemas de IA | Define conjuntos de evaluación, métricas y pruebas para calidad, robustez, seguridad y regresiones; combina evaluación automática con revisión humana cuando corresponda. | C04, C05, C17, AI01, AI02, AI04 |
| AI08 | Diseñar seguridad y controles de riesgo específicos de IA | Analiza amenazas como prompt injection, fuga de datos, abuso de herramientas, salidas inseguras y uso indebido; define controles, límites y pruebas de ataque. | C04, C14, AI03, AI05, AI06, AI07 |
| AI09 | Diseñar operación, observabilidad y optimización de soluciones de IA | Define señales de calidad y operación, seguimiento de latencia y coste, trazas, manejo de fallos, degradación, fallback y criterios para cambiar modelos o componentes. | C10, C14, C15, C17, AI02, AI07 |
| AI10 | Gobernar el ciclo de vida de una solución de IA | Define responsabilidades, aprobación de cambios, versionado de modelos/prompts/datos, auditoría, privacidad, gestión de proveedores y supervisión humana según el riesgo. | C14, C15, C18, AI02, AI03, AI07, AI08, AI09 |

### Límite de alcance

Esta lista no presupone que todas las soluciones necesiten RAG, agentes, embeddings propios, varios modelos o despliegue en cloud. La competencia consiste en decidir con fundamento qué componentes se requieren, cuáles no y por qué.

## 7. Relación entre niveles y competencias

| Nivel formativo | Competencias incluidas |
|---|---|
| Software Architecture | C01–C15 |
| Transición y especialización en IA | C16, AI01–AI10 |
| Transversales | C17–C18, aplicables a ambos niveles según el contexto |

La asignación es una propuesta de organización. La ruta curricular debe determinar cuándo se introduce cada competencia, sus prerrequisitos y el nivel de dominio esperado en cada clase.

Las competencias transversales no deben duplicarse en dos listas. La evidencia exigida debe escalar según el tipo de solución, el riesgo, la complejidad y el impacto.

## 8. Regla de validación del dominio

Una competencia no se considera dominada por exposición, memorización o por producir una respuesta plausible una sola vez.

La validación requiere:

1. Criterios específicos y observables para el nivel evaluado.
2. Evidencia identificable, con contexto, alcance y fecha.
3. Correspondencia explícita entre evidencia y criterios.
4. Aplicación a un caso nuevo cuando se evalúe APLICAR.
5. Registro de supuestos, límites e incertidumbre cuando sean relevantes.
6. Revisión humana para decisiones de evaluación de alto impacto o cuando la evidencia automatizada no sea suficiente.
7. Estado explícito: pendiente, en revisión, cumple parcialmente o validado, según la convención que se apruebe para el curso.

No se debe inferir dominio de una competencia a partir de otra relacionada ni de la aprobación de una clase completa, salvo que la evidencia cubra los criterios correspondientes.

## 9. Trazabilidad curricular y evaluación

Cada plan de clase debe declarar:

- IDs de las competencias objetivo.
- Niveles de dominio que pretende desarrollar o evaluar.
- Prerrequisitos necesarios.
- Actividad y evidencia que permitan observar el resultado.
- IDs de criterios aplicables (`CR-...`).
- Rúbrica o regla de decisión correspondiente.
- Limitaciones de la evidencia y estado de revisión.

El registro de trazabilidad debe relacionar clase, competencia, criterio, evidencia y estado de revisión. Las rúbricas deben concretar los criterios en indicadores observables y umbrales adecuados al objetivo. Estos documentos deben referenciar esta matriz, no redefinir las competencias por separado.

## 10. Mejoras futuras y control de cambios

La matriz se encuentra aprobada como línea base curricular. Los siguientes puntos son oportunidades de mejora continua, no bloqueos para su estado FINAL:

- Verificar periódicamente que C01–C18 y sus asignaciones sigan alineadas con la ruta curricular activa.
- Revisar con evidencia de uso si AI01–AI10 tienen la granularidad adecuada o si alguna competencia debe dividirse o combinarse.
- Comprobar que las competencias específicas de IA cubran las necesidades del curso sin imponer tecnologías particulares.
- Precisar, cuando se diseñen evaluaciones concretas, los niveles mínimos esperados por competencia y etapa curricular; no exigir automáticamente APLICAR en todas las clases.
- Alinear los criterios específicos y las rúbricas de cada clase con esta matriz.
- Revisar la trazabilidad de los planes de clase y corregir enlaces a identificadores o evidencias históricas que dejen de ser válidos.
- Mantener coherentes el nombre canónico del curso y la estructura de carpetas del repositorio.
- Usar pruebas piloto de evaluación para informar futuras revisiones, sin invalidar esta aprobación inicial.

Cualquier cambio sustantivo deberá realizarse mediante una modificación versionada, con su justificación y trazabilidad en Git.

## 11. Estado del documento

**Estado actual:** FINAL — APPROVED.

La matriz maestra queda aprobada como referencia curricular para alinear rutas de aprendizaje, clases, criterios, rúbricas y evidencias. Esta aprobación no acredita el dominio de ninguna persona ni elimina la posibilidad de corregir o ampliar la matriz mediante futuras versiones revisadas. Los cambios se registrarán en el historial de Git.
